# Comparing `tmp/bot_station_client-0.0.3.tar.gz` & `tmp/bot_station_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station_client-0.0.3.tar", last modified: Mon Mar 25 19:51:27 2024, max compression
+gzip compressed data, was "bot_station_client-0.0.4.tar", last modified: Wed Apr  3 19:45:08 2024, max compression
```

## Comparing `bot_station_client-0.0.3.tar` & `bot_station_client-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-03-25 19:51:27.160396 bot_station_client-0.0.3/
--rw-r--r--   0 mrmx       (501) staff       (20)     1070 2024-03-22 14:52:19.000000 bot_station_client-0.0.3/LICENSE
--rw-r--r--   0 mrmx       (501) staff       (20)      408 2024-03-25 19:51:27.159355 bot_station_client-0.0.3/PKG-INFO
--rw-r--r--   0 mrmx       (501) staff       (20)       24 2024-03-22 14:41:22.000000 bot_station_client-0.0.3/README.md
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-03-25 19:51:27.155238 bot_station_client-0.0.3/bot_station_client/
--rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 14:38:45.000000 bot_station_client-0.0.3/bot_station_client/__init__.py
--rw-r--r--   0 mrmx       (501) staff       (20)     2754 2024-03-25 19:40:32.000000 bot_station_client-0.0.3/bot_station_client/client.py
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-03-25 19:51:27.157509 bot_station_client-0.0.3/bot_station_client/model/
--rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 15:15:24.000000 bot_station_client-0.0.3/bot_station_client/model/__init__.py
--rw-r--r--   0 mrmx       (501) staff       (20)      100 2024-03-22 15:23:15.000000 bot_station_client-0.0.3/bot_station_client/model/config.py
-drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-03-25 19:51:27.158475 bot_station_client-0.0.3/bot_station_client.egg-info/
--rw-r--r--   0 mrmx       (501) staff       (20)      408 2024-03-25 19:51:27.000000 bot_station_client-0.0.3/bot_station_client.egg-info/PKG-INFO
--rw-r--r--   0 mrmx       (501) staff       (20)      367 2024-03-25 19:51:27.000000 bot_station_client-0.0.3/bot_station_client.egg-info/SOURCES.txt
--rw-r--r--   0 mrmx       (501) staff       (20)        1 2024-03-25 19:51:27.000000 bot_station_client-0.0.3/bot_station_client.egg-info/dependency_links.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       17 2024-03-25 19:51:27.000000 bot_station_client-0.0.3/bot_station_client.egg-info/requires.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       19 2024-03-25 19:51:27.000000 bot_station_client-0.0.3/bot_station_client.egg-info/top_level.txt
--rw-r--r--   0 mrmx       (501) staff       (20)       38 2024-03-25 19:51:27.160589 bot_station_client-0.0.3/setup.cfg
--rw-r--r--   0 mrmx       (501) staff       (20)      780 2024-03-25 19:51:10.000000 bot_station_client-0.0.3/setup.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 19:45:08.428226 bot_station_client-0.0.4/
+-rw-r--r--   0 mrmx       (501) staff       (20)     1070 2024-03-22 14:52:19.000000 bot_station_client-0.0.4/LICENSE
+-rw-r--r--   0 mrmx       (501) staff       (20)      408 2024-04-03 19:45:08.427095 bot_station_client-0.0.4/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)       24 2024-03-22 14:41:22.000000 bot_station_client-0.0.4/README.md
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 19:45:08.422400 bot_station_client-0.0.4/bot_station_client/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 14:38:45.000000 bot_station_client-0.0.4/bot_station_client/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     2704 2024-04-03 19:44:30.000000 bot_station_client-0.0.4/bot_station_client/client.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 19:45:08.425333 bot_station_client-0.0.4/bot_station_client/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-22 15:15:24.000000 bot_station_client-0.0.4/bot_station_client/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      100 2024-03-22 15:23:15.000000 bot_station_client-0.0.4/bot_station_client/model/config.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-04-03 19:45:08.426208 bot_station_client-0.0.4/bot_station_client.egg-info/
+-rw-r--r--   0 mrmx       (501) staff       (20)      408 2024-04-03 19:45:08.000000 bot_station_client-0.0.4/bot_station_client.egg-info/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)      367 2024-04-03 19:45:08.000000 bot_station_client-0.0.4/bot_station_client.egg-info/SOURCES.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)        1 2024-04-03 19:45:08.000000 bot_station_client-0.0.4/bot_station_client.egg-info/dependency_links.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       17 2024-04-03 19:45:08.000000 bot_station_client-0.0.4/bot_station_client.egg-info/requires.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       19 2024-04-03 19:45:08.000000 bot_station_client-0.0.4/bot_station_client.egg-info/top_level.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       38 2024-04-03 19:45:08.428400 bot_station_client-0.0.4/setup.cfg
+-rw-r--r--   0 mrmx       (501) staff       (20)      780 2024-04-03 19:44:44.000000 bot_station_client-0.0.4/setup.py
```

### Comparing `bot_station_client-0.0.3/LICENSE` & `bot_station_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station_client-0.0.3/bot_station_client/client.py` & `bot_station_client-0.0.4/bot_station_client/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 from typing import Dict, Any
 
 import aiohttp
-
 from bot_station_client.model.config import BotStationClientConfig
 
 
 class BotStationClient:
     config: BotStationClientConfig = ""
 
     def __init__(self, config: BotStationClientConfig):
@@ -78,14 +77,13 @@
     async def __post(self,
                      method: str,
                      content: Dict[str, str | int],
                      ) -> Any:
         """
         Returns response json body
         """
-        headers: Dict[str, str] = {}
-        content_str: str = json.dumps(content)
-        async with aiohttp.ClientSession(headers=headers) as session:
-            url = f'{self.config.base_uri}/{method}'
-            async with session.post(url=url, data=content_str) as response:
-                data = await response.json()
-                return data
+        headers: Dict[str, str] = {'content-type': 'application/json'}
+        session = aiohttp.ClientSession(headers=headers)
+        url = f'{self.config.base_uri}/{method}'
+        response = await session.post(url=url, data=json.dumps(content))
+        data = await response.json()
+        return data
```

### Comparing `bot_station_client-0.0.3/setup.py` & `bot_station_client-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="bot_station_client",
-    version="0.0.3",
+    version="0.0.4",
     author="Maxim Marashan",
     # author_email="ericjaychi@gmail.com",
     description="Bot Station client SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/ericjaychi/sample-pypi-package",
     packages=setuptools.find_packages(),
```

