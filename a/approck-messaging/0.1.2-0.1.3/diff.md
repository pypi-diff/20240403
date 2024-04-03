# Comparing `tmp/approck_messaging-0.1.2.tar.gz` & `tmp/approck_messaging-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approck_messaging-0.1.2.tar", max compression
+gzip compressed data, was "approck_messaging-0.1.3.tar", max compression
```

## Comparing `approck_messaging-0.1.2.tar` & `approck_messaging-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       19 2024-03-19 20:09:34.923725 approck_messaging-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-19 20:09:34.946724 approck_messaging-0.1.2/approck_messaging/__init__.py
--rw-r--r--   0        0        0        0 2024-03-19 20:09:34.947724 approck_messaging-0.1.2/approck_messaging/models/__init__.py
--rw-r--r--   0        0        0      748 2024-03-19 20:09:34.923725 approck_messaging-0.1.2/approck_messaging/models/message.py
--rw-r--r--   0        0        0      743 2024-03-19 20:09:34.923725 approck_messaging-0.1.2/approck_messaging/publisher.py
--rw-r--r--   0        0        0      807 2024-03-19 20:09:34.923725 approck_messaging-0.1.2/approck_messaging/subscriber.py
--rw-r--r--   0        0        0      598 2024-03-19 20:09:34.924724 approck_messaging-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 approck_messaging-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       19 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 19:48:45.791515 approck_messaging-0.1.3/approck_messaging/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 19:48:45.791515 approck_messaging-0.1.3/approck_messaging/models/__init__.py
+-rw-r--r--   0        0        0      753 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/models/message.py
+-rw-r--r--   0        0        0      743 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/publisher.py
+-rw-r--r--   0        0        0      817 2024-04-03 19:48:45.767516 approck_messaging-0.1.3/approck_messaging/subscriber.py
+-rw-r--r--   0        0        0      598 2024-04-03 19:48:45.768516 approck_messaging-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 approck_messaging-0.1.3/PKG-INFO
```

### Comparing `approck_messaging-0.1.2/approck_messaging/models/message.py` & `approck_messaging-0.1.3/approck_messaging/models/message.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     # Generic
     caption: Optional[str] = None
     media: Optional[List[MessageMedia]] = None
     buttons: Optional[List[MessageButton]] = None
 
     # Video Note
-    video_note: Optional[HttpUrl] = None
+    video_note: Optional[MessageMedia] = None
 
 
 class TransportMessageRecipient(BaseModel):
     telegram_id: int
 
 
 class TransportMessage(Message):
```

### Comparing `approck_messaging-0.1.2/approck_messaging/publisher.py` & `approck_messaging-0.1.3/approck_messaging/publisher.py`

 * *Files identical despite different names*

### Comparing `approck_messaging-0.1.2/approck_messaging/subscriber.py` & `approck_messaging-0.1.3/approck_messaging/subscriber.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.broker = broker
 
         for key, value in kwargs.items():
             context.set_global(key, value)
 
     @classmethod
     def from_uri(cls, redis_uri: str, **kwargs) -> "Subscriber":
-        return cls(broker=RedisBroker(redis_uri))
+        return cls(broker=RedisBroker(redis_uri), **kwargs)
 
     def message(
         self, stream: str
     ) -> Callable[
         [Callable[P_HandlerParams, T_HandlerReturn]],
         HandlerCallWrapper[Any, P_HandlerParams, T_HandlerReturn],
     ]:
```

### Comparing `approck_messaging-0.1.2/pyproject.toml` & `approck_messaging-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "approck-messaging"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Aleksey Dalekin <ald@approck.pro>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 faststream = { extras = ["redis"], version = "^0.4.4", optional = true }
 pydantic = { extras = ["email", "dotenv"], version = ">=2.4.1,<2.6" }
```

### Comparing `approck_messaging-0.1.2/PKG-INFO` & `approck_messaging-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approck-messaging
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

