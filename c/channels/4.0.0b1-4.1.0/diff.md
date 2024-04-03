# Comparing `tmp/channels-4.0.0b1.tar.gz` & `tmp/channels-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "channels-4.0.0b1.tar", last modified: Thu Aug 25 13:29:19 2022, max compression
+gzip compressed data, was "channels-4.1.0.tar", last modified: Wed Apr  3 14:01:35 2024, max compression
```

## Comparing `channels-4.0.0b1.tar` & `channels-4.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.274709 channels-4.0.0b1/
--rw-r--r--   0 carlton    (501) staff       (20)     1552 2022-01-27 19:52:18.000000 channels-4.0.0b1/LICENSE
--rw-r--r--   0 carlton    (501) staff       (20)       42 2022-01-27 19:52:18.000000 channels-4.0.0b1/MANIFEST.in
--rw-r--r--   0 carlton    (501) staff       (20)     1177 2022-08-25 13:29:19.274758 channels-4.0.0b1/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)     3036 2022-07-25 13:10:20.000000 channels-4.0.0b1/README.rst
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.272708 channels-4.0.0b1/channels/
--rw-r--r--   0 carlton    (501) staff       (20)       60 2022-08-25 13:25:17.000000 channels-4.0.0b1/channels/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)      122 2022-08-08 11:56:06.000000 channels-4.0.0b1/channels/apps.py
--rw-r--r--   0 carlton    (501) staff       (20)     6547 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/auth.py
--rw-r--r--   0 carlton    (501) staff       (20)     4316 2022-05-24 12:44:20.000000 channels-4.0.0b1/channels/consumer.py
--rw-r--r--   0 carlton    (501) staff       (20)      562 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/db.py
--rw-r--r--   0 carlton    (501) staff       (20)     1119 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/exceptions.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.273623 channels-4.0.0b1/channels/generic/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/generic/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     3089 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/generic/http.py
--rw-r--r--   0 carlton    (501) staff       (20)     8563 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/generic/websocket.py
--rw-r--r--   0 carlton    (501) staff       (20)    11809 2022-07-21 10:16:59.000000 channels-4.0.0b1/channels/layers.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.273737 channels-4.0.0b1/channels/management/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/management/__init__.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.273932 channels-4.0.0b1/channels/management/commands/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/management/commands/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     1594 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/management/commands/runworker.py
--rw-r--r--   0 carlton    (501) staff       (20)      756 2022-07-25 15:26:04.000000 channels-4.0.0b1/channels/middleware.py
--rw-r--r--   0 carlton    (501) staff       (20)     5772 2022-08-08 12:11:30.000000 channels-4.0.0b1/channels/routing.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.274146 channels-4.0.0b1/channels/security/
--rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/security/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     5800 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/security/websocket.py
--rw-r--r--   0 carlton    (501) staff       (20)    10062 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/sessions.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.274596 channels-4.0.0b1/channels/testing/
--rw-r--r--   0 carlton    (501) staff       (20)      343 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/testing/__init__.py
--rw-r--r--   0 carlton    (501) staff       (20)     2043 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/testing/http.py
--rw-r--r--   0 carlton    (501) staff       (20)     2455 2022-08-25 07:34:20.000000 channels-4.0.0b1/channels/testing/live.py
--rw-r--r--   0 carlton    (501) staff       (20)     3901 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/testing/websocket.py
--rw-r--r--   0 carlton    (501) staff       (20)     2176 2022-04-07 11:59:51.000000 channels-4.0.0b1/channels/utils.py
--rw-r--r--   0 carlton    (501) staff       (20)     1687 2022-01-27 19:52:18.000000 channels-4.0.0b1/channels/worker.py
-drwxr-xr-x   0 carlton    (501) staff       (20)        0 2022-08-25 13:29:19.273277 channels-4.0.0b1/channels.egg-info/
--rw-r--r--   0 carlton    (501) staff       (20)     1177 2022-08-25 13:29:19.000000 channels-4.0.0b1/channels.egg-info/PKG-INFO
--rw-r--r--   0 carlton    (501) staff       (20)      811 2022-08-25 13:29:19.000000 channels-4.0.0b1/channels.egg-info/SOURCES.txt
--rw-r--r--   0 carlton    (501) staff       (20)        1 2022-08-25 13:29:19.000000 channels-4.0.0b1/channels.egg-info/dependency_links.txt
--rw-r--r--   0 carlton    (501) staff       (20)      129 2022-08-25 13:29:19.000000 channels-4.0.0b1/channels.egg-info/requires.txt
--rw-r--r--   0 carlton    (501) staff       (20)        9 2022-08-25 13:29:19.000000 channels-4.0.0b1/channels.egg-info/top_level.txt
--rw-r--r--   0 carlton    (501) staff       (20)      226 2022-08-25 13:29:19.274964 channels-4.0.0b1/setup.cfg
--rw-r--r--   0 carlton    (501) staff       (20)     1621 2022-08-25 10:14:15.000000 channels-4.0.0b1/setup.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.472038 channels-4.1.0/
+-rw-r--r--   0 carlton    (501) staff       (20)     1552 2022-01-27 19:52:18.000000 channels-4.1.0/LICENSE
+-rw-r--r--   0 carlton    (501) staff       (20)       42 2022-01-27 19:52:18.000000 channels-4.1.0/MANIFEST.in
+-rw-r--r--   0 carlton    (501) staff       (20)     4487 2024-04-03 14:01:35.471884 channels-4.1.0/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)     3026 2024-04-03 13:29:07.000000 channels-4.1.0/README.rst
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.466397 channels-4.1.0/channels/
+-rw-r--r--   0 carlton    (501) staff       (20)       58 2024-04-03 13:51:40.000000 channels-4.1.0/channels/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)      121 2024-04-03 12:49:32.000000 channels-4.1.0/channels/apps.py
+-rw-r--r--   0 carlton    (501) staff       (20)     6547 2022-04-07 11:59:51.000000 channels-4.1.0/channels/auth.py
+-rw-r--r--   0 carlton    (501) staff       (20)     4316 2022-10-15 18:14:26.000000 channels-4.1.0/channels/consumer.py
+-rw-r--r--   0 carlton    (501) staff       (20)      562 2022-04-07 11:59:51.000000 channels-4.1.0/channels/db.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1119 2022-01-27 19:52:18.000000 channels-4.1.0/channels/exceptions.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.467861 channels-4.1.0/channels/generic/
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.1.0/channels/generic/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     3085 2024-04-03 13:10:25.000000 channels-4.1.0/channels/generic/http.py
+-rw-r--r--   0 carlton    (501) staff       (20)     8864 2024-04-03 13:11:22.000000 channels-4.1.0/channels/generic/websocket.py
+-rw-r--r--   0 carlton    (501) staff       (20)    11953 2022-11-12 08:04:25.000000 channels-4.1.0/channels/layers.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.468387 channels-4.1.0/channels/management/
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.1.0/channels/management/__init__.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.468738 channels-4.1.0/channels/management/commands/
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.1.0/channels/management/commands/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1593 2024-04-03 12:49:32.000000 channels-4.1.0/channels/management/commands/runworker.py
+-rw-r--r--   0 carlton    (501) staff       (20)      756 2022-11-12 08:04:25.000000 channels-4.1.0/channels/middleware.py
+-rw-r--r--   0 carlton    (501) staff       (20)     6589 2024-04-03 13:10:25.000000 channels-4.1.0/channels/routing.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.469336 channels-4.1.0/channels/security/
+-rw-r--r--   0 carlton    (501) staff       (20)        0 2022-01-27 19:52:18.000000 channels-4.1.0/channels/security/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     5800 2022-04-07 11:59:51.000000 channels-4.1.0/channels/security/websocket.py
+-rw-r--r--   0 carlton    (501) staff       (20)    10070 2024-04-03 12:49:32.000000 channels-4.1.0/channels/sessions.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.470681 channels-4.1.0/channels/testing/
+-rw-r--r--   0 carlton    (501) staff       (20)      343 2022-01-27 19:52:18.000000 channels-4.1.0/channels/testing/__init__.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2043 2022-01-27 19:52:18.000000 channels-4.1.0/channels/testing/http.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2600 2022-11-12 08:04:25.000000 channels-4.1.0/channels/testing/live.py
+-rw-r--r--   0 carlton    (501) staff       (20)     4172 2024-04-03 13:11:22.000000 channels-4.1.0/channels/testing/websocket.py
+-rw-r--r--   0 carlton    (501) staff       (20)     2177 2022-11-12 08:04:25.000000 channels-4.1.0/channels/utils.py
+-rw-r--r--   0 carlton    (501) staff       (20)     1687 2022-01-27 19:52:18.000000 channels-4.1.0/channels/worker.py
+drwxr-xr-x   0 carlton    (501) staff       (20)        0 2024-04-03 14:01:35.471065 channels-4.1.0/channels.egg-info/
+-rw-r--r--   0 carlton    (501) staff       (20)     4487 2024-04-03 14:01:35.000000 channels-4.1.0/channels.egg-info/PKG-INFO
+-rw-r--r--   0 carlton    (501) staff       (20)      817 2024-04-03 14:01:35.000000 channels-4.1.0/channels.egg-info/SOURCES.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        1 2024-04-03 14:01:35.000000 channels-4.1.0/channels.egg-info/dependency_links.txt
+-rw-r--r--   0 carlton    (501) staff       (20)      127 2024-04-03 14:01:35.000000 channels-4.1.0/channels.egg-info/requires.txt
+-rw-r--r--   0 carlton    (501) staff       (20)        9 2024-04-03 14:01:35.000000 channels-4.1.0/channels.egg-info/top_level.txt
+-rw-r--r--   0 carlton    (501) staff       (20)       81 2024-04-03 12:49:32.000000 channels-4.1.0/pyproject.toml
+-rw-r--r--   0 carlton    (501) staff       (20)     1460 2024-04-03 14:01:35.472623 channels-4.1.0/setup.cfg
```

### Comparing `channels-4.0.0b1/LICENSE` & `channels-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/README.rst` & `channels-4.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 You can install channels from PyPI as the ``channels`` package.
 See our `installation <https://channels.readthedocs.io/en/latest/installation.html>`_
 and `tutorial <https://channels.readthedocs.io/en/latest/tutorial/index.html>`_ docs for more.
 
 Dependencies
 ------------
 
