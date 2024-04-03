# Comparing `tmp/minigram_py-0.1.0.tar.gz` & `tmp/minigram_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minigram_py-0.1.0.tar", last modified: Mon Apr  1 19:34:43 2024, max compression
+gzip compressed data, was "minigram_py-0.1.1.tar", last modified: Wed Apr  3 20:41:54 2024, max compression
```

## Comparing `minigram_py-0.1.0.tar` & `minigram_py-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.0/LICENSE
--rw-r--r--   0        0        0     2913 2024-04-01 19:34:24.622411 minigram_py-0.1.0/README.md
--rw-r--r--   0        0        0      542 2024-04-01 19:34:43.445878 minigram_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.0/src/minigram/__init__.py
--rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.0/src/minigram/aiohttp.py
--rw-r--r--   0        0        0      716 2024-04-01 19:34:24.841240 minigram_py-0.1.0/src/minigram/ass.py
--rw-r--r--   0        0        0     4974 2024-04-01 19:34:24.842964 minigram_py-0.1.0/src/minigram/main.py
--rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.0/src/minigram/py.typed
--rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.0/src/minigram/request.py
--rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.0/src/minigram/starlette.py
--rw-r--r--   0        0        0        0 2024-04-01 19:34:24.843137 minigram_py-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 minigram_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-01 19:34:24.620396 minigram_py-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2916 2024-04-03 20:41:41.418410 minigram_py-0.1.1/README.md
+-rw-r--r--   0        0        0      542 2024-04-03 20:41:54.332791 minigram_py-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      368 2024-04-01 19:34:24.841512 minigram_py-0.1.1/src/minigram/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-01 19:34:24.841106 minigram_py-0.1.1/src/minigram/aiohttp.py
+-rw-r--r--   0        0        0      695 2024-04-03 20:41:41.419190 minigram_py-0.1.1/src/minigram/ass.py
+-rw-r--r--   0        0        0     4979 2024-04-03 20:41:41.423188 minigram_py-0.1.1/src/minigram/main.py
+-rw-r--r--   0        0        0        0 2024-04-01 19:34:24.842703 minigram_py-0.1.1/src/minigram/py.typed
+-rw-r--r--   0        0        0     3002 2024-04-01 19:34:24.841375 minigram_py-0.1.1/src/minigram/request.py
+-rw-r--r--   0        0        0      476 2024-04-01 19:34:24.840972 minigram_py-0.1.1/src/minigram/starlette.py
+-rw-r--r--   0        0        0     3343 1970-01-01 00:00:00.000000 minigram_py-0.1.1/PKG-INFO
```

### Comparing `minigram_py-0.1.0/LICENSE` & `minigram_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.0/README.md` & `minigram_py-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     await bot.sent_text(YOUR_CHAT_ID, "Hello from an asynchronous bot! 🚀")
 ```
 
 MiniGram works just as well in asynchronous mode, making it easy to integrate with your existing async application. 🎛️
 
 ## Contributing 🤝
 
-We love contributions! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request on our [GitHub repository](https://github.com/bobuk/minigram). Let's make MiniGram even better together! 💪
+We love contributions! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request on our [GitHub repository](https://github.com/bobuk/minigram-py). Let's make MiniGram even better together! 💪
 
 ## License 📄
 
 MiniGram is released under the [MIT License](https://opensource.org/licenses/MIT), so feel free to use it in your projects, whether they're open-source or commercial. 😄
 
 ---
```

