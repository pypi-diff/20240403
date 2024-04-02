# Comparing `tmp/deltachat-rpc-client-1.136.6.tar.gz` & `tmp/deltachat-rpc-client-1.137.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deltachat-rpc-client-1.136.6.tar", last modified: Tue Mar 19 04:01:11 2024, max compression
+gzip compressed data, was "deltachat-rpc-client-1.137.0.tar", last modified: Tue Apr  2 22:09:47 2024, max compression
```

## Comparing `deltachat-rpc-client-1.136.6.tar` & `deltachat-rpc-client-1.137.0.tar`

### file list

```diff
@@ -1,36 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.303972 deltachat-rpc-client-1.136.6/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-19 04:01:11.303972 deltachat-rpc-client-1.136.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.299972 deltachat-rpc-client-1.136.6/examples/
--rwxr-xr-x   0 runner    (1001) docker     (127)      538 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/examples/echobot.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2145 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/examples/echobot_advanced.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1949 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/examples/echobot_no_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 04:01:11.303972 deltachat-rpc-client-1.136.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.299972 deltachat-rpc-client-1.136.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.299972 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/deltachat.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/message.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/pytestplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.303972 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-19 04:01:11.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-19 04:01:11.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 04:01:11.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-19 04:01:11.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-19 04:01:11.000000 deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 04:01:11.303972 deltachat-rpc-client-1.136.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/tests/test_securejoin.py
--rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/tests/test_something.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/tests/test_webxdc.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-19 04:01:03.000000 deltachat-rpc-client-1.136.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:09:47.655156 deltachat-rpc-client-1.137.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-02 22:09:47.655156 deltachat-rpc-client-1.137.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:09:47.655156 deltachat-rpc-client-1.137.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:09:47.651157 deltachat-rpc-client-1.137.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:09:47.651157 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12417 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/deltachat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/pytestplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:09:47.655156 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-02 22:09:47.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-02 22:09:47.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:09:47.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 22:09:47.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-02 22:09:47.000000 deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:09:47.655156 deltachat-rpc-client-1.137.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/tests/test_securejoin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/tests/test_something.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-02 22:09:39.000000 deltachat-rpc-client-1.137.0/tests/test_webxdc.py
```

### Comparing `deltachat-rpc-client-1.136.6/LICENSE` & `deltachat-rpc-client-1.137.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/PKG-INFO` & `deltachat-rpc-client-1.137.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.136.6
+Version: 1.137.0
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat-rpc-client-1.136.6/README.md` & `deltachat-rpc-client-1.137.0/README.md`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/pyproject.toml` & `deltachat-rpc-client-1.137.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=45"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deltachat-rpc-client"
+version = "1.137.0"
 description = "Python client for Delta Chat core JSON-RPC interface"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: POSIX :: Linux",
     "Operating System :: MacOS :: MacOS X",
@@ -15,30 +16,24 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Communications :: Chat",
     "Topic :: Communications :: Email"
 ]
-dynamic = [
-    "version"
-]
 readme = "README.md"
 
 [tool.setuptools.package-data]
 deltachat_rpc_client = [
     "py.typed"
 ]
 
 [project.entry-points.pytest11]
 "deltachat_rpc_client.pytestplugin" = "deltachat_rpc_client.pytestplugin"
 
-[tool.setuptools_scm]
-root = ".."
-
 [tool.black]
 line-length = 120
 
 [tool.ruff]
 select = [
   "E", "W", # pycodestyle
   "F", # Pyflakes
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/__init__.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/_utils.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -164,7 +164,37 @@
 
     if text.startswith("group left by "):
         addr = extract_addr(text[13:])
         if addr:
             return "removed", addr, addr
 
     return None
+
+
+class futuremethod:  # noqa: N801
+    """Decorator for async methods."""
+
+    def __init__(self, func):
+        self._func = func
+
+    def __get__(self, instance, owner=None):
+        if instance is None:
+            return self
+
+        def future(*args):
+            generator = self._func(instance, *args)
+            res = next(generator)
+
+            def f():
+                try:
+                    generator.send(res())
+                except StopIteration as e:
+                    return e.value
+
+            return f
+
+        def wrapper(*args):
+            f = future(*args)
+            return f()
+
+        wrapper.future = future
+        return wrapper
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/account.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 from warnings import warn
 
-from ._utils import AttrDict
+from ._utils import AttrDict, futuremethod
 from .chat import Chat
 from .const import ChatlistFlag, ContactFlag, EventType, SpecialContactId
 from .contact import Contact
 from .message import Message
 
 if TYPE_CHECKING:
     from .deltachat import DeltaChat
@@ -72,17 +72,18 @@
         """
         self.set_config("selfavatar", img_path)
 
     def get_avatar(self) -> Optional[str]:
         """Get self avatar."""
         return self.get_config("selfavatar")
 
-    def configure(self) -> None:
+    @futuremethod
+    def configure(self):
         """Configure an account."""
-        self._rpc.configure(self.id)
+        yield self._rpc.configure.future(self.id)
 
     def create_contact(self, obj: Union[int, str, Contact], name: Optional[str] = None) -> Contact:
         """Create a new Contact or return an existing one.
 
         Calling this method will always result in the same
         underlying contact id.  If there already is a Contact
         with that e-mail address, it is unblocked and its display
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/chat.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/chat.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/client.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/client.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/const.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/const.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/contact.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/contact.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/deltachat.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/deltachat.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/events.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/events.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/message.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/message.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/pytestplugin.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/pytestplugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import random
 from typing import AsyncGenerator, List, Optional
 
 import pytest
 
 from . import Account, AttrDict, Bot, Client, DeltaChat, EventType, Message
+from ._utils import futuremethod
 from .rpc import Rpc
 
 
 def get_temp_credentials() -> dict:
     domain = os.getenv("CHATMAIL_DOMAIN")
     username = "ci-" + "".join(random.choice("2345789acdefghjkmnpqrstuvwxyz") for i in range(6))
     password = f"{username}${username}"
@@ -33,37 +34,40 @@
         credentials = get_temp_credentials()
         account = self.get_unconfigured_account()
         account.set_config("addr", credentials["email"])
         account.set_config("mail_pw", credentials["password"])
         assert not account.is_configured()
         return account
 
-    def new_configured_account(self) -> Account:
+    @futuremethod
+    def new_configured_account(self):
         account = self.new_preconfigured_account()
-        account.configure()
+        yield account.configure.future()
         assert account.is_configured()
         return account
 
     def new_configured_bot(self) -> Bot:
         credentials = get_temp_credentials()
         bot = self.get_unconfigured_bot()
         bot.configure(credentials["email"], credentials["password"])
         return bot
 
-    def get_online_account(self) -> Account:
-        account = self.new_configured_account()
+    @futuremethod
+    def get_online_account(self):
+        account = yield self.new_configured_account.future()
         account.start_io()
         while True:
             event = account.wait_for_event()
             if event.kind == EventType.IMAP_INBOX_IDLE:
                 break
         return account
 
     def get_online_accounts(self, num: int) -> List[Account]:
-        return [self.get_online_account() for _ in range(num)]
+        futures = [self.get_online_account.future() for _ in range(num)]
+        return [f() for f in futures]
 
     def resetup_account(self, ac: Account) -> Account:
         """Resetup account from scratch, losing the encryption key."""
         ac.stop_io()
         ac_clone = self.get_unconfigured_account()
         for i in ["addr", "mail_pw"]:
             ac_clone.set_config(i, ac.get_config(i))
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client/rpc.py` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client/rpc.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,56 @@
 from typing import Any, Dict, Iterator, Optional
 
 
 class JsonRpcError(Exception):
     pass
 
 
