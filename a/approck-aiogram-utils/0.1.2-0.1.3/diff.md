# Comparing `tmp/approck_aiogram_utils-0.1.2.tar.gz` & `tmp/approck_aiogram_utils-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_aiogram_utils-0.1.2.tar", max compression
+gzip compressed data, was "approck_aiogram_utils-0.1.3.tar", max compression
```

## Comparing `approck_aiogram_utils-0.1.2.tar` & `approck_aiogram_utils-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       23 2024-04-03 20:11:19.092525 approck_aiogram_utils-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 20:11:19.116525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/__init__.py
--rw-r--r--   0        0        0     1314 2024-04-03 20:11:19.093525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/app.py
--rw-r--r--   0        0        0     5100 2024-04-03 20:11:19.093525 approck_aiogram_utils-0.1.2/approck_aiogram_utils/message.py
--rw-r--r--   0        0        0      773 2024-04-03 20:11:19.094525 approck_aiogram_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:48:21.423008 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/__init__.py
+-rw-r--r--   0        0        0     1314 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/app.py
+-rw-r--r--   0        0        0     5104 2024-04-03 21:48:21.400009 approck_aiogram_utils-0.1.3/approck_aiogram_utils/message.py
+-rw-r--r--   0        0        0      773 2024-04-03 21:48:21.401008 approck_aiogram_utils-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      876 1970-01-01 00:00:00.000000 approck_aiogram_utils-0.1.3/PKG-INFO
```

### Comparing `approck_aiogram_utils-0.1.2/approck_aiogram_utils/integration/uprock/app.py` & `approck_aiogram_utils-0.1.3/approck_aiogram_utils/integration/uprock/app.py`

 * *Files identical despite different names*

### Comparing `approck_aiogram_utils-0.1.2/approck_aiogram_utils/message.py` & `approck_aiogram_utils-0.1.3/approck_aiogram_utils/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 async def _send_message_video_note(
     bot: Bot,
     chat_id: Union[int, str],
     message: Message,
     reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup, ReplyKeyboardRemove, ForceReply]] = None,
 ) -> None:
     await bot.send_video_note(
-        chat_id=chat_id, video_note=URLInputFile(url=message.video_note), reply_markup=reply_markup
+        chat_id=chat_id, video_note=URLInputFile(url=message.video_note.url), reply_markup=reply_markup
     )
 
 
 async def _send_message_impl(
     bot: Bot,
     chat_id: Union[int, str],
     message: Message,
```

### Comparing `approck_aiogram_utils-0.1.2/pyproject.toml` & `approck_aiogram_utils-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-aiogram-utils"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 aiogram = "^3.4.1"
 approck-messaging = [
```

### Comparing `approck_aiogram_utils-0.1.2/PKG-INFO` & `approck_aiogram_utils-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-aiogram-utils
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Aleksey Dalekin
 Author-email: ald@approck.pro
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