-All Channels projects currently support Python 3.7 and up. ``channels`` is
-compatible with Django 2.2, 3.2, 4.0 and 4.1.
+All Channels projects currently support Python 3.8 and up. ``channels`` is
+compatible with Django 4.2 and 5.0.
 
 
 Contributing
 ------------
 
 To learn more about contributing, please `read our contributing docs <https://channels.readthedocs.io/en/latest/contributing.html>`_.
```

### Comparing `channels-4.0.0b1/channels/auth.py` & `channels-4.1.0/channels/auth.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/consumer.py` & `channels-4.1.0/channels/consumer.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/db.py` & `channels-4.1.0/channels/db.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/exceptions.py` & `channels-4.1.0/channels/exceptions.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/generic/http.py` & `channels-4.1.0/channels/generic/http.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if "body" in message:
             self.body.append(message["body"])
         if not message.get("more_body"):
             try:
                 await self.handle(b"".join(self.body))
             finally:
                 await self.disconnect()
-                raise StopConsumer()
+            raise StopConsumer()
 
     async def http_disconnect(self, message):
         """
         Let the user do their cleanup and close the consumer.
         """
         await self.disconnect()
         raise StopConsumer()
```

### Comparing `channels-4.0.0b1/channels/generic/websocket.py` & `channels-4.1.0/channels/generic/websocket.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,19 +40,23 @@
             self.accept()
         except DenyConnection:
             self.close()
 
     def connect(self):
         self.accept()
 