+class RpcFuture:
+    def __init__(self, rpc: "Rpc", request_id: int, event: Event):
+        self.rpc = rpc
+        self.request_id = request_id
+        self.event = event
+
+    def __call__(self):
+        self.event.wait()
+        response = self.rpc.request_results.pop(self.request_id)
+        if "error" in response:
+            raise JsonRpcError(response["error"])
+        if "result" in response:
+            return response["result"]
+        return None
+
+
+class RpcMethod:
+    def __init__(self, rpc: "Rpc", name: str):
+        self.rpc = rpc
+        self.name = name
+
+    def __call__(self, *args) -> Any:
+        """Synchronously calls JSON-RPC method."""
+        future = self.future(*args)
+        return future()
+
+    def future(self, *args) -> Any:
+        """Asynchronously calls JSON-RPC method."""
+        request_id = next(self.rpc.id_iterator)
+        request = {
+            "jsonrpc": "2.0",
+            "method": self.name,
+            "params": args,
+            "id": request_id,
+        }
+        event = Event()
+        self.rpc.request_events[request_id] = event
+        self.rpc.request_queue.put(request)
+
+        return RpcFuture(self.rpc, request_id, event)
+
+
 class Rpc:
     def __init__(self, accounts_dir: Optional[str] = None, **kwargs):
         """The given arguments will be passed to subprocess.Popen()"""
         if accounts_dir:
             kwargs["env"] = {
                 **kwargs.get("env", os.environ),
                 "DC_ACCOUNTS_PATH": str(accounts_dir),
@@ -141,28 +183,8 @@
 
     def wait_for_event(self, account_id: int) -> Optional[dict]:
         """Waits for the next event from the given account and returns it."""
         queue = self.get_queue(account_id)
         return queue.get()
 
     def __getattr__(self, attr: str):
-        def method(*args) -> Any:
-            request_id = next(self.id_iterator)
-            request = {
-                "jsonrpc": "2.0",
-                "method": attr,
-                "params": args,
-                "id": request_id,
-            }
-            event = Event()
-            self.request_events[request_id] = event
-            self.request_queue.put(request)
-            event.wait()
-
-            response = self.request_results.pop(request_id)
-            if "error" in response:
-                raise JsonRpcError(response["error"])
-            if "result" in response:
-                return response["result"]
-            return None
-
-        return method
+        return RpcMethod(self, attr)
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/PKG-INFO` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltachat-rpc-client
-Version: 1.136.6
+Version: 1.137.0
 Summary: Python client for Delta Chat core JSON-RPC interface
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
```

### Comparing `deltachat-rpc-client-1.136.6/src/deltachat_rpc_client.egg-info/SOURCES.txt` & `deltachat-rpc-client-1.137.0/src/deltachat_rpc_client.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-tox.ini
-examples/echobot.py
-examples/echobot_advanced.py
-examples/echobot_no_hooks.py
 src/deltachat_rpc_client/__init__.py
 src/deltachat_rpc_client/_utils.py
 src/deltachat_rpc_client/account.py
 src/deltachat_rpc_client/chat.py
 src/deltachat_rpc_client/client.py
 src/deltachat_rpc_client/const.py
 src/deltachat_rpc_client/contact.py
```

### Comparing `deltachat-rpc-client-1.136.6/tests/test_securejoin.py` & `deltachat-rpc-client-1.137.0/tests/test_securejoin.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/tests/test_something.py` & `deltachat-rpc-client-1.137.0/tests/test_something.py`

 * *Files identical despite different names*

### Comparing `deltachat-rpc-client-1.136.6/tests/test_webxdc.py` & `deltachat-rpc-client-1.137.0/tests/test_webxdc.py`

 * *Files identical despite different names*

