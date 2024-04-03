# Comparing `tmp/sweetdebug-1.0.8.tar.gz` & `tmp/sweetdebug-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweetdebug-1.0.8.tar", last modified: Thu Jan 25 06:13:39 2024, max compression
+gzip compressed data, was "sweetdebug-1.0.9.tar", last modified: Mon Jan 29 13:59:31 2024, max compression
```

## Comparing `sweetdebug-1.0.8.tar` & `sweetdebug-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:13:39.326973 sweetdebug-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-25 06:13:39.326973 sweetdebug-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-25 06:13:26.000000 sweetdebug-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 06:13:39.326973 sweetdebug-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-25 06:13:26.000000 sweetdebug-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:13:39.326973 sweetdebug-1.0.8/sweetdebug/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-25 06:13:26.000000 sweetdebug-1.0.8/sweetdebug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-01-25 06:13:26.000000 sweetdebug-1.0.8/sweetdebug/dm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-25 06:13:26.000000 sweetdebug-1.0.8/sweetdebug/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 06:13:39.326973 sweetdebug-1.0.8/sweetdebug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-25 06:13:39.000000 sweetdebug-1.0.8/sweetdebug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-25 06:13:39.000000 sweetdebug-1.0.8/sweetdebug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 06:13:39.000000 sweetdebug-1.0.8/sweetdebug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-25 06:13:39.000000 sweetdebug-1.0.8/sweetdebug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-25 06:13:39.000000 sweetdebug-1.0.8/sweetdebug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 13:59:31.045464 sweetdebug-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-29 13:59:31.045464 sweetdebug-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-29 13:59:19.000000 sweetdebug-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 13:59:31.045464 sweetdebug-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-29 13:59:19.000000 sweetdebug-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 13:59:31.045464 sweetdebug-1.0.9/sweetdebug/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-29 13:59:19.000000 sweetdebug-1.0.9/sweetdebug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-01-29 13:59:19.000000 sweetdebug-1.0.9/sweetdebug/dm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-29 13:59:19.000000 sweetdebug-1.0.9/sweetdebug/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 13:59:31.045464 sweetdebug-1.0.9/sweetdebug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-01-29 13:59:31.000000 sweetdebug-1.0.9/sweetdebug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-01-29 13:59:31.000000 sweetdebug-1.0.9/sweetdebug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 13:59:31.000000 sweetdebug-1.0.9/sweetdebug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-29 13:59:31.000000 sweetdebug-1.0.9/sweetdebug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-29 13:59:31.000000 sweetdebug-1.0.9/sweetdebug.egg-info/top_level.txt
```

### Comparing `sweetdebug-1.0.8/PKG-INFO` & `sweetdebug-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetdebug
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic pdb invoker
 Home-page: https://github.com/sweetcocoa/sweetdebug
 Author: sweetcocoa
 Author-email: sweetcocoa@snu.ac.kr
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `sweetdebug-1.0.8/README.md` & `sweetdebug-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sweetdebug-1.0.8/setup.py` & `sweetdebug-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="sweetdebug",
-    version="1.0.8",
+    version="1.0.9",
     description="Automatic pdb invoker",
     author="sweetcocoa",
     author_email="sweetcocoa@snu.ac.kr",
     url="https://github.com/sweetcocoa/sweetdebug",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
```

### Comparing `sweetdebug-1.0.8/sweetdebug/dm.py` & `sweetdebug-1.0.9/sweetdebug/dm.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,42 @@
 import typing
 import logging
 import datetime
 import os
 
 TELEGRAM_INSTALLED = False
 TELEGRAM_CACHE = os.path.join(os.path.dirname(__file__), "cache.txt")
+TELEGRAM_MAX_MESSAGE_LENGTH = 4096
 
 try:
     import telegram
 
     TELEGRAM_INSTALLED = True
 except ImportError:
     pass
 
 
 async def send_telegram_message(token, chat_ids, message):
+    messages = [
+        message[i : i + TELEGRAM_MAX_MESSAGE_LENGTH]
+        for i in range(0, len(message), TELEGRAM_MAX_MESSAGE_LENGTH)
+    ]
+
+    if len(messages) > 2:
+        messages = [
+            messages[0],
+            "\n\n ... \n\n [skipped by sweetdebug] \n\n ... \n\n",
+            (messages[-2] + messages[-1])[-TELEGRAM_MAX_MESSAGE_LENGTH:],
+        ]
+
     try:
         async with telegram.Bot(token) as bot:
             for chat_id in chat_ids:
-                await bot.send_message(chat_id=str(chat_id), text=message)
+                for message in messages:
+                    await bot.send_message(chat_id=str(chat_id), text=message)
     except telegram.error.TelegramError as e:
         logging.warning(f"sweetdebug : telegram error, {e}, {type(e)}")
 
 
 def load_cache():
     with open(TELEGRAM_CACHE) as f:
         contents = f.readlines()
```

### Comparing `sweetdebug-1.0.8/sweetdebug/timer.py` & `sweetdebug-1.0.9/sweetdebug/timer.py`

 * *Files identical despite different names*

### Comparing `sweetdebug-1.0.8/sweetdebug.egg-info/PKG-INFO` & `sweetdebug-1.0.9/sweetdebug.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweetdebug
-Version: 1.0.8
+Version: 1.0.9
 Summary: Automatic pdb invoker
 Home-page: https://github.com/sweetcocoa/sweetdebug
 Author: sweetcocoa
 Author-email: sweetcocoa@snu.ac.kr
 License: MIT
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