-    def accept(self, subprotocol=None):
+    def accept(self, subprotocol=None, headers=None):
         """
         Accepts an incoming socket
         """
-        super().send({"type": "websocket.accept", "subprotocol": subprotocol})
+        message = {"type": "websocket.accept", "subprotocol": subprotocol}
+        if headers:
+            message["headers"] = list(headers)
+
+        super().send(message)
 
     def websocket_receive(self, message):
         """
         Called when a WebSocket frame is received. Decodes it and passes it
         to receive().
         """
         if "text" in message:
@@ -75,22 +79,24 @@
         elif bytes_data is not None:
             super().send({"type": "websocket.send", "bytes": bytes_data})
         else:
             raise ValueError("You must pass one of bytes_data or text_data")
         if close:
             self.close(close)
 
-    def close(self, code=None):
+    def close(self, code=None, reason=None):
         """
         Closes the WebSocket from the server end
         """
+        message = {"type": "websocket.close"}
         if code is not None and code is not True:
-            super().send({"type": "websocket.close", "code": code})
-        else:
-            super().send({"type": "websocket.close"})
+            message["code"] = code
+        if reason:
+            message["reason"] = reason
+        super().send(message)
 
     def websocket_disconnect(self, message):
         """
         Called when a WebSocket connection is closed. Base level so you don't
         need to call super() all the time.
         """
         try:
