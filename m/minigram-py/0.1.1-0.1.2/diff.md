# Comparing `tmp/minigram_py-0.1.1.tar.gz` & `tmp/minigram_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minigram_py-0.1.1.tar", last modified: Wed Apr  3 20:41:54 2024, max compression
+gzip compressed data, was "minigram_py-0.1.2.tar", last modified: Wed Apr  3 21:08:36 2024, max compression
```

## Comparing `minigram_py-0.1.1.tar` & `minigram_py-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.1/LICENSE
--rw-r--r--   0        0        0     2916 2024-04-03 20:41:41.418410 minigram_py-0.1.1/README.md
--rw-r--r--   0        0        0      542 2024-04-03 20:41:54.332791 minigram_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.1/src/minigram/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.1/src/minigram/aiohttp.py
--rw-r--r--   0        0        0      695 2024-04-03 20:41:41.419190 minigram_py-0.1.1/src/minigram/ass.py
--rw-r--r--   0        0        0     4979 2024-04-03 20:41:41.423188 minigram_py-0.1.1/src/minigram/main.py
--rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.1/src/minigram/py.typed
--rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.1/src/minigram/request.py
--rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.1/src/minigram/starlette.py
--rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 minigram_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2922 2024-04-03 21:06:24.236374 minigram_py-0.1.2/README.md
+-rw-r--r--   0        0        0      542 2024-04-03 21:08:36.048473 minigram_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.2/src/minigram/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.2/src/minigram/aiohttp.py
+-rw-r--r--   0        0        0      698 2024-04-03 21:07:03.769425 minigram_py-0.1.2/src/minigram/ass.py
+-rw-r--r--   0        0        0     5105 2024-04-03 21:05:43.162608 minigram_py-0.1.2/src/minigram/main.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.2/src/minigram/py.typed
+-rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.2/src/minigram/request.py
+-rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.2/src/minigram/starlette.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 minigram_py-0.1.2/PKG-INFO
```

### Comparing `minigram_py-0.1.1/LICENSE` & `minigram_py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.1/README.md` & `minigram_py-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ### Basic Example
 
 ```python
 from minigram import MiniGram
 
 class MyAwesomeBot(MiniGram):
-    def incoming(self, msg):
+    async def incoming(self, msg):
         if msg.text == "/start":
             return msg.reply("Welcome to my awesome bot! 🎉")
 
 bot = MyAwesomeBot("YOUR_BOT_TOKEN")
 bot.start_polling()
 ```
```

### Comparing `minigram_py-0.1.1/pyproject.toml` & `minigram_py-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "minigram-py"
-version = "0.1.1"
+version = "0.1.2"
 description = "minimalistic telegram bot framework that can be used in AWS Lambda or anywhere"
 authors = [
     { name = "Grigory Bakunov", email = "bobuk@rubedo.cloud" },
 ]
 dependencies = []
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `minigram_py-0.1.1/src/minigram/main.py` & `minigram_py-0.1.2/src/minigram/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,18 @@
         return response
 
     @ass
     async def start_polling(self):
         while True:
             updates = await self.get_updates()
             for update in updates.get("result", []):
-                await self.incoming(update)
+                msg = MiniGramMessage(update)
+                res = await self.incoming(msg)
+                if res:
+                    await self.reply_to_message(res)
                 self.last_updated_id = update["update_id"]
             await asyncio.sleep(0.1)
 
     @ass
     async def get_updates(self) -> dict:
         if self.last_updated_id != 0:
             return await self.req(
```

### Comparing `minigram_py-0.1.1/src/minigram/request.py` & `minigram_py-0.1.2/src/minigram/request.py`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.1/PKG-INFO` & `minigram_py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minigram-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: minimalistic telegram bot framework that can be used in AWS Lambda or anywhere
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: MIT
 Requires-Python: >=3.12
 Provides-Extra: starlette
 Provides-Extra: aiohttp
 Requires-Dist: starlette>=0.37.2; extra == "starlette"
@@ -37,15 +37,15 @@
 
 ### Basic Example
 
 ```python
 from minigram import MiniGram
 
 class MyAwesomeBot(MiniGram):
-    def incoming(self, msg):
+    async def incoming(self, msg):
         if msg.text == "/start":
             return msg.reply("Welcome to my awesome bot! 🎉")
 
 bot = MyAwesomeBot("YOUR_BOT_TOKEN")
 bot.start_polling()
 ```
```