### Comparing `minigram_py-0.1.0/pyproject.toml` & `minigram_py-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "minigram-py"
-version = "0.1.0"
+version = "0.1.1"
 description = "minimalistic telegram bot framework that can be used in AWS Lambda or anywhere"
 authors = [
     { name = "Grigory Bakunov", email = "bobuk@rubedo.cloud" },
 ]
 dependencies = []
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `minigram_py-0.1.0/src/minigram/ass.py` & `minigram_py-0.1.1/src/minigram/ass.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 import functools
 import inspect
 
 def ass(func):
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         signature = inspect.signature(func).parameters
-        kargs = kwargs
         try:
             loop = asyncio.get_running_loop()
             if 'is_async' in signature:
                 kargs['is_async'] = True
-            return func(*args, **kargs)
+            return func(*args, **kwargs)
         except RuntimeError:
             if 'is_async' in signature:
                 kargs['is_async'] = False
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
-            result = loop.run_until_complete(func(*args, **kargs))
+            result = loop.run_until_complete(func(*args, **kwargs))
             loop.close()
             return result
 
     return wrapper
```

### Comparing `minigram_py-0.1.0/src/minigram/main.py` & `minigram_py-0.1.1/src/minigram/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return response
 
     @ass
     async def start_polling(self):
         while True:
             updates = await self.get_updates()
             for update in updates.get("result", []):
-                await self.handler(update)
+                await self.incoming(update)
                 self.last_updated_id = update["update_id"]
             await asyncio.sleep(0.1)
 
     @ass
     async def get_updates(self) -> dict:
         if self.last_updated_id != 0:
             return await self.req(
@@ -125,39 +125,43 @@
     @ass
     async def send_text(
         self, chat_id: int, text: str, parse_mode: str = "HTML", **kwargs
     ) -> dict:
         return await self.req(
             "sendMessage", chat_id=chat_id, text=text, parse_mode=parse_mode, **kwargs
         )
+
     @ass
     async def reply_to_message(self, reply: MiniGramMessage):
         reply_params = {
             "chat_id": reply.chat_id,
             "text": reply.text,
             "reply_to_message_id": reply.message_id,
         }
         return await self.req("sendMessage", **reply_params)
+
     @ass
     async def set_webhook(self, url: str) -> dict:
         return await self.req("setWebhook", url=url)
+
     @ass
     async def delete_webhook(self) -> dict:
         return await self.req("deleteWebhook")
+
     @ass
     async def get_webhook_info(self) -> dict:
         return await self.req("getWebhookInfo")
 
-
     async def async_handler(self, data: dict) -> None:
         msg = MiniGramMessage(data)
         res = await self.incoming(msg)
         if res:
             await self.reply_to_message(res)
 
     def sync_handler(self, data: dict) -> None:
         msg = MiniGramMessage(data)
         res = self.incoming(msg)
         if res:
             self.reply_to_message(res)
 
+
 CURRENT: MiniGram | None = None
```

### Comparing `minigram_py-0.1.0/src/minigram/request.py` & `minigram_py-0.1.1/src/minigram/request.py`

 * *Files identical despite different names*

### Comparing `minigram_py-0.1.0/PKG-INFO` & `minigram_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minigram-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: minimalistic telegram bot framework that can be used in AWS Lambda or anywhere
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: MIT
 Requires-Python: >=3.12
 Provides-Extra: starlette
 Provides-Extra: aiohttp
 Requires-Dist: starlette>=0.37.2; extra == "starlette"
@@ -89,15 +89,15 @@
     await bot.sent_text(YOUR_CHAT_ID, "Hello from an asynchronous bot! 🚀")
 ```
 
 MiniGram works just as well in asynchronous mode, making it easy to integrate with your existing async application. 🎛️
 
 ## Contributing 🤝
 
-We love contributions! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request on our [GitHub repository](https://github.com/bobuk/minigram). Let's make MiniGram even better together! 💪
+We love contributions! If you have any ideas, suggestions, or bug reports, please open an issue or submit a pull request on our [GitHub repository](https://github.com/bobuk/minigram-py). Let's make MiniGram even better together! 💪
 
 ## License 📄
 
 MiniGram is released under the [MIT License](https://opensource.org/licenses/MIT), so feel free to use it in your projects, whether they're open-source or commercial. 😄
 
 ---
```