@@ -175,19 +181,22 @@
             await self.accept()
         except DenyConnection:
             await self.close()
 
     async def connect(self):
         await self.accept()
 
-    async def accept(self, subprotocol=None):
+    async def accept(self, subprotocol=None, headers=None):
         """
         Accepts an incoming socket
         """
-        await super().send({"type": "websocket.accept", "subprotocol": subprotocol})
+        message = {"type": "websocket.accept", "subprotocol": subprotocol}
+        if headers:
+            message["headers"] = list(headers)
+        await super().send(message)
 
     async def websocket_receive(self, message):
         """
         Called when a WebSocket frame is received. Decodes it and passes it
         to receive().
         """
         if "text" in message:
@@ -210,22 +219,24 @@
         elif bytes_data is not None:
             await super().send({"type": "websocket.send", "bytes": bytes_data})
         else:
             raise ValueError("You must pass one of bytes_data or text_data")
         if close:
             await self.close(close)
 
-    async def close(self, code=None):
+    async def close(self, code=None, reason=None):
         """
         Closes the WebSocket from the server end
         """
+        message = {"type": "websocket.close"}
         if code is not None and code is not True:
-            await super().send({"type": "websocket.close", "code": code})
-        else:
-            await super().send({"type": "websocket.close"})
+            message["code"] = code
+        if reason:
+            message["reason"] = reason
+        await super().send(message)
 
     async def websocket_disconnect(self, message):
         """
         Called when a WebSocket connection is closed. Base level so you don't
         need to call super() all the time.
         """
         try:
```

### Comparing `channels-4.0.0b1/channels/layers.py` & `channels-4.1.0/channels/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,16 @@
 
 class BaseChannelLayer:
     """
     Base channel layer class that others can inherit from, with useful
     common functionality.
     """
 
+    MAX_NAME_LENGTH = 100
+
     def __init__(self, expiry=60, capacity=100, channel_capacity=None):
         self.expiry = expiry
         self.capacity = capacity
         self.channel_capacity = channel_capacity or {}
 
     def compile_capacities(self, channel_capacity):
         """
@@ -127,43 +129,45 @@
         """
         for pattern, capacity in self.channel_capacity:
             if pattern.match(channel):
                 return capacity
         return self.capacity
 
     def match_type_and_length(self, name):
-        if isinstance(name, str) and (len(name) < 100):
+        if isinstance(name, str) and (len(name) < self.MAX_NAME_LENGTH):
             return True
         return False
 
     # Name validation functions
 
     channel_name_regex = re.compile(r"^[a-zA-Z\d\-_.]+(\![\d\w\-_.]*)?$")
     group_name_regex = re.compile(r"^[a-zA-Z\d\-_.]+$")
     invalid_name_error = (
-        "{} name must be a valid unicode string containing only ASCII "
-        + "alphanumerics, hyphens, underscores, or periods."
+        "{} name must be a valid unicode string "
+        + "with length < {} ".format(MAX_NAME_LENGTH)
+        + "containing only ASCII alphanumerics, hyphens, underscores, or periods, "
+        + "not {}"
     )
 
     def valid_channel_name(self, name, receive=False):
         if self.match_type_and_length(name):
             if bool(self.channel_name_regex.match(name)):
                 # Check cases for special channels
                 if "!" in name and not name.endswith("!") and receive:
                     raise TypeError(
                         "Specific channel names in receive() must end at the !"
                     )
                 return True
-        raise TypeError(self.invalid_name_error("Channel"))
+        raise TypeError(self.invalid_name_error.format("Channel", name))
 
     def valid_group_name(self, name):
         if self.match_type_and_length(name):
             if bool(self.group_name_regex.match(name)):
                 return True
