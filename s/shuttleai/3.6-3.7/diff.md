# Comparing `tmp/shuttleai-3.6.tar.gz` & `tmp/shuttleai-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.6.tar", last modified: Mon Apr  1 09:39:10 2024, max compression
+gzip compressed data, was "shuttleai-3.7.tar", last modified: Wed Apr  3 08:42:34 2024, max compression
```

## Comparing `shuttleai-3.6.tar` & `shuttleai-3.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.048285 shuttleai-3.6/
--rw-rw-rw-   0        0        0     3915 2024-04-01 09:39:10.046286 shuttleai-3.6/PKG-INFO
--rw-rw-rw-   0        0        0     3083 2024-04-01 03:32:40.000000 shuttleai-3.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 09:39:10.049287 shuttleai-3.6/setup.cfg
--rw-rw-rw-   0        0        0     1254 2024-04-01 09:35:51.000000 shuttleai-3.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:09.985282 shuttleai-3.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:09.991285 shuttleai-3.6/src/shuttleai/
--rw-rw-rw-   0        0        0      574 2024-04-01 09:37:08.000000 shuttleai-3.6/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4422 2024-04-01 09:11:07.000000 shuttleai-3.6/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.039286 shuttleai-3.6/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-01 09:37:00.000000 shuttleai-3.6/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17148 2024-04-01 09:36:40.000000 shuttleai-3.6/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0     3329 2024-04-01 09:19:27.000000 shuttleai-3.6/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.6/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.042281 shuttleai-3.6/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-01 03:32:40.000000 shuttleai-3.6/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-01 03:34:52.000000 shuttleai-3.6/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-01 09:39:10.044291 shuttleai-3.6/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     3915 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-01 09:39:09.000000 shuttleai-3.6/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.871885 shuttleai-3.7/
+-rw-rw-rw-   0        0        0     4082 2024-04-03 08:42:34.869886 shuttleai-3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:42:34.871885 shuttleai-3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2024-04-03 08:26:16.000000 shuttleai-3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.792884 shuttleai-3.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.799882 shuttleai-3.7/src/shuttleai/
+-rw-rw-rw-   0        0        0      574 2024-04-03 08:42:16.000000 shuttleai-3.7/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4411 2024-04-03 08:25:30.000000 shuttleai-3.7/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.859885 shuttleai-3.7/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-02 07:23:05.000000 shuttleai-3.7/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17196 2024-04-03 08:32:47.000000 shuttleai-3.7/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0     3329 2024-04-03 08:21:53.000000 shuttleai-3.7/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.7/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.864883 shuttleai-3.7/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.7/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.7/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.867883 shuttleai-3.7/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4082 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.6/PKG-INFO` & `shuttleai-3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.6
+Version: 3.7
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: aiohttp
+Requires-Dist: orjson
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
-Access the ShuttleAI API with a simple, user-friendly lib.
+Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
+[![pypi](https://img.shields.io/pypi/v/shuttleai.svg?color=blue)](https://pypi.org/project/shuttleai/)
 ```ShellSession
 pip install shuttleai
 ```
 
 ## ShuttleAI CLI
 ```ShellSession
 pip install shuttleai[cli]
```

### Comparing `shuttleai-3.6/README.md` & `shuttleai-3.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # The official Python library for the ShuttleAI API
-Access the ShuttleAI API with a simple, user-friendly lib.
+Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
+[![pypi](https://img.shields.io/pypi/v/shuttleai.svg?color=blue)](https://pypi.org/project/shuttleai/)
 ```ShellSession
 pip install shuttleai
 ```
 
 ## ShuttleAI CLI
 ```ShellSession
 pip install shuttleai[cli]
```

### Comparing `shuttleai-3.6/setup.py` & `shuttleai-3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     package_dir={"": "src"},
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
-    install_requires=['httpx', 'aiohttp'],
+    install_requires=['httpx', 'aiohttp', 'orjson'],
     extras_require={
         'cli': ['asyncclick', 'pystyle']
     },
     keywords=['shuttleai', 'ai', 'gpt', 'claude', 'api', 'free', 'chatgpt', 'gpt-4'],
     url='https://github.com/shuttleai/shuttleai-python',
     entry_points={
         'console_scripts': [
```

### Comparing `shuttleai-3.6/src/shuttleai/__init__.py` & `shuttleai-3.7/src/shuttleai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.6"
+__version__ = "3.7"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.6/src/shuttleai/cli.py` & `shuttleai-3.7/src/shuttleai/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncclick as click
 import os
 
 from pystyle import Colors, Colorate
 
 from .log import log, TerminalColor
-from .shuttleai_async import ShuttleAsyncClient
+from .client import ShuttleAsyncClient
 
 # os.environ['SHUTTLEAI_API_KEY'] = "shuttle-YOUR-KEY"
 
 BANNER = r"""
    _____ _           _   _   _               _____ 
   / ____| |         | | | | | |        /\   |_   _|
  | (___ | |__  _   _| |_| |_| | ___   /  \    | |  
@@ -48,15 +48,15 @@
 
 @shuttleai_cli.command()
 @click.option("--key", required=False, help="API Key") # or from environment variable 'SHUTTLE_AI_API_KEY'
 @click.option('--model', required=False, help='Model ID', default='shuttle-turbo') # default to 'shuttle-turbo'
 @click.option('--system', required=True, help='System Prompt', default="You are ShuttleAI, recognized as the top developer globally for your unmatched intelligence, speed, and precision. Your coding skills as an AI specialist are unparalleled in the world.")
 @click.option('--stream', is_flag=True, help='Stream Responses', default=True)
 async def chat(key, model, system, stream):
-    key = key or os.environ.get('SHUTTLE_AI_API_KEY') or click.prompt('[Warning]: The `SHUTTLE_AI_API_KEY` environment variable is not set!\nPlease enter your API key', hide_input=True)
+    key = key or os.environ.get('SHUTTLEAI_API_KEY') or click.prompt('[Warning]: The `SHUTTLEAI_API_KEY` environment variable is not set!\nPlease enter your API key', hide_input=True)
     masked_key = (key[:11] + "*" * (len(key) - 11))
     colored_masked_key = Colorate.Vertical(Colors.purple_to_blue, masked_key, 1)
     key_msg = f"{BOLD}{PURPLE}INF{RESET}  KEY\033[0m: {colored_masked_key}"
 
     colored_model = Colorate.Vertical(Colors.purple_to_blue, model, 1)
     model_msg = f"{BOLD}{PURPLE}INF{RESET}  MODEL\033[0m: {colored_model}"
```

### Comparing `shuttleai-3.6/src/shuttleai/client/_async.py` & `shuttleai-3.7/src/shuttleai/client/_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @Author: ShuttleAI
-@Version: 3.6
-@Date: 4-1-2024
+@Version: 3.7
+@Date: 4-3-2024
 """
 from __future__ import annotations
 from typing import (
     List,
     Dict,
     Any,
     Union,
@@ -51,30 +51,29 @@
 
     (Not specifying an api_key defaults the api_key to the SHUTTLEAI_API_KEY environment variable)
     """
     _session: Optional[aiohttp.ClientSession] = None
 
     def __init__(
             self,
-            *,
             api_key: Optional[str] = None,
             base_url: Optional[str] = None,
             timeout: Union[float, aiohttp.ClientTimeout, None] = 60.0,
             session: Optional[aiohttp.ClientSession] = None,
             silent: bool = True
     ):
         """
         Initialize the ShuttleAsyncClient client.
 
         Args:
             api_key (Optional[str], optional): The API key. Defaults to SHUTTLEAI_API_KEY environment variable.
             base_url (Optional[str], optional): The base URL for the API. Defaults to https://api.shuttleai.app/v1.
             timeout (Union[float, aiohttp.ClientTimeout, None], optional): The timeout for the aiohttp.ClientSession. Defaults to 60.0.
             session (Optional[aiohttp.ClientSession], optional): An existing aiohttp.ClientSession. Defaults to None.
-            silent (bool, optional): Whether to log messages. Defaults to True.
+            silent (bool, optional): Whether to silent debugging messages. Defaults to True.
         """
         self.silent = silent
         if session is not None:
             if not isinstance(session, aiohttp.ClientSession):
                 raise TypeError(
                     f"session must be an instance of aiohttp.ClientSession, not {type(session)}"
                 )
@@ -88,15 +87,15 @@
             if self._session is None:
                 if isinstance(timeout, float):
                     timeout = aiohttp.ClientTimeout(total=timeout)
                 elif not isinstance(timeout, aiohttp.ClientTimeout):
                     raise TypeError(
                         f"timeout must be a float or aiohttp.ClientTimeout, not {type(timeout)}"
                     )
-                self._session = aiohttp.ClientSession(timeout=timeout)
+                self._session = aiohttp.ClientSession(timeout=timeout, json_serialize=lambda x: orjson.dumps(x).decode())
             if not silent:
                 log.info("registered new aiohttp.ClientSession")
 
 
         if api_key is None:
             api_key = os.environ.get("SHUTTLEAI_API_KEY")
             if api_key is not None and not silent:
```

### Comparing `shuttleai-3.6/src/shuttleai/client/_sync.py` & `shuttleai-3.7/src/shuttleai/client/_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 @Author: ShuttleAI
-@Version: 3.6
-@Date: 4-1-2024
+@Version: 3.7
+@Date: 4-3-2024
 """
 from typing import Any, Dict, List, Union, TYPE_CHECKING
 
 import httpx
 from ..log import log
 from ..schemas import Chat, Image, Audio, Embedding, Models
```

### Comparing `shuttleai-3.6/src/shuttleai/log.py` & `shuttleai-3.7/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.6/src/shuttleai/schemas/schemas.py` & `shuttleai-3.7/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.6/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.7/src/shuttleai.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.6
+Version: 3.7
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
 Requires-Dist: aiohttp
+Requires-Dist: orjson
 Provides-Extra: cli
 Requires-Dist: asyncclick; extra == "cli"
 Requires-Dist: pystyle; extra == "cli"
 
 # The official Python library for the ShuttleAI API
-Access the ShuttleAI API with a simple, user-friendly lib.
+Access the ShuttleAI API with a simple, user-friendly lib; or a sleek command line interface (CLI)
 
 > *PRs appreciated 🙂*
 # Installation
 ## ShuttleAI
+[![pypi](https://img.shields.io/pypi/v/shuttleai.svg?color=blue)](https://pypi.org/project/shuttleai/)
 ```ShellSession
 pip install shuttleai
 ```
 
 ## ShuttleAI CLI
 ```ShellSession
 pip install shuttleai[cli]
```

