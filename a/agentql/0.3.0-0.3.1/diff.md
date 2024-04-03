# Comparing `tmp/agentql-0.3.0.tar.gz` & `tmp/agentql-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.3.0.tar", max compression
+gzip compressed data, was "agentql-0.3.1.tar", max compression
```

## Comparing `agentql-0.3.0.tar` & `agentql-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1066 2024-03-25 21:27:04.768579 agentql-0.3.0/LICENSE
--rw-r--r--   0        0        0      111 2024-03-25 21:27:04.768579 agentql-0.3.0/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-03-25 21:27:04.856580 agentql-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      152 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/__init__.py
--rw-r--r--   0        0        0      183 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/core.py
--rw-r--r--   0        0        0     1322 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/popup.py
--rw-r--r--   0        0        0     5053 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/response_proxy.py
--rw-r--r--   0        0        0     8982 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/session.py
--rw-r--r--   0        0        0      301 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/web/__init__.py
--rw-r--r--   0        0        0     3747 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/web/network_monitor.py
--rw-r--r--   0        0        0    22054 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/web/playwright_driver.py
--rw-r--r--   0        0        0     3506 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/async_api/web/web_driver.py
--rw-r--r--   0        0        0        0 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/__init__.py
--rw-r--r--   0        0        0       78 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/api_constants.py
--rw-r--r--   0        0        0      247 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/aria_constants.py
--rw-r--r--   0        0        0      193 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/driver_constants.py
--rw-r--r--   0        0        0      367 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/driver_settings.py
--rw-r--r--   0        0        0     4487 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/errors.py
--rw-r--r--   0        0        0     1980 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/html_constants.py
--rw-r--r--   0        0        0        0 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     5644 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/character_utils.py
--rw-r--r--   0        0        0     5011 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/node.py
--rw-r--r--   0        0        0     4695 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/source.py
--rw-r--r--   0        0        0     1602 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/token.py
--rw-r--r--   0        0        0      213 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/syntax/token_kind.py
--rw-r--r--   0        0        0      192 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/common/utils.py
--rw-r--r--   0        0        0      183 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     1036 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/core.py
--rw-r--r--   0        0        0     1242 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/popup.py
--rw-r--r--   0        0        0     4509 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/response_proxy.py
--rw-r--r--   0        0        0     8704 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/session.py
--rw-r--r--   0        0        0      301 2024-03-25 21:27:04.856580 agentql-0.3.0/src/agentql/sync_api/web/__init__.py
--rw-r--r--   0        0        0    21473 2024-03-25 21:27:04.860580 agentql-0.3.0/src/agentql/sync_api/web/playwright_driver.py
--rw-r--r--   0        0        0     3046 2024-03-25 21:27:04.860580 agentql-0.3.0/src/agentql/sync_api/web/web_driver.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-03 04:03:14.917107 agentql-0.3.1/LICENSE
+-rw-r--r--   0        0        0      111 2024-04-03 04:03:14.917107 agentql-0.3.1/PACKAGE_README.md
+-rw-r--r--   0        0        0      771 2024-04-03 04:03:15.005108 agentql-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/__init__.py
+-rw-r--r--   0        0        0      183 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     1799 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/core.py
+-rw-r--r--   0        0        0     1605 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/popup.py
+-rw-r--r--   0        0        0     5520 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/response_proxy.py
+-rw-r--r--   0        0        0    10846 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/session.py
+-rw-r--r--   0        0        0      301 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/__init__.py
+-rw-r--r--   0        0        0     3813 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/network_monitor.py
+-rw-r--r--   0        0        0    26961 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/playwright_driver.py
+-rw-r--r--   0        0        0     5806 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/async_api/web/web_driver.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/__init__.py
+-rw-r--r--   0        0        0       78 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/api_constants.py
+-rw-r--r--   0        0        0      247 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/aria_constants.py
+-rw-r--r--   0        0        0      193 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/driver_constants.py
+-rw-r--r--   0        0        0      367 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/driver_settings.py
+-rw-r--r--   0        0        0     4741 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/errors.py
+-rw-r--r--   0        0        0     1980 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/html_constants.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     5986 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      145 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-04-03 04:03:15.005108 agentql-0.3.1/src/agentql/common/js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/character_utils.py
+-rw-r--r--   0        0        0     5011 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/lexer.py
+-rw-r--r--   0        0        0     2431 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/node.py
+-rw-r--r--   0        0        0     4695 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/token.py
+-rw-r--r--   0        0        0      213 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/syntax/token_kind.py
+-rw-r--r--   0        0        0      192 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/common/utils.py
+-rw-r--r--   0        0        0      183 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     1759 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/core.py
+-rw-r--r--   0        0        0     1525 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/popup.py
+-rw-r--r--   0        0        0     4976 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/response_proxy.py
+-rw-r--r--   0        0        0    10597 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/session.py
+-rw-r--r--   0        0        0      301 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/__init__.py
+-rw-r--r--   0        0        0    26810 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/playwright_driver.py
+-rw-r--r--   0        0        0     4922 2024-04-03 04:03:15.009108 agentql-0.3.1/src/agentql/sync_api/web/web_driver.py
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.3.1/PKG-INFO
```

### Comparing `agentql-0.3.0/LICENSE` & `agentql-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/pyproject.toml` & `agentql-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentql"
-version = "0.3.0"
+version = "0.3.1"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `agentql-0.3.0/src/agentql/async_api/core.py` & `agentql-0.3.1/src/agentql/sync_api/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 """
 This module is an entrypoint to AgentQL service
 """
 
 import logging
 from typing import Any
 
-from agentql.async_api.web import (
-    InteractiveItemTypeT,
-    PageTypeT,
-    PlaywrightWebDriver,
-    WebDriver,
-)
+from agentql.sync_api.web import InteractiveItemTypeT, PageTypeT, PlaywrightWebDriver, WebDriver
 
 from .session import Session
 
 log = logging.getLogger(__name__)
 
 
-async def start_async_session(
-    url: str,
+def start_session(
+    url: str = "",
     *,
     web_driver: WebDriver[InteractiveItemTypeT, PageTypeT] = PlaywrightWebDriver(),
     user_auth_session: Any = None,
 ) -> Session[InteractiveItemTypeT, PageTypeT]:
-    """Start a new asynchronous AgentQL session.
+    """Start a new synchronous AgentQL session with the given URL, web driver and user authentication session. By default, session will use Playwright Web Driver.
 
     Parameters:
-
-    url (str): The URL to start the session with.
-    web_driver (optional): The web driver to use. Defaults to Playwright web driver.
-    user_auth_session (optional): The user authentication session.
+    ----------
+    url (str): URL to navigate session to. To navigate after a session has already started, users could start session with an initialized web driver and invoke `driver.open_url()` method.
+    web_driver (webDriver) (optional): Web driver is responsible for interacting with the browser and page. Defaults to Playwright web driver, which is built on top of the [Playwright framework](https://playwright.dev/python/).
+    user_auth_session (dict) (optional): The user authentication session that contains previous login session. Users could retrieve authentication session by starting a session, logging into desired website, and calling `session.get_user_auth_session()`, which will return a `auth_session` object defined in web driver.
 
     Returns:
-
-    Session: The new session.
+    -------
+    Session: An instance of AgentQL Session class for synchronous environment.
     """
-    log.debug(f"Starting asynchronous session with {url}")
+    log.debug(f"Starting session with {url}")
 
-    await web_driver.start_browser(user_auth_session=user_auth_session)
-    await web_driver.open_url(url)
+    web_driver.start_browser(user_auth_session=user_auth_session)
+    if url:
+        web_driver.open_url(url)
     session = Session[InteractiveItemTypeT, PageTypeT](web_driver)
     return session
```

### Comparing `agentql-0.3.0/src/agentql/async_api/popup.py` & `agentql-0.3.1/src/agentql/sync_api/popup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,50 @@
-import asyncio
 from typing import Callable
 
 
 class Popup:
-    """The Popup class represents a popup dialog in the page."""
+    """Popup objects are dispatched by session via session.on("popup") event. For each popup window detected on the page, there will be corresponding event and popup objects emitted."""
 
     def __init__(self, popup_tree: dict, popup_name: str, on_popup_close: Callable[[dict], None]):
         self._tree = popup_tree
         self._name = popup_name
         self._close_popup_callback = on_popup_close
 
     def __str__(self):
         return f"Popup {self._name}"
 
+    @property
     def accessibility_tree(self) -> dict:
         """
         Returns the part of accessibility tree where the popup node as the parent.
 
         Returns:
+        --------
         dict: The part of accessibility tree wheree the popup no9de as the parent.
         """
         return self._tree
 
+    @property
     def name(self) -> str:
         """
         Returns the name of the popup.
 
         Returns:
+        --------
         str: The name of the popup.
         """
         return self._name
 
-    async def close(self):
-        """Close the popup."""
-        await self._close_popup_callback(self._tree)
+    def close(self):
+        """Close the popup by invoking the callback function passed into the Popup object when it is initialized."""
+        self._close_popup_callback(self._tree)
 
 
-async def close_all_popups_handler(popups: list):
-    """This is a asynchronous handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
+def close_all_popups_handler(popups: list):
+    """This is a handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
 
     Parameters:
-
+    ----------
     popups(list): The list containing popup objects.
     """
-    tasks = [popup.close() for popup in popups]
-    await asyncio.gather(*tasks)
+    for popup in popups:
+        popup.close()
```

### Comparing `agentql-0.3.0/src/agentql/async_api/response_proxy.py` & `agentql-0.3.1/src/agentql/sync_api/response_proxy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-import asyncio
 import json
 import logging
 from typing import Generic, Union
 
-from agentql.async_api.web import InteractiveItemTypeT, WebDriver
 from agentql.common.errors import AttributeNotFoundError
 from agentql.common.syntax.node import ContainerListNode, ContainerNode, IdListNode, IdNode
+from agentql.sync_api.web import InteractiveItemTypeT, WebDriver
 
-log = logging.getLogger("agentql")
+log = logging.getLogger(__name__)
 
 
 class AQLResponseProxy(Generic[InteractiveItemTypeT]):
+    """
+    AQLResponseProxy class acts as a dynamic proxy to the response received from AgentQL server. It allows users to interact with resulting web elements and to retrieve their text contents. This class is designed to work with the web driver to fetch and process query results.
+    """
+
     def __init__(
         self,
         data: dict,
         web_driver: "WebDriver[InteractiveItemTypeT]",
         query_tree: ContainerNode,
     ):
         self._response_data = data
@@ -57,69 +60,60 @@
         if self._response_data is None:
             return 0
         return len(self._response_data)
 
     def __str__(self):
         return json.dumps(self._response_data, indent=2)
 
-    async def to_data(self) -> dict:
+    def to_data(self) -> dict:
         """Converts the response data into a structured dictionary based on the query tree.
 
         Returns:
-        dict: A structured dictionary representing the processed response data, with fact nodes replaced by name (values) from the response data.
+        --------
+        dict: A structured dictionary representing the processed response data, with fact nodes replaced by name (values) from the response data. It will have the following structure:
+
+        ```py
+        {
+        "query_field": "text content of the corresponding web element"
+        }
+        ```
         """
-        return await self._to_data_node(self._response_data, self._query_tree_node)
+        return self._to_data_node(self._response_data, self._query_tree_node)
 
-    async def _to_data_node(self, response_data, query_tree_node) -> dict:
+    def _to_data_node(self, response_data, query_tree_node) -> dict:
         if isinstance(query_tree_node, ContainerListNode):
-            return await self._to_data_container_list_node(response_data, query_tree_node)
+            return self._to_data_container_list_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, ContainerNode):
-            return await self._to_data_container_node(response_data, query_tree_node)
+            return self._to_data_container_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, IdListNode):
-            return await self._to_data_id_list_node(response_data)
+            return self._to_data_id_list_node(response_data)
         elif isinstance(query_tree_node, IdNode):
-            return await self._to_data_id_node(response_data)
+            return self._to_data_id_node(response_data)
         else:
             raise TypeError("Unsupported query tree node type")
 
-    async def _to_data_container_node(
-        self, response_data: dict, query_tree_node: ContainerNode
-    ) -> dict:
-        tasks = []
-        children = []
-
+    def _to_data_container_node(self, response_data: dict, query_tree_node: ContainerNode) -> dict:
+        data_dict = {}
         for child_name, child_data in response_data.items():
             child_query_tree = query_tree_node.get_child_by_name(child_name)
+            data_dict[child_name] = self._to_data_node(child_data, child_query_tree)
+        return data_dict
 
-            task = asyncio.create_task(self._to_data_node(child_data, child_query_tree))
-            tasks.append(task)
-            children.append(child_name)
-
-        # run all tasks concurrently.
-        results = await asyncio.gather(*tasks)
-
-        return {child_name: result for result, child_name in zip(results, children)}
-
-    async def _to_data_container_list_node(
+    def _to_data_container_list_node(
         self, response_data: dict, query_tree_node: ContainerListNode
     ) -> list:
-        tasks = [self._to_data_container_node(item, query_tree_node) for item in response_data]
-        result_list = await asyncio.gather(*tasks)
-        return result_list
+        return [self._to_data_container_node(item, query_tree_node) for item in response_data]
 
-    async def _to_data_id_node(self, response_data: dict) -> dict:
+    def _to_data_id_node(self, response_data: dict) -> dict:
         if response_data is None:
             return None
         name = response_data.get("name")
         if not name or not name.strip():
             web_element = self._web_driver.locate_interactive_element(response_data)
             if not web_element:
                 log.warning(f"Could not locate web element for item {response_data}")
                 return None
-            element_text = await self._web_driver.get_text_content(web_element)
-            name = element_text.strip()
+            name = self._web_driver.get_text_content(web_element)
         return name
 
-    async def _to_data_id_list_node(self, response_data: list) -> list:
-        tasks = [self._to_data_id_node(item) for item in response_data]
-        res = await asyncio.gather(*tasks)
-        return [node for node in res if node is not None]
+    def _to_data_id_list_node(self, response_data: list) -> list:
+        return [node for item in response_data if (node := self._to_data_id_node(item)) is not None]
```

### Comparing `agentql-0.3.0/src/agentql/async_api/session.py` & `agentql-0.3.1/src/agentql/async_api/session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import logging
 import os
-from typing import Callable, Generic, List, Literal
+from typing import Callable, Generic, List, Literal, Optional
 
 import httpx
 
 from agentql.async_api.popup import Popup
 from agentql.async_api.web import InteractiveItemTypeT, PageTypeT, WebDriver
 from agentql.common.api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
 from agentql.common.errors import (
@@ -22,123 +22,158 @@
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
 AGENTQL_API_KEY = os.getenv("AGENTQL_API_KEY")
 
 
 class Session(Generic[InteractiveItemTypeT, PageTypeT]):
-    """An asynchronous session with a AgentQL service. It is responsible for querying and managing session-related state (like authentication)."""
+    """Session class contains core functionality of AgentQL service. It is responsible for querying elements, managing session-related state (like authentication), and handling various events."""
 
     def __init__(self, web_driver: WebDriver[InteractiveItemTypeT, PageTypeT]):
         """Initialize the session.
 
         Parameters:
-
+        ----------
         web_driver (WebDriver): The web driver that will be used in this session.
         """
         if AGENTQL_API_KEY:
             self._api_key = AGENTQL_API_KEY
         else:
             raise APIKeyError(
                 "API key not provided. Please set the environment variable 'AGENTQL_API_KEY' with your API key."
             )
         self._web_driver = web_driver
         self._event_listeners = {}
         self._check_popup = False
+        self._last_query = None
+        self._last_response = None
 
     @property
     async def current_page(self) -> PageTypeT:
-        """Get the current page."""
+        """Get the current page being processed by AgentQL.
+
+        Returns:
+        -------
+        PageTypeT: A type variable representing the type of a page in a web driver session. If you did not pass a customized web driver when starting the session, then it will return [Playwright Page](https://playwright.dev/python/docs/api/class-page) object.
+        """
         return await self._web_driver.get_current_page()
 
     @property
     def driver(self) -> WebDriver[InteractiveItemTypeT, PageTypeT]:
-        """Get the web driver."""
+        """Get the web driver.
+
+        Returns:
+        -------
+        WebDriver: A protocol representing the web driver. If you did not pass a customized web driver when starting the session, default PlaywrightWebDriver will be returned.
+        """
         return self._web_driver
 
+    @property
+    def last_query(self) -> Optional[str]:
+        """Get the last query."""
+        return self._last_query
+
+    @property
+    def last_response(self) -> Optional[dict]:
+        """Get the last response."""
+        return self._last_response
+
     async def query(
         self,
         query: str,
         timeout: int = 500,
         lazy_load_pages_count: int = 0,
         wait_for_network_idle: bool = True,
+        include_aria_hidden: bool = False,
     ) -> AQLResponseProxy[InteractiveItemTypeT]:
         """Query the web page tree for elements that match the AgentQL query.
 
         Parameters:
-
-        query (str): The query string.
-        timeout (optional): Optional timeout value for the connection with backend api service.
-        lazy_load_pages_count (optional): The number of pages to scroll down and up to load lazy loaded content.
-        wait_for_network_idle (optional): Whether to wait for the network to be idle before querying the page.
+        ----------
+        query (str): The AgentQL query in String format.
+        timeout (int) (optional): Optional timeout value for the connection with backend api service.
+        lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
+        wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
 
         Returns:
-
-        dict: AgentQL Response (Elements that match the query)
+        -------
+        AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         log.debug(f"querying {query}")
 
+        self._last_query = query
         parser = Parser(query)
         query_tree = parser.parse()
 
         await self._web_driver.wait_for_page_ready_state(
             wait_for_network_idle=wait_for_network_idle
         )
 
-        accessibility_tree = await self._web_driver.prepare_accessiblity_tree(
-            lazy_load_pages_count=lazy_load_pages_count
+        accessibility_tree = await self._web_driver.prepare_accessibility_tree(
+            lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
         # Check if there is a popup in the page before sending the agentql query
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 await self._handle_popup(popup_list)
 
         response = await self._query(query, accessibility_tree, timeout)
+        self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
             accessibility_tree = await self._web_driver.get_accessibility_tree()
 
             popup_list = self._detect_popup(accessibility_tree, popup_list)
             if popup_list:
                 await self._handle_popup(popup_list)
 
         return AQLResponseProxy[InteractiveItemTypeT](response, self._web_driver, query_tree)
 
-    async def get_user_auth_session(self):
-        """Get the user authentication session."""
+    async def get_user_auth_session(self) -> dict:
+        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+
+        Returns:
+        --------
+        User auth session in Python dictionary format.
+        """
         return await self._web_driver.get_user_auth_session()
 
     async def stop(self):
         """Close the session."""
         log.debug("closing session")
         await self._web_driver.stop_browser()
 
     def on(self, event: Literal["popup"], callback: Callable[[dict], None]):
-        """Emitted when there is a popup on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections."""
+        """Emitted when there is a popup (such as promotion window) on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections.
+
+        Event Data:
+        -----------
+        popups (list): The list of popups captured on the page by AgentQL Popup Detection algorithm.
+        """
         self._event_listeners[event] = callback
         if callback:
             self._check_popup = True
         else:
             self._check_popup = False
 
     async def _query(self, query: str, accessibility_tree: dict, timeout: int) -> dict:
         """Make Request to AgentQL API.
 
         Parameters:
-
+        ----------
         query (str): The query string.
         accessibility_tree (dict): The accessibility tree.
         timeout (int): The timeout value for the connection with backend api service
 
         Returns:
-
+        -------
         dict: AgentQL response in json format.
         """
         try:
             page_url = await self._web_driver.get_current_url()
             request_data = {
                 "query": f"{query}",
                 "accessibility_tree": accessibility_tree,
@@ -173,19 +208,20 @@
         except httpx.RequestError as e:
             raise AgentQLServerError(str(e)) from e
 
     def _detect_popup(self, tree: dict, known_popups: List[Popup]) -> List[Popup]:
         """Detect if there is a popup in the page. If so, create a Popup object and add it to the popup dict.
 
         Parameters:
-
+        ----------
         tree (dict): The accessibility tree.
         known_popups (list): The list of known popups.
 
         Returns:
+        --------
         popups (list): The list of popups.
         """
         tree_role = tree.get("role", "")
         tree_name = tree.get("name", "")
         popup_list = []
         if tree_role == "dialog":
             popup = Popup(copy.deepcopy(tree), tree_name, self._close_popup)
@@ -206,25 +242,26 @@
 
         return popup_list
 
     async def _handle_popup(self, popups: List[Popup]):
         """Handle the popup. If there is a popup in the list, and there is an event listener, emit the popup event by invoking the callback function.
 
         Parameters:
-
+        ----------
         popups (list): The list of popups to handle."""
         if popups and "popup" in self._event_listeners and self._event_listeners["popup"]:
             await self._event_listeners["popup"](popups)
 
     async def _close_popup(self, tree: dict):
-        """Close the popup.
+        """Close the popup by querying AgentQL server and click the close button.
 
         Parameters:
-
+        ----------
         popup (Popup): The popup to close.
+        query (str): The query to close the popup.
         """
         query = """
             {
                 popup {
                     close_btn
                 }
             }
```

### Comparing `agentql-0.3.0/src/agentql/async_api/web/network_monitor.py` & `agentql-0.3.1/src/agentql/async_api/web/network_monitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,50 +13,50 @@
         self._page_loaded = False
         self._start_time = time.time()
 
     def track_network_request(self, request):
         """Track a request and record its timestamp into the _last_network_active_time.
 
         Parameters:
-
+        ----------
         request (requests.PreparedRequest): The request to track."""
         self._last_network_active_time = time.time()
         # Start logging duplicate urls after the first 6 seconds
         if time.time() - self._start_time > 6:
             if request.url in self._request_log:
                 self._multi_request_found = True
         self._request_log[request.url] = time.time()
 
     def track_network_response(self, response):
         """Track a response and mark it in the network log.
 
         Parameters:
-
+        ----------
         response (requests.Response): The response to track."""
         self._last_network_active_time = time.time()
         if response.url in self._request_log:
             self._response_log.add(response.url)
 
     def track_load(self):
         """Track whether the current page has loaded to make sure navigation is finished."""
         self._page_loaded = True
 
     def get_load_status(self):
         """Get the status of the page load.
 
         Returns:
-
+        -------
         bool: True if the page has loaded, False otherwise."""
         return self._page_loaded
 
     def check_conditions(self, last_active_dom_time=None) -> bool:
         """Check if the conditions for Page Ready state have been met
 
         Returns:
-
+        -------
         bool: True if the conditions for Page Ready State have been met, False otherwise."""
         dom_is_quiet = False
         network_is_quiet = False
 
         # Check if DOM has changed
         if last_active_dom_time:
             last_active_dom_time = float(last_active_dom_time) / 1000
```

### Comparing `agentql-0.3.0/src/agentql/async_api/web/playwright_driver.py` & `agentql-0.3.1/src/agentql/async_api/web/playwright_driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 import time
-from typing import Union
+from typing import Optional, Union
 
 from playwright.async_api import Error, Frame, Locator, Page, StorageState, async_playwright
 from playwright_stealth import StealthConfig, stealth_async
 
 from agentql.async_api.web.network_monitor import PageActivityMonitor
 from agentql.async_api.web.web_driver import WebDriver
 from agentql.common.driver_constants import RENDERER, USER_AGENT, VENDOR
@@ -20,15 +20,31 @@
 from agentql.common.js_snippets.snippet_loader import load_js
 from agentql.common.utils import ensure_url_scheme
 
 from .web_driver import WebDriver
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
+    """
+    PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
+    """
+
     def __init__(self, headless=True, proxy: ProxySettings = None) -> None:
+        """
+        Construct the PlaywrightWebDriver instance.
+
+        Parameters:
+        -----------
+        headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
+        proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
+
+        Returns:
+        --------
+        PlaywrightWebDriver: An instance of PlaywrightWebDriver.
+        """
         self._playwright = None
 
         self._browser = None
         """The current browser. Only use this to close the browser session in the end."""
 
         self._context = None
         """The current browser context. Use this to open a new page"""
@@ -51,55 +67,64 @@
         self._stealth_mode_config = None
 
     def locate_interactive_element(self, response_data: dict) -> Locator:
         """
         Locates an interactive element in the web page.
 
         Parameters:
+        -----------
 
         response_data (dict): The data of the interactive element from the AgentQL response.
 
         Returns:
+        --------
 
-        Locator: The interactive element.
+        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
         """
         tf623_id = response_data.get("tf623_id")
         if not tf623_id:
             raise ElementNotFoundError("tf623_id")
         iframe_path = response_data.get("attributes", {}).get("iframe_path")
         return self.find_element_by_id(tf623_id, iframe_path)
 
     async def get_text_content(self, web_element: Locator) -> str:
         """
         Gets the text content of the web element.
 
         Parameters:
+        -----------
 
-        web_element (Locator): The web element.
+        web_element ([Playwright Locator](https://playwright.dev/python/docs/api/class-locator)): The web element represented by Playwright's Locator object.
 
         Returns:
+        --------
 
         str: The text content of the web element.
         """
         return await web_element.text_content()
 
     async def start_browser(self, user_auth_session: StorageState = None):
         """
         Starts a new browser session and set user session state (if there is any).
 
         Parameters:
+        -----------
         user_auth_session (optional): The user authentication session information.
         """
         await self._start_browser(
             headless=self._headless, user_session_extras=user_auth_session, proxy=self._proxy
         )
 
     @property
     def is_headless(self) -> bool:
-        """Returns whether the browser is running in headless mode or not."""
+        """Returns whether the browser is running in headless mode or not.
+
+        Returns:
+        --------
+        bool: True if the browser is running in headless mode, False otherwise."""
         return self._headless
 
     async def stop_browser(self):
         """Closes the current browser session."""
         if self._context:
             await self._context.close()
             self._context = None
@@ -110,117 +135,168 @@
             await self._playwright.stop()
             self._playwright = None
 
     def enable_stealth_mode(
         self,
         webgl_vendor: str = VENDOR,
         webgl_renderer: str = RENDERER,
-        nav_user_agent: str | None = USER_AGENT,
+        nav_user_agent: Optional[str] = USER_AGENT,
     ):
         """Enable the stealth mode and set the stealth mode configuration.
         Ideally parameters values should match some real values to avoid detection.
         To get a realistic examples, you can use browser fingerprinting websites such as https://bot.sannysoft.com/ and https://pixelscan.net/
 
         Parameters:
-        webgl_vendor (str): The WebGL vendor to use.
-        webgl_renderer (str): The WebGL renderer to use.
-        nav_user_agent (str): The navigator user agent to use.
+        -----------
+        webgl_vendor (str) (optional):
+            The vendor of the GPU used by WebGL to render graphics, such as `Apple Inc.`. After setting this parameter, your browser will emit this vendor information.
+        webgl_renderer (str) (optional):
+            Identifies the specific GPU model or graphics rendering engine used by WebGL, such as `Apple M3`. After setting this parameter, your browser will emit this renderer information.
+        nav_user_agent (str) (optional):
+            Identifies the browser, its version, and the operating system, such as `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36`. After setting this parameter, your browser will send this user agent information to the website.
         """
         self._stealth_mode_config = StealthModeConfig(
             vendor=webgl_vendor, renderer=webgl_renderer, nav_user_agent=nav_user_agent
         )
 
-    async def open_url(self, url: str):
-        """
-        Opens a new page and navigates to the given URL.
+    async def open_url(self, url: str, new_page: bool = False):
+        """Open URL in the browser.
+
+        Parameters:
+        ----------
+        url (str): The URL to open.
+        new_page (bool): Whether to open the URL in a new tab in that tab. To navigate to a new url with the current tab, use Playwright Page object's [page.goto()](https://playwright.dev/python/docs/api/class-page#page-goto) method.
         """
         if not self._browser:
             raise NoOpenBrowserError()
-        await self._open_url(url)
+        if new_page or self._current_page is None:
+            await self._open_url(url)
+        else:
+            await self._current_page.goto(url, wait_until="load")
 
     async def get_current_url(self) -> str:
-        """Get the URL of the active page."""
+        """Get the URL of the current page being processed by AgentQL.
+
+        Returns:
+        --------
+        str: The URL of the current page.
+        """
         if not self._current_page:
             raise NoOpenPageError()
         return self._current_page.url
 
     async def get_html(self) -> dict:
         """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page".
 
         Returns:
-
-        string: The HTML content of the web page.
+        --------
+        dict: The HTML content of the web page in Dict format.
         """
         if not self._current_page:
-            raise ValueError('No page is open. Make sure you call "open_url()" first.')
+            raise NoOpenPageError()
         return self._original_html
 
     async def get_current_page(self) -> Page:
-        """Returns the current page.
+        """Returns the [Playwright page object](https://playwright.dev/python/docs/api/class-page) that represents the current page. Users could do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
-
-        Page: The current page.
+        --------
+        [Playwright Page](https://playwright.dev/python/docs/api/class-page): The current page.
         """
         if not self._current_page:
-            raise ValueError('No page is open. Make sure you call "open_url()" first.')
+            raise NoOpenPageError()
         return self._current_page
 
     async def open_html(self, html: str):
         """
         Opens a new page and loads the given HTML content.
+
+        Parameters:
+        -----------
+        html (str): The HTML content to load in the page.
         """
         if not self._browser:
             raise NoOpenBrowserError()
         self._current_page = await self._context.new_page()
         self._current_tf_id = 0
         await self._current_page.set_content(html)
 
-    async def prepare_accessiblity_tree(self, lazy_load_pages_count: int = 3) -> dict:
+    async def prepare_accessibility_tree(
+        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
+    ) -> dict:
         """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
 
         Parameters:
+        -----------
         lazy_load_pages_count: The number of times to scroll down and up the page.
 
         Returns:
+        --------
         dict: AT of the page
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         self._original_html = await self._current_page.content()
         await self._page_scroll(pages=lazy_load_pages_count)
 
         accessibility_tree = None
         try:
-            accessibility_tree = await self._get_page_accessibility_tree(self._current_page)
+            accessibility_tree = await self._get_page_accessibility_tree(
+                self._current_page, include_aria_hidden=include_aria_hidden
+            )
             await self._process_iframes(accessibility_tree)
             await self._post_process_accessibility_tree(accessibility_tree)
 
         except Exception as e:
             raise AccessibilityTreeError() from e
 
         return accessibility_tree
 
     async def get_accessibility_tree(self) -> dict:
         """Returns the up-to-date accessibility tree of the page.
 
         Returns:
-        dict: The accessibility tree of the page.
+        --------
+        dict: The accessibility tree of the page in Dict format.
         """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         try:
             accessibility_tree = await self._get_page_accessibility_tree(self._current_page)
             await self._process_iframes(accessibility_tree)
         except Exception as e:
             raise AccessibilityTreeError() from e
 
         return accessibility_tree
 
     async def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
-        """Wait for the page to reach the "Page Ready" or stable state."""
+        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
+
+        Usage:
+        -----
+        ```py
+        session = agentql.start_async_session(YOUTUBE_URL)
+
+        # Scroll to bottom to trigger comments loading
+        await session.driver.scroll_to_bottom()
+
+        # Wait for comments to load before making a query
+        await session.driver.wait_for_page_ready_state()
+        await session.query(QUERY)
+        ```
+
+        Parameters:
+        -----------
+        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
+        """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if not self._page_monitor:
             self._page_monitor = PageActivityMonitor()
         else:
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
@@ -229,42 +305,51 @@
         # Wait for the page to reach the "Page Ready" state
         await self._determine_load_state(self._page_monitor, wait_for_network_idle)
 
         # Remove the event listeners to prevent overwhelming the async event loop
         await self._remove_page_event_listeners()
 
     async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
-        """Scrolls the page up or down.
+        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
-        scroll_direction (ScrollDirection): The direction to scroll the page.
-        pixels (int): The number of pixels to scroll.
+        -----------
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         await self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
 
     async def scroll_to_bottom(self):
-        """Scrolls the page to the bottom."""
+        """Scrolls to the bottom of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         await self._current_page.evaluate(load_js("scroll_to_bottom"))
 
     async def scroll_to_top(self):
-        """Scrolls the page to the top."""
+        """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         await self._current_page.evaluate(load_js("scroll_to_top"))
 
     async def get_user_auth_session(self) -> StorageState:
-        """Returns the user auth session state of the browser."""
+        """
+        **NOT RECOMMENDED** (Use session.get_user_auth_session() instead)
+
+        Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+
+        Returns:
+        --------
+        dict: User auth session in Python dictionary format.
+        """
         if not self._browser:
             raise NoOpenBrowserError()
         return await self._context.storage_state()
 
     async def _post_process_accessibility_tree(self, accessibility_tree: dict):
         """Post-process the accessibility tree by removing node's attributes that are Null."""
         if "children" in accessibility_tree and accessibility_tree.get("children") is None:
@@ -280,20 +365,18 @@
         iframe_path: str = "",
         frame: Frame = None,
     ):
         """
         Recursively retrieves the accessibility trees for all iframes in a page or frame.
 
         Parameters:
-            iframe_path (str): The path of the iframe in the frame hierarchy.
-            frame (Frame): The frame object representing the current frame.
-            page_accessibility_tree (dict): The accessibility tree of the page.
-
-        Returns:
-            None
+        ----------
+        iframe_path (str): The path of the iframe in the frame hierarchy.
+        frame (Frame): The frame object representing the current frame.
+        page_accessibility_tree (dict): The accessibility tree of the page.
         """
         if frame is None:
             iframes = await self._current_page.query_selector_all("iframe")
         else:
             content_frame = await frame.content_frame()
             iframes = await content_frame.query_selector_all("iframe")
 
@@ -313,47 +396,54 @@
 
             await self._process_iframes(
                 iframe_path=iframe_path_to_send,
                 frame=iframe,
                 page_accessibility_tree=page_accessibility_tree,
             )
 
-    async def _get_page_accessibility_tree(self, context: Union[Page, Frame]) -> dict:
+    async def _get_page_accessibility_tree(
+        self, context: Union[Page, Frame], include_aria_hidden: bool = False
+    ) -> dict:
         """
         Retrieves the accessibility tree for the given page.
 
         Parameters:
-            context (Page | Frame): The context in which to retrieve the accessibility tree.
+        ----------
+        context (Page | Frame): The context in which to retrieve the accessibility tree.
 
         Returns:
-            dict: The accessibility tree for the page.
+        --------
+        dict: The accessibility tree for the page.
         """
         result = await context.evaluate(
             load_js("generate_accessibility_tree"),
             {
                 "currentGlobalId": self._current_tf_id,
                 "roleTagMap": HTML_ROLE_MAPPING,
                 "processIFrames": False,
+                "includeAriaHidden": include_aria_hidden,
             },
         )
 
         self._current_tf_id = result.get("lastUsedId")
 
         return result.get("tree")
 
     async def _get_frame_accessibility_tree(self, frame: Frame, iframe_path) -> dict:
         """
         Retrieves the accessibility tree for a given frame.
 
         Parameters:
-            frame (Frame): The frame for which to retrieve the accessibility tree.
-            iframe_path: The path of the iframe within the frame.
+        ----------
+        frame (Frame): The frame for which to retrieve the accessibility tree.
+        iframe_path: The path of the iframe within the frame.
 
         Returns:
-            dict: The accessibility tree for the frame.
+        --------
+        dict: The accessibility tree for the frame.
         """
         frame_context = await frame.content_frame()
 
         if not frame_context:
             return {}
 
         await self._set_iframe_path(context=frame_context, iframe_path=iframe_path)
@@ -364,20 +454,22 @@
     def _merge_iframe_tree_into_page(
         self, iframe_id, accessibility_tree: dict, iframe_accessibility_tree: dict
     ):
         """
         Stitches the iframe accessibility tree with the page accessibility tree.
 
         Parameters:
-            iframe_id (str): The ID of the iframe.
-            accessibility_tree (dict): The accessibility tree of the page.
-            iframe_accessibility_tree (dict): The accessibility tree of the iframe.
+        ----------
+        iframe_id (str): The ID of the iframe.
+        accessibility_tree (dict): The accessibility tree of the page.
+        iframe_accessibility_tree (dict): The accessibility tree of the iframe.
 
         Returns:
-            None
+        --------
+        None
         """
         children = accessibility_tree.get("children", []) or []
         for child in children:
             attributes = child.get("attributes", {})
             if "tf623_id" in attributes and attributes["tf623_id"] == iframe_id:
                 if not child.get("children"):
                     child["children"] = []
@@ -385,14 +477,15 @@
                 break
             self._merge_iframe_tree_into_page(iframe_id, child, iframe_accessibility_tree)
 
     async def _apply_stealth_mode_to_page(self, page: Page):
         """Applies stealth mode to the given page.
 
         Parameters:
+        ----------
         page (Page): The page to which stealth mode will be applied.
         """
         # Only mask User Agent in headless mode to avoid detection for headless browsers
         mask_user_agent = self._headless
 
         await stealth_async(
             page,
@@ -405,18 +498,17 @@
             ),
         )
 
     async def _open_url(self, url: str):
         """Opens a new page and navigates to the given URL. Initialize the storgage state if provided.
 
         Parameters:
-
+        ----------
         url (str): The URL to navigate to.
         storgate_state_content (optional): The storage state with which user would like to initialize the browser.
-
         """
 
         self._current_page = None
         url = ensure_url_scheme(url)
 
         try:
             page = await self._context.new_page()
@@ -430,27 +522,28 @@
         self._current_page = page
 
     async def _set_iframe_path(self, context: Union[Page, Frame], iframe_path=None):
         """
         Sets the iframe path in the given context.
 
         Parameters:
-            context (Page | Frame): The context in which the DOM will be modified.
-            iframe_path (str, optional): The path to the iframe. Defaults to None.
+        ----------
+        context (Page | Frame): The context in which the DOM will be modified.
+        iframe_path (str, optional): The path to the iframe. Defaults to None.
         """
         await context.evaluate(
             load_js("set_iframe_path"),
             {"iframe_path": iframe_path},
         )
 
     async def _page_scroll(self, pages=3):
         """Scrolls the page down first and then up to load all contents on the page.
 
         Parameters:
-
+        ----------
         pages (int): The number of pages to scroll down.
         """
         if pages < 1:
             return
 
         if self._stealth_mode_config is None:
             delta_y = 10000
@@ -479,15 +572,15 @@
         user_session_extras: dict = None,
         headless=True,
         proxy: ProxySettings = None,
     ):
         """Starts a new browser session and set storage state (if there is any).
 
         Parameters:
-
+        ----------
         user_session_extras (optional): the JSON object that holds user session information
         headless (bool): Whether to start the browser in headless mode.
         load_media (bool): Whether to load media (images, fonts, etc.) or not.
         """
         ignored_args = [
             "--enable-automation",
             "--disable-extensions",
@@ -507,40 +600,45 @@
         )
 
     def _get_frame_context(self, iframe_path: str = None) -> Union[Frame, Page]:
         """
         Returns the frame context for the given iframe path.
 
         Parameters:
-            iframe_path (str): The path of the iframe within the frame.
+        ----------
+        iframe_path (str): The path of the iframe within the frame.
 
         Returns:
-            Frame | Page: The frame context for the given iframe path.
+        --------
+        Frame | Page: The frame context for the given iframe path.
         """
         if not iframe_path:
             return self._current_page
         iframe_path_list = iframe_path.split(".")
         frame_context = self._current_page
         for iframe_id in iframe_path_list:
             frame_context = frame_context.frame_locator(f"[tf623_id='{iframe_id}']")
         return frame_context
 
     def find_element_by_id(self, tf623_id: str, iframe_path: str = None) -> Locator:
         """
         Finds an element by its TF ID within a specified iframe.
 
-        Args:
-            tf623_id (str): The generated tf id of the element to find.
-            iframe_path (str): The path to the iframe containing the element.
+        Parameters:
+        ----------
+        tf623_id (str): The generated tf id of the element to find.
+        iframe_path (str): The path to the iframe containing the element.
 
         Returns:
-            Locator: The located element.
+        --------
+        Locator: The located element.
 
         Raises:
-            ElementNotFoundError: If the element with the specified TF ID is not found.
+        ------
+        ElementNotFoundError: If the element with the specified TF ID is not found.
         """
         try:
             element_frame_context = self._get_frame_context(iframe_path)
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
             raise ElementNotFoundError(tf623_id) from e
```

### Comparing `agentql-0.3.0/src/agentql/common/errors.py` & `agentql-0.3.1/src/agentql/common/errors.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,15 +97,24 @@
         self.row = row
         self.column = column
 
 
 class UnableToClosePopupError(BaseAgentQLError):
     def __init__(
         self,
-        message="Failed to automatically close popup. Call accessibility_tree() if you would like to analyze the popup and manually close it.",
+        message="""Failed to automatically close popup. By default, the close function will query AgentQL server and click the close button in popup with the following query:
+
+        {
+            popup_form {
+                close_btn
+            }
+        }
+
+        You could analyze the popup by invoking popup.accessibility_tree and close it manually by querying AgentQL server.
+        """,
     ):
         super().__init__(message, AGENTQL_1011_UNABLE_TO_CLOSE_POPUP_ERROR)
 
 
 class AgentQLServerError(BaseAgentQLError):
     def __init__(self, error=None, error_code=None):
         if error is None:
```

### Comparing `agentql-0.3.0/src/agentql/common/html_constants.py` & `agentql-0.3.1/src/agentql/common/html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/js_snippets/generate_accessibility_tree.js` & `agentql-0.3.1/src/agentql/common/js_snippets/generate_accessibility_tree.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,23 +1,24 @@
 ({
     currentGlobalId,
     roleTagMap,
     processIFrames = true,
+    iframePath = "",
     includeAriaHidden = false,
     nodeIdsToIgnore = [],
 }) => {
     function generate_unqie_dom_id() {
         currentGlobalId++;
         window["tf_generated_dom_id"] = currentGlobalId;
         return currentGlobalId;
     }
 
     function buildAccessibilityTree() {
         const rootNode = document.documentElement;
-        const tree = createNode(rootNode);
+        const tree = createNode(rootNode, iframePath);
         return tree;
     }
 
     function extractAttributes(node) {
         const attributes = {
             html_tag: node.nodeName.toLowerCase()
         };
@@ -38,14 +39,15 @@
         }
         const tag = node.nodeName.toLowerCase();
         if (tag == "input") {
             const type = node.getAttribute("type");
             if (type) {
                 return roleTagMap.input[type] || type;
             }
+            return "textbox";
         }
         return roleTagMap.role[tag] || "generic";
     }
 
     function getName(element) {
         // Special case: textContent for button elements
         if (element.tagName.toLowerCase() === "button") {
@@ -85,15 +87,15 @@
         return (
             style.display === "none" ||
             style.visibility === "hidden" ||
             element.hasAttribute("hidden")
         );
     }
 
-    function createNode(node) {
+    function createNode(node, currentIframePath = "") {
         const ariaHidden =
             node.getAttribute("aria-hidden") === "true" ||
             node.getAttribute("aria-hidden") === true;
         const tag = node.nodeName.toLowerCase();
         const skippedTags = [
             "script",
             "style",
@@ -105,30 +107,47 @@
             "head",
         ];
         if (skippedTags.includes(tag) || nodeIdsToIgnore.includes(node.id)) {
             return null;
         }
         let role = getRole(node);
         let name = getName(node) || "";
+        let newIframePath = currentIframePath;
 
         let children = [];
         let currentChildNodes = node.childNodes;
+
+        let nodeId = node.getAttribute("tf623_id");
+        if (!nodeId) {
+            nodeId = generate_unqie_dom_id();
+            node.setAttribute("tf623_id", nodeId);
+        }
+
+        if (currentIframePath && processIFrames) {
+            node.setAttribute("iframe_path", currentIframePath);
+        }
+
         if (node.shadowRoot) {
             const shadowRootChildren = node.shadowRoot.children;
             const childrenNodeList = Array.prototype.slice.call(shadowRootChildren);
 
             if (childrenNodeList.length > 0) {
                 currentChildNodes = Array.from(childrenNodeList);
             } else if (node.shadowRoot.textContent.trim() !== "") {
                 name = node.shadowRoot.textContent.trim();
             }
         } else if (tag == "slot") {
             currentChildNodes = node.assignedNodes();
         } else if (tag == "iframe") {
             const iframeDocument = node.contentDocument;
+            if (currentIframePath) {
+                newIframePath = currentIframePath + "." + nodeId;
+            } else {
+                newIframePath = nodeId;
+            }
             if (iframeDocument && processIFrames) {
                 if (iframeDocument.body) {
                     currentChildNodes = iframeDocument.body.childNodes;
                 } else {
                     currentChildNodes = iframeDocument.childNodes;
                 }
             } else if (node.src) {
@@ -160,45 +179,41 @@
                             role = "text";
                         }
                         name = text;
                     }
                 }
             }
             if (childNode.nodeType === Node.ELEMENT_NODE) {
-                const child = createNode(childNode);
+                const child = createNode(childNode, newIframePath);
                 if (child) {
                     children.push(child);
                 }
             }
         }
         if (children.length === 0) {
             children = undefined;
         }
 
         if (!role && !name && !children) {
             return null;
-        } else {
-            let nodeId = generate_unqie_dom_id();
-            if (!node.hasAttribute("tf623_id")) {
-                node.setAttribute("tf623_id", nodeId);
-            }
-            if (!isElementHidden(node) && (includeAriaHidden || !ariaHidden)) {
-                let node_dict = {
-                    role: role || "generic",
-                    name,
-                    attributes: extractAttributes(node),
-                };
-                if (children) {
-                    node_dict["children"] = children;
-                }
-                return node_dict;
-            } else {
-                return null;
-            }
         }
+
+        if (isElementHidden(node) || (ariaHidden && !includeAriaHidden)) {
+            return null;
+        }
+
+        let node_dict = {
+            role: role || "generic",
+            name,
+            attributes: extractAttributes(node),
+        };
+        if (children) {
+            node_dict["children"] = children;
+        }
+        return node_dict;
     }
 
     return {
         tree: buildAccessibilityTree(),
         lastUsedId: currentGlobalId,
     };
 };
```

### Comparing `agentql-0.3.0/src/agentql/common/js_snippets/set_iframe_path.js` & `agentql-0.3.1/src/agentql/common/js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/character_utils.py` & `agentql-0.3.1/src/agentql/common/syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/lexer.py` & `agentql-0.3.1/src/agentql/common/syntax/lexer.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/node.py` & `agentql-0.3.1/src/agentql/common/syntax/node.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/parser.py` & `agentql-0.3.1/src/agentql/common/syntax/parser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/source.py` & `agentql-0.3.1/src/agentql/common/syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/common/syntax/token.py` & `agentql-0.3.1/src/agentql/common/syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.3.0/src/agentql/sync_api/session.py` & `agentql-0.3.1/src/agentql/sync_api/session.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import copy
 import json
 import logging
 import os
-from typing import Callable, Generic, List, Literal
+from typing import Callable, Generic, List, Literal, Optional
 
 import requests
 
 from agentql.common.api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
 from agentql.common.errors import (
     AgentQLServerError,
     AgentQLServerTimeoutError,
@@ -22,85 +22,115 @@
 
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
 
 
 class Session(Generic[InteractiveItemTypeT, PageTypeT]):
-    """A synchronous session with a AgentQL service."""
+    """A synchronous session with a AgentQL service. It is responsible for querying and managing session-related state (like authentication)."""
 
     def __init__(self, web_driver: WebDriver[InteractiveItemTypeT, PageTypeT]):
         """Initialize the session.
 
         Parameters:
-
+        ----------
         web_driver (WebDriver): The web driver that will be used in this session.
         """
 
         self._api_key = os.getenv("AGENTQL_API_KEY")
         if not self._api_key:
             raise APIKeyError(
                 "API key not provided. Please set the environment variable 'AGENTQL_API_KEY' with your API key."
             )
         self._web_driver = web_driver
         self._event_listeners = {}
         self._check_popup = False
+        self._last_query = None
+        self._last_response = None
 
     @property
     def current_page(self) -> PageTypeT:
-        """Get the current page."""
+        """Get the current page being processed by AgentQL.
+
+        Returns:
+        -------
+        PageTypeT: A type variable representing the type of a page in a web driver session. If you did not pass a customized web driver when starting the session, then it will return [Playwright Page](https://playwright.dev/python/docs/api/class-page) object.
+        """
         return self._web_driver.get_current_page()
 
     @property
     def driver(self) -> WebDriver[InteractiveItemTypeT, PageTypeT]:
-        """Get the web driver"""
+        """Get the web driver.
+
+        Returns:
+        -------
+        WebDriver: A protocol representing the web driver. If you did not pass a customized web driver when starting the session, default PlaywrightWebDriver will be returned.
+        """
         return self._web_driver
 
+    @property
+    def last_query(self) -> Optional[str]:
+        """Get the last query."""
+        return self._last_query
+
+    @property
+    def last_response(self) -> Optional[dict]:
+        """Get the last response."""
+        return self._last_response
+
     def get_user_auth_session(self):
-        """Get the user authentication session."""
+        """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+
+        Returns:
+        --------
+        User auth session in Python dictionary format.
+        """
         return self._web_driver.get_user_auth_session()
 
     def query(
         self,
         query: str,
         timeout: int = 500,
         lazy_load_pages_count: int = 0,
         wait_for_network_idle: bool = True,
+        include_aria_hidden: bool = False,
     ) -> AQLResponseProxy[InteractiveItemTypeT]:
         """Query the web page tree for elements that match the AgentQL query.
 
         Parameters:
-
-        query (str): The query string.
-        timeout (optional): Optional timeout value for the connection with backend api service.
-        lazy_load_pages_count (optional): The number of pages to scroll down and up to load lazy loaded content.
-        wait_for_network_idle (optional): Whether to wait for the network to be idle before querying the page.
+        ----------
+        query (str): The AgentQL query in String format.
+        timeout (int) (optional): Optional timeout value for the connection with backend api service.
+        lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
+        wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
 
         Returns:
-
-        dict: AgentQL Response (Elements that match the query)
+        -------
+        AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         log.debug(f"querying {query}")
 
+        self._last_query = query
         parser = Parser(query)
         query_tree = parser.parse()
 
         self._web_driver.wait_for_page_ready_state(wait_for_network_idle)
 
-        accessibility_tree = self._web_driver.prepare_accessiblity_tree(
-            lazy_load_pages_count=lazy_load_pages_count
+        accessibility_tree = self._web_driver.prepare_accessibility_tree(
+            lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
         # Check if there is a popup in the page before sending the agentql query
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 self._handle_popup(popup_list)
 
         response = self._query(query, accessibility_tree, timeout)
+        self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
             accessibility_tree = self._web_driver.get_accessibility_tree()
 
             popup_list = self._detect_popup(accessibility_tree, popup_list)
@@ -111,32 +141,37 @@
 
     def stop(self):
         """Close the session."""
         log.debug("closing session")
         self._web_driver.stop_browser()
 
     def on(self, event: Literal["popup"], callback: Callable[[dict], None]):
-        """Emitted when there is a popup on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections."""
+        """Emitted when there is a popup (such as promotion window) on the page. The callback function will be invoked with the popup object as the argument. Passing None as the callback function will disable popup detections.
+
+        Event Data:
+        -----------
+        popups (list): The list of popups captured on the page by AgentQL Popup Detection algorithm.
+        """
         self._event_listeners[event] = callback
         if callback:
             self._check_popup = True
         else:
             self._check_popup = False
 
     def _query(self, query: str, accessibility_tree: dict, timeout: int) -> dict:
         """Make Request to AgentQL API.
 
         Parameters:
-
+        ----------
         query (str): The query string.
         accessibility_tree (dict): The accessibility tree.
         timeout (int): The timeout value for the connection with backend api service
 
         Returns:
-
+        -------
         dict: AgentQL response in json format.
         """
         try:
             page_url = self._web_driver.get_current_url()
             request_data = {
                 "query": f"{query}",
                 "accessibility_tree": accessibility_tree,
@@ -168,31 +203,32 @@
                     raise AgentQLServerError(server_error, error_code) from e
             raise AgentQLServerError(server_error, error_code) from e
 
     def _detect_popup(self, tree: dict, known_popups: List[Popup]) -> List[Popup]:
         """Detect if there is a popup in the page. If so, create a Popup object and add it to the popup dict.
 
         Parameters:
-
+        ----------
         tree (dict): The accessibility tree.
         known_popups (list): The list of known popups.
 
         Returns:
+        --------
         popups (list): The list of popups.
         """
         tree_role = tree.get("role", "")
         tree_name = tree.get("name", "")
         popup_list = []
         if tree_role == "dialog":
             popup = Popup(copy.deepcopy(tree), tree_name, self._close_popup)
 
             # Avoid adding existing popup to the dict and double handle the popup
             if known_popups:
                 for popup_object in known_popups:
-                    if popup_object.name() != popup.name():
+                    if popup_object.name != popup.name:
                         popup_list.append(popup)
             else:
                 popup_list.append(popup)
 
             return popup_list
 
         if "children" in tree:
@@ -201,25 +237,26 @@
 
         return popup_list
 
     def _handle_popup(self, popups: List[Popup]):
         """Handle the popup. If there is a popup in the list, and there is an event listener, emit the popup event by invoking the callback function.
 
         Parameters:
-
+        ----------
         popups (list): The list of popups to handle."""
         if popups and "popup" in self._event_listeners and self._event_listeners["popup"]:
             self._event_listeners["popup"](popups)
 
     def _close_popup(self, tree: dict):
-        """Close the popup.
+        """Close the popup by querying AgentQL server and click the close button.
 
         Parameters:
-
+        ----------
         popup (Popup): The popup to close.
+        query (str): The query to close the popup.
         """
         query = """
             {
                 popup {
                     close_btn
                 }
             }
```

### Comparing `agentql-0.3.0/src/agentql/sync_api/web/playwright_driver.py` & `agentql-0.3.1/src/agentql/sync_api/web/playwright_driver.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import Union
+from typing import Optional, Union
 
 from playwright.sync_api import Error, Frame, Locator, Page, StorageState, sync_playwright
 from playwright_stealth import StealthConfig, stealth_sync
 
 from agentql.async_api.web.network_monitor import PageActivityMonitor
 from agentql.common.driver_constants import RENDERER, USER_AGENT, VENDOR
 from agentql.common.driver_settings import ProxySettings, ScrollDirection, StealthModeConfig
@@ -19,15 +19,31 @@
 from agentql.common.utils import ensure_url_scheme
 from agentql.sync_api.web.web_driver import WebDriver
 
 from .web_driver import WebDriver
 
 
 class PlaywrightWebDriver(WebDriver[Locator, Page]):
+    """
+    PlaywrightWebDriver is a web driver that builds on top of [Playwright framework](https://playwright.dev/python/). It is the default web driver used by AgentQL. Users could use PlaywrightWebDriver for browser / page related activities, such as scrolling, wait for page to load, and browse in stealth mode.
+    """
+
     def __init__(self, headless=True, proxy: ProxySettings = None) -> None:
+        """
+        Construct the PlaywrightWebDriver instance.
+
+        Parameters:
+        -----------
+        headless (bool) (optional): Whether to start browser in headless mode. Headless browser will run in background while headful browser will run like a normal browser.
+        proxy (dict) (optional): The proxy setting dictionary that includes server, username, and password as key.
+
+        Returns:
+        --------
+        PlaywrightWebDriver: An instance of PlaywrightWebDriver.
+        """
         self._playwright = None
 
         self._browser = None
         """The current browser. Only use this to close the browser session in the end."""
 
         self._context = None
         """The current browser context. Use this to open a new page"""
@@ -50,52 +66,61 @@
         self._stealth_mode_config = None
 
     def locate_interactive_element(self, response_data: dict) -> Locator:
         """
         Locates an interactive element in the web page.
 
         Parameters:
+        -----------
 
         response_data (dict): The data of the interactive element from the AgentQL response.
 
         Returns:
+        --------
 
-        Locator: The interactive element.
+        [Playwright Locator](https://playwright.dev/python/docs/api/class-locator): The web element represented by Playwright's Locator object.
         """
         tf623_id = response_data.get("tf623_id")
         if not tf623_id:
             raise ElementNotFoundError("tf623_id")
         iframe_path = response_data.get("attributes", {}).get("iframe_path")
         return self.find_element_by_id(tf623_id, iframe_path)
 
     @property
     def is_headless(self) -> bool:
-        """Returns whether the browser is running in headless mode or not."""
+        """Returns whether the browser is running in headless mode or not.
+
+        Returns:
+        --------
+        bool: True if the browser is running in headless mode, False otherwise."""
         return self._headless
 
     def get_text_content(self, web_element: Locator) -> str:
         """
-        Returns the text content of the web element.
+        Gets the text content of the web element.
 
         Parameters:
+        -----------
 
-        web_element (Locator): The web element to get the text content from.
+        web_element ([Playwright Locator](https://playwright.dev/python/docs/api/class-locator)): The web element represented by Playwright's Locator object.
 
         Returns:
+        --------
 
         str: The text content of the web element.
         """
         return web_element.text_content()
 
     def start_browser(self, user_auth_session: StorageState = None):
         """
         Starts a new browser session and set user session state (if there is any).
 
         Parameters:
-        user_auth_session (optional): The user auth session state to use.
+        -----------
+        user_auth_session (optional): The user authentication session information.
         """
         self._start_browser(
             headless=self._headless, user_auth_session=user_auth_session, proxy=self._proxy
         )
 
     def stop_browser(self):
         """Closes the current browser session."""
@@ -109,123 +134,196 @@
             self._playwright.stop()
             self._playwright = None
 
     def enable_stealth_mode(
         self,
         webgl_vendor: str = VENDOR,
         webgl_renderer: str = RENDERER,
-        nav_user_agent: str | None = USER_AGENT,
+        nav_user_agent: Optional[str] = USER_AGENT,
     ):
-        """Enable the Stealth Mode and set the stealth mode configuration.
+        """Enable the stealth mode and set the stealth mode configuration.
         Ideally parameters values should match some real values to avoid detection.
         To get a realistic examples, you can use browser fingerprinting websites such as https://bot.sannysoft.com/ and https://pixelscan.net/
 
         Parameters:
-        webgl_vendor (str): The WebGL vendor to use.
-        webgl_renderer (str): The WebGL renderer to use.
-        nav_user_agent (str): The navigator user agent to use.
+        -----------
+        webgl_vendor (str) (optional):
+            The vendor of the GPU used by WebGL to render graphics, such as `Apple Inc.`. After setting this parameter, your browser will emit this vendor information.
+        webgl_renderer (str) (optional):
+            Identifies the specific GPU model or graphics rendering engine used by WebGL, such as `Apple M3`. After setting this parameter, your browser will emit this renderer information.
+        nav_user_agent (str) (optional):
+            Identifies the browser, its version, and the operating system, such as `Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/121.0.0.0 Safari/537.36`. After setting this parameter, your browser will send this user agent information to the website.
         """
         self._stealth_mode_config = StealthModeConfig(
             vendor=webgl_vendor, renderer=webgl_renderer, nav_user_agent=nav_user_agent
         )
 
-    def open_url(self, url: str):
-        """
-        Opens a new page and navigates to the given URL.
+    def open_url(self, url: str, new_page: bool = False):
+        """Open URL in the browser.
+
+        Parameters:
+        ----------
+        url (str): The URL to open.
+        new_page (bool): Whether to open the URL in a new page.
         """
         if not self._browser:
             raise NoOpenBrowserError()
-        self._open_url(url)
+
+        if new_page or self._current_page is None:
+            self._open_url(url)
+        else:
+            self._current_page.goto(url, wait_until="domcontentloaded")
 
     def get_current_url(self) -> str:
-        """Get the URL of the active page."""
+        """Get the URL of the current page being processed by AgentQL.
+
+        Returns:
+        --------
+        str: The URL of the current page.
+        """
         if not self._current_page:
             raise NoOpenPageError()
         return self._current_page.url
 
     def get_html(self) -> dict:
         """Returns the original HTML (i.e. without any AgentQL modifications) fetched from the most recently loaded page".
 
         Returns:
-
-        string: The HTML content of the web page.
+        --------
+        dict: The HTML content of the web page in Dict format.
         """
         if not self._current_page:
-            raise ValueError('No page is open. Make sure you call "open_url()" first.')
+            raise NoOpenPageError()
         return self._original_html
 
     def get_current_page(self) -> Page:
-        """Returns the current page.
+        """Returns the [Playwright page object](https://playwright.dev/python/docs/api/class-page) that represents the current page. Users could do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
-
-        Page: The current page.
+        --------
+        [Playwright Page](https://playwright.dev/python/docs/api/class-page): The current page.
         """
         if not self._current_page:
-            raise ValueError('No page is open. Make sure you call "open_url()" first.')
+            raise NoOpenPageError()
         return self._current_page
 
+    def navigate_to(self, url: str):
+        """Navigates the current page to the given URL.
+
+        Parameters:
+        ----------
+        url (str): The URL to navigate to.
+        """
+        if not self._current_page:
+            self._open_url(url)
+        else:
+            self._current_page.goto(url, wait_until="load")
+
     def open_html(self, html: str):
         """
         Opens a new page and loads the given HTML content.
+
+        Parameters:
+        -----------
+        html (str): The HTML content to load in the page.
         """
         if not self._browser:
             raise NoOpenBrowserError()
         self._current_page = self._context.new_page()
         self._current_tf_id = 0
         self._current_page.set_content(html)
 
-    def prepare_accessiblity_tree(self, lazy_load_pages_count: int = 3) -> dict:
+    def prepare_accessibility_tree(
+        self, lazy_load_pages_count: int = 3, include_aria_hidden: bool = False
+    ) -> dict:
         """Prepare the AT by modifing the dom. It will return the accessibility tree after waiting for page to load and dom modification.
 
         Parameters:
-        lazy_load_pages_count: The number of times to scroll down and up the page.
+        -----------
+        lazy_load_pages_count (int): The number of times to scroll down and up the page.
+        include_aria_hidden (bool): Whether to include elements with aria-hidden attribute in the accessibility tree.
 
         Returns:
+        --------
         dict: AT of the page
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         self._original_html = self._current_page.content()
         self._page_scroll(pages=lazy_load_pages_count)
 
         accessibility_tree = None
         try:
-            accessibility_tree = self._get_page_accessibility_tree(self._current_page)
+            accessibility_tree = self._get_page_accessibility_tree(
+                self._current_page, include_aria_hidden=include_aria_hidden
+            )
             self._process_iframes(accessibility_tree)
             self._post_process_accessibility_tree(accessibility_tree)
 
         except Exception as e:
             raise AccessibilityTreeError() from e
 
         return accessibility_tree
 
     def get_accessibility_tree(self) -> dict:
         """Returns the up-to-date accessibility tree of the page.
 
         Returns:
-        dict: The accessibility tree of the page.
+        --------
+        dict: The accessibility tree of the page in Dict format.
         """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         try:
             accessibility_tree = self._get_page_accessibility_tree(self._current_page)
             self._process_iframes(accessibility_tree)
         except Exception as e:
             raise AccessibilityTreeError() from e
 
         return accessibility_tree
 
     def get_user_auth_session(self) -> StorageState:
-        """Returns the user auth session state of the browser."""
+        """
+        **NOT RECOMMENDED** (Use session.get_user_auth_session() instead)
+
+        Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
+
+        Returns:
+        --------
+        dict: User auth session in Python dictionary format.
+        """
         if not self._browser:
             raise NoOpenBrowserError()
         return self._context.storage_state()
 
     def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
-        """Wait for the page to reach the "Page Ready" or stable state."""
+        """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
+
+        Usage:
+        -----
+        ```py
+        session = agentql.start_async_session(YOUTUBE_URL)
+
+        # Scroll to bottom to trigger comments loading
+        await session.driver.scroll_to_bottom()
+
+        # Wait for comments to load before making a query
+        await session.driver.wait_for_page_ready_state()
+        await session.query(QUERY)
+        ```
+
+        Parameters:
+        -----------
+        wait_for_network_idle (bool) (optional): This acts as a switch to determine whether to use default chekcing mechanism. If set to `False`, this method will only check for whether page has emitted `load` [event](https://developer.mozilla.org/en-US/docs/Web/API/Window/load_event) and provide a less costly checking mechanism for fast-loading pages.
+        """
+        if not self._current_page:
+            raise NoOpenPageError()
+
         if not self._page_monitor:
             self._page_monitor = PageActivityMonitor()
         else:
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
@@ -234,35 +332,36 @@
         # Wait for the page to reach the "Page Ready" state
         self._determine_load_state(self._page_monitor, wait_for_network_idle)
 
         # Remove the event listeners to prevent overwhelming the async event loop
         self._remove_page_event_listeners()
 
     def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
-        """Scrolls the page up or down.
+        """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
         Parameters:
-        scroll_direction (ScrollDirection): The direction to scroll the page.
-        pixels (int): The number of pixels to scroll.
+        -----------
+        scroll_direction (ScrollDirection): An enumeration class that represents the direction in which a scroll action can occur. Currently, it has `UP` and `DOWN` member. You could import this class with `from agentql.common.driver_settings import ScrollDirection`.
+        pixels (int) (optional): The number of pixels to scroll. 720 by default.
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         delta_y = pixels if scroll_direction == ScrollDirection.DOWN else -pixels
         self._current_page.mouse.wheel(delta_x=0, delta_y=delta_y)
 
     def scroll_to_bottom(self):
-        """Scrolls the page to the bottom."""
+        """Scrolls to the bottom of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         self._current_page.evaluate(load_js("scroll_to_bottom"))
 
     def scroll_to_top(self):
-        """Scrolls the page to the top."""
+        """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         self._current_page.evaluate(load_js("scroll_to_top"))
 
     def _post_process_accessibility_tree(self, accessibility_tree: dict):
         """Post-process the accessibility tree by removing node's attributes that are Null."""
@@ -279,20 +378,22 @@
         iframe_path: str = "",
         frame: Frame = None,
     ):
         """
         Recursively retrieves the accessibility trees for all iframes in a page or frame.
 
         Parameters:
-            iframe_path (str): The path of the iframe in the frame hierarchy.
-            frame (Frame): The frame object representing the current frame.
-            page_accessibility_tree (dict): The accessibility tree of the page.
+        ----------
+        iframe_path (str): The path of the iframe in the frame hierarchy.
+        frame (Frame): The frame object representing the current frame.
+        page_accessibility_tree (dict): The accessibility tree of the page.
 
         Returns:
-            None
+        --------
+        None
         """
         if frame is None:
             iframes = self._current_page.query_selector_all("iframe")
         else:
             frame = frame.content_frame()
             if not frame:
                 return
@@ -314,44 +415,54 @@
 
             self._process_iframes(
                 iframe_path=iframe_path_to_send,
                 frame=iframe,
                 page_accessibility_tree=page_accessibility_tree,
             )
 
-    def _get_page_accessibility_tree(self, context: Union[Page, Frame]) -> dict:
+    def _get_page_accessibility_tree(
+        self, context: Union[Page, Frame], include_aria_hidden: bool = False
+    ) -> dict:
         """
         Retrieves the accessibility tree for the given page.
 
+        Parameters:
+        ----------
+        context (Page | Frame): The context in which to retrieve the accessibility tree.
+
         Returns:
-            dict: The accessibility tree for the page.
+        --------
+        dict: The accessibility tree for the page.
         """
         result = context.evaluate(
             load_js("generate_accessibility_tree"),
             {
                 "currentGlobalId": self._current_tf_id,
                 "roleTagMap": HTML_ROLE_MAPPING,
                 "processIFrames": False,
+                "includeAriaHidden": include_aria_hidden,
             },
         )
 
         self._current_tf_id = result.get("lastUsedId")
 
         return result.get("tree")
 
     def _get_frame_accessibility_tree(self, frame: Frame, iframe_path) -> dict:
         """
         Retrieves the accessibility tree for a given frame.
 
         Parameters:
-            frame (Frame): The frame for which to retrieve the accessibility tree.
-            iframe_path: The path of the iframe within the frame.
+        ----------
+        frame (Frame): The frame for which to retrieve the accessibility tree.
+        iframe_path: The path of the iframe within the frame.
 
         Returns:
-            dict: The accessibility tree for the frame.
+        --------
+        dict: The accessibility tree for the frame.
         """
         frame_context = frame.content_frame()
 
         if not frame_context:
             return {}
 
         self._set_iframe_path(context=frame_context, iframe_path=iframe_path)
@@ -362,20 +473,22 @@
     def _merge_iframe_tree_into_page(
         self, iframe_id, accessibility_tree: dict, iframe_accessibility_tree: dict
     ):
         """
         Stitches the iframe accessibility tree with the page accessibility tree.
 
         Parameters:
-            iframe_id (str): The ID of the iframe.
-            accessibility_tree (dict): The accessibility tree of the page.
-            iframe_accessibility_tree (dict): The accessibility tree of the iframe.
+        ----------
+        iframe_id (str): The ID of the iframe.
+        accessibility_tree (dict): The accessibility tree of the page.
+        iframe_accessibility_tree (dict): The accessibility tree of the iframe.
 
         Returns:
-            None
+        --------
+        None
         """
         children = accessibility_tree.get("children", [])
         if children is None:
             return
         for child in children:
             attributes = child.get("attributes", {})
             if "tf623_id" in attributes and attributes["tf623_id"] == iframe_id:
@@ -385,14 +498,15 @@
                 break
             self._merge_iframe_tree_into_page(iframe_id, child, iframe_accessibility_tree)
 
     def _apply_stealth_mode_to_page(self, page: Page):
         """Applies stealth mode to the given page.
 
         Parameters:
+        ----------
         page (Page): The page to which stealth mode will be applied.
         """
         # Only mask User Agent in headless mode to avoid detection for headless browsers
         mask_user_agent = self._headless
 
         stealth_sync(
             page,
@@ -405,18 +519,17 @@
             ),
         )
 
     def _open_url(self, url: str):
         """Opens a new page and navigates to the given URL. Initialize the storgage state if provided.
 
         Parameters:
-
+        ----------
         url (str): The URL to navigate to.
         storgate_state_content (optional): The storage state with which user would like to initialize the browser.
-
         """
 
         self._current_page = None
         url = ensure_url_scheme(url)
 
         try:
             page = self._context.new_page()
@@ -430,27 +543,28 @@
         self._current_page = page
 
     def _set_iframe_path(self, context: Union[Page, Frame], iframe_path=None):
         """
         Sets the iframe path in the given context.
 
         Parameters:
-            context (Page | Frame): The context in which the DOM will be modified.
-            iframe_path (str, optional): The path to the iframe. Defaults to None.
+        ----------
+        context (Page | Frame): The context in which the DOM will be modified.
+        iframe_path (str, optional): The path to the iframe. Defaults to None.
         """
         context.evaluate(
             load_js("set_iframe_path"),
             {"iframe_path": iframe_path},
         )
 
     def _page_scroll(self, pages=3):
         """Scrolls the page down first and then up to load all contents on the page.
 
         Parameters:
-
+        ----------
         pages (int): The number of pages to scroll down.
         """
         if pages < 1:
             return
 
         if self._stealth_mode_config is None:
             delta_y = 10000
@@ -478,15 +592,15 @@
         user_auth_session=None,
         headless=True,
         proxy: ProxySettings = None,
     ):
         """Starts a new browser session and set storage state (if there is any).
 
         Parameters:
-
+        ----------
         user_session_extras (optional): the JSON object that holds user session information
         headless (bool): Whether to start the browser in headless mode.
         load_media (bool): Whether to load media (images, fonts, etc.) or not.
         """
         ignored_args = ["--enable-automation", "--disable-extensions"]
         args = [
             "--no-sandbox",
@@ -504,40 +618,45 @@
         )
 
     def _get_frame_context(self, iframe_path: str = None) -> Union[Frame, Page]:
         """
         Returns the frame context for the given iframe path.
 
         Parameters:
-            iframe_path (str): The path of the iframe within the frame.
+        ----------
+        iframe_path (str): The path of the iframe within the frame.
 
         Returns:
-            Frame | Page: The frame context for the given iframe path.
+        --------
+        Frame | Page: The frame context for the given iframe path.
         """
         if not iframe_path:
             return self._current_page
         iframe_path_list = iframe_path.split(".")
         frame_context = self._current_page
         for iframe_id in iframe_path_list:
             frame_context = frame_context.frame_locator(f"[tf623_id='{iframe_id}']")
         return frame_context
 
     def find_element_by_id(self, tf623_id: str, iframe_path: str = None) -> Locator:
         """
         Finds an element by its TF ID within a specified iframe.
 
-        Args:
-            tf623_id (str): The generated tf id of the element to find.
-            iframe_path (str): The path to the iframe containing the element.
+        Parameters:
+        ----------
+        tf623_id (str): The generated tf id of the element to find.
+        iframe_path (str): The path to the iframe containing the element.
 
         Returns:
-            Locator: The located element.
+        --------
+        Locator: The located element.
 
         Raises:
-            ElementNotFoundError: If the element with the specified TF ID is not found.
+        ------
+        ElementNotFoundError: If the element with the specified TF ID is not found.
         """
         try:
             element_frame_context = self._get_frame_context(iframe_path)
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
             raise ElementNotFoundError(tf623_id) from e
```

### Comparing `agentql-0.3.0/PKG-INFO` & `agentql-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.3.0
+Version: 0.3.1
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