-        raise TypeError(self.invalid_name_error("Group"))
+        raise TypeError(self.invalid_name_error.format("Group", name))
 
     def valid_channel_names(self, names, receive=False):
         _non_empty_list = True if names else False
         _names_type = isinstance(names, list)
         assert _non_empty_list and _names_type, "names must be a non-empty list"
 
         assert all(
```

### Comparing `channels-4.0.0b1/channels/management/commands/runworker.py` & `channels-4.1.0/channels/management/commands/runworker.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from channels.routing import get_default_application
 from channels.worker import Worker
 
 logger = logging.getLogger("django.channels.worker")
 
 
 class Command(BaseCommand):
-
     leave_locale_alone = True
     worker_class = Worker
 
     def add_arguments(self, parser):
         super(Command, self).add_arguments(parser)
         parser.add_argument(
             "--layer",
```

### Comparing `channels-4.0.0b1/channels/middleware.py` & `channels-4.1.0/channels/middleware.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/routing.py` & `channels-4.1.0/channels/routing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib
 
 from django.conf import settings
 from django.core.exceptions import ImproperlyConfigured
 from django.urls.exceptions import Resolver404
-from django.urls.resolvers import URLResolver
+from django.urls.resolvers import RegexPattern, RoutePattern, URLResolver
 
 """
 All Routing instances inside this file are also valid ASGI applications - with
 new Channels routing, whatever you end up with as the top level object is just
 served up as the "ASGI application".
 """
 
@@ -83,27 +83,43 @@
     def __init__(self, routes):
         self.routes = routes
 
         for route in self.routes:
             # The inner ASGI app wants to do additional routing, route
             # must not be an endpoint
             if getattr(route.callback, "_path_routing", False) is True:
-                route.pattern._is_endpoint = False
+                pattern = route.pattern
+                if isinstance(pattern, RegexPattern):
+                    arg = pattern._regex
+                elif isinstance(pattern, RoutePattern):
+                    arg = pattern._route
+                else:
+                    raise ValueError(f"Unsupported pattern type: {type(pattern)}")
+                route.pattern = pattern.__class__(arg, pattern.name, is_endpoint=False)
 
             if not route.callback and isinstance(route, URLResolver):
                 raise ImproperlyConfigured(
                     "%s: include() is not supported in URLRouter. Use nested"
                     " URLRouter instances instead." % (route,)
                 )
 
     async def __call__(self, scope, receive, send):
         # Get the path
         path = scope.get("path_remaining", scope.get("path", None))
         if path is None:
             raise ValueError("No 'path' key in connection scope, cannot route URLs")
+
+        if "path_remaining" not in scope:
+            # We are the outermost URLRouter, so handle root_path if present.
+            root_path = scope.get("root_path", "")
+            if root_path and not path.startswith(root_path):
+                # If root_path is present, path must start with it.
+                raise ValueError("No route found for path %r." % path)
+            path = path[len(root_path) :]
+
         # Remove leading / to match Django's handling
         path = path.lstrip("/")
         # Run through the routes we have until one matches
         for route in self.routes:
             try:
                 match = route.pattern.match(path)
                 if match:
```

### Comparing `channels-4.0.0b1/channels/security/websocket.py` & `channels-4.1.0/channels/security/websocket.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/sessions.py` & `channels-4.1.0/channels/sessions.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
                 "lax",
                 "none",
             ], "samesite must be either 'strict', 'lax' or 'none'"
             cookies[key]["samesite"] = samesite
         # Write out the cookies to the response
         for c in cookies.values():
             message.setdefault("headers", []).append(
-                (b"Set-Cookie", bytes(c.output(header=""), encoding="utf-8"))
+                (b"Set-Cookie", bytes(c.output(header="").strip(), encoding="utf-8"))
             )
 
     @classmethod
     def delete_cookie(cls, message, key, path="/", domain=None):
         """
         Deletes a cookie in a response.
         """
```

### Comparing `channels-4.0.0b1/channels/testing/http.py` & `channels-4.1.0/channels/testing/http.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels/testing/live.py` & `channels-4.1.0/channels/testing/live.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-import multiprocessing
+from functools import partial
 
 from daphne.testing import DaphneProcess
 from django.contrib.staticfiles.handlers import ASGIStaticFilesHandler
 from django.core.exceptions import ImproperlyConfigured
 from django.db import connections
 from django.test.testcases import TransactionTestCase
 from django.test.utils import modify_settings
 
 from channels.routing import get_default_application
 
-# Enforce multiprocessing start method for macOS.
-multiprocessing.set_start_method("fork")
+
+def make_application(*, static_wrapper):
+    # Module-level function for pickle-ability
+    application = get_default_application()
+    if static_wrapper is not None:
+        application = static_wrapper(application)
+    return application
 
 
 class ChannelsLiveServerTestCase(TransactionTestCase):
     """
     Does basically the same as TransactionTestCase but also launches a
     live Daphne server in a separate process, so
     that the tests may use another test framework, such as Selenium,
@@ -44,20 +49,19 @@
         super(ChannelsLiveServerTestCase, self)._pre_setup()
 
         self._live_server_modified_settings = modify_settings(
             ALLOWED_HOSTS={"append": self.host}
         )
         self._live_server_modified_settings.enable()
 
-        if self.serve_static:
-            application = self.static_wrapper(get_default_application())
-        else:
-            application = get_default_application()
-
-        self._server_process = self.ProtocolServerProcess(self.host, application)
+        get_application = partial(
+            make_application,
+            static_wrapper=self.static_wrapper if self.serve_static else None,
+        )
+        self._server_process = self.ProtocolServerProcess(self.host, get_application)
         self._server_process.start()
         self._server_process.ready.wait()
         self._port = self._server_process.port.value
 
     def _post_teardown(self):
         self._server_process.terminate()
         self._server_process.join()
```

### Comparing `channels-4.0.0b1/channels/testing/websocket.py` & `channels-4.1.0/channels/testing/websocket.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,39 +8,46 @@
     """
     ApplicationCommunicator subclass that has WebSocket shortcut methods.
 
     It will construct the scope for you, so you need to pass the application
     (uninstantiated) along with the initial connection parameters.
     """
 
-    def __init__(self, application, path, headers=None, subprotocols=None):
+    def __init__(
+        self, application, path, headers=None, subprotocols=None, spec_version=None
+    ):
         if not isinstance(path, str):
             raise TypeError("Expected str, got {}".format(type(path)))
         parsed = urlparse(path)
         self.scope = {
             "type": "websocket",
             "path": unquote(parsed.path),
             "query_string": parsed.query.encode("utf-8"),
             "headers": headers or [],
             "subprotocols": subprotocols or [],
         }
+        if spec_version:
+            self.scope["spec_version"] = spec_version
         super().__init__(application, self.scope)
+        self.response_headers = None
 
     async def connect(self, timeout=1):
         """
         Trigger the connection code.
 
         On an accepted connection, returns (True, <chosen-subprotocol>)
         On a rejected connection, returns (False, <close-code>)
         """
         await self.send_input({"type": "websocket.connect"})
         response = await self.receive_output(timeout)
         if response["type"] == "websocket.close":
             return (False, response.get("code", 1000))
         else:
+            assert response["type"] == "websocket.accept"
+            self.response_headers = response.get("headers", [])
             return (True, response.get("subprotocol", None))
 
     async def send_to(self, text_data=None, bytes_data=None):
         """
         Sends a WebSocket frame to the application.
         """
         # Make sure we have exactly one of the arguments
```

### Comparing `channels-4.0.0b1/channels/utils.py` & `channels-4.1.0/channels/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
 
 async def await_many_dispatch(consumer_callables, dispatch):
     """
     Given a set of consumer callables, awaits on them all and passes results
     from them to the dispatch awaitable as they come in.
     """
-    # Start them all off as tasks
-    loop = asyncio.get_event_loop()
+    # Call all callables, and ensure all return types are Futures
     tasks = [
-        loop.create_task(consumer_callable())
+        asyncio.ensure_future(consumer_callable())
         for consumer_callable in consumer_callables
     ]
     try:
         while True:
             # Wait for any of them to complete
             await asyncio.wait(tasks, return_when=asyncio.FIRST_COMPLETED)
             # Find the completed one(s), yield results, and replace them
```

### Comparing `channels-4.0.0b1/channels/worker.py` & `channels-4.1.0/channels/worker.py`

 * *Files identical despite different names*

### Comparing `channels-4.0.0b1/channels.egg-info/SOURCES.txt` & `channels-4.1.0/channels.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
 channels/__init__.py
 channels/apps.py
 channels/auth.py
 channels/consumer.py
 channels/db.py
 channels/exceptions.py
 channels/layers.py
```

