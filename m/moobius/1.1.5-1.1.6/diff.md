# Comparing `tmp/moobius-1.1.5.tar.gz` & `tmp/moobius-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moobius-1.1.5.tar", last modified: Fri Mar 29 16:36:25 2024, max compression
+gzip compressed data, was "moobius-1.1.6.tar", last modified: Wed Apr  3 05:37:41 2024, max compression
```

## Comparing `moobius-1.1.5.tar` & `moobius-1.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:25.006878 moobius-1.1.5/
--rw-rw-rw-   0        0        0     8910 2024-03-29 16:36:25.005875 moobius-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.5/license.md
--rw-rw-rw-   0        0        0      647 2024-03-29 16:35:46.000000 moobius-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.5/readme.md
--rw-rw-rw-   0        0        0       42 2024-03-29 16:36:25.007875 moobius-1.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:24.981466 moobius-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:24.984345 moobius-1.1.5/src/moobius/
--rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.5/src/moobius/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:24.993665 moobius-1.1.5/src/moobius/core/
--rw-rw-rw-   0        0        0    55479 2024-03-28 22:58:55.000000 moobius-1.1.5/src/moobius/core/sdk.py
--rw-rw-rw-   0        0        0     4170 2024-03-25 06:01:03.000000 moobius-1.1.5/src/moobius/core/wand.py
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:24.998709 moobius-1.1.5/src/moobius/database/
--rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.5/src/moobius/database/database_interface.py
--rw-rw-rw-   0        0        0     4062 2024-03-25 06:01:03.000000 moobius-1.1.5/src/moobius/database/json_database.py
--rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.5/src/moobius/database/null_database.py
--rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.5/src/moobius/database/redis_database.py
--rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.5/src/moobius/database/storage.py
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:25.004063 moobius-1.1.5/src/moobius/network/
--rw-rw-rw-   0        0        0    14222 2024-03-28 22:03:20.000000 moobius-1.1.5/src/moobius/network/asserts.py
--rw-rw-rw-   0        0        0    43927 2024-03-25 06:01:03.000000 moobius-1.1.5/src/moobius/network/http_api_wrapper.py
--rw-rw-rw-   0        0        0    25256 2024-03-28 22:27:41.000000 moobius-1.1.5/src/moobius/network/ws_client.py
--rw-rw-rw-   0        0        0     7154 2024-03-28 21:49:49.000000 moobius-1.1.5/src/moobius/types.py
--rw-rw-rw-   0        0        0     7399 2024-03-26 23:06:54.000000 moobius-1.1.5/src/moobius/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-29 16:36:25.005377 moobius-1.1.5/src/moobius.egg-info/
--rw-rw-rw-   0        0        0     8910 2024-03-29 16:36:24.000000 moobius-1.1.5/src/moobius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2024-03-29 16:36:24.000000 moobius-1.1.5/src/moobius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 16:36:24.000000 moobius-1.1.5/src/moobius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      131 2024-03-29 16:36:24.000000 moobius-1.1.5/src/moobius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-29 16:36:24.000000 moobius-1.1.5/src/moobius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      329 2024-03-26 23:06:54.000000 moobius-1.1.5/src/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.324196 moobius-1.1.6/
+-rw-rw-rw-   0        0        0     8910 2024-04-03 05:37:41.323200 moobius-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1067 2024-03-24 16:36:44.000000 moobius-1.1.6/license.md
+-rw-rw-rw-   0        0        0      647 2024-04-03 04:47:09.000000 moobius-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0     8055 2024-03-17 18:58:55.000000 moobius-1.1.6/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 05:37:41.324196 moobius-1.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.303965 moobius-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.307116 moobius-1.1.6/src/moobius/
+-rw-rw-rw-   0        0        0      184 2024-03-05 05:12:19.000000 moobius-1.1.6/src/moobius/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.314667 moobius-1.1.6/src/moobius/core/
+-rw-rw-rw-   0        0        0    56123 2024-04-02 21:26:58.000000 moobius-1.1.6/src/moobius/core/sdk.py
+-rw-rw-rw-   0        0        0     4170 2024-04-01 21:02:47.000000 moobius-1.1.6/src/moobius/core/wand.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.317651 moobius-1.1.6/src/moobius/database/
+-rw-rw-rw-   0        0        0     2655 2024-03-13 15:36:04.000000 moobius-1.1.6/src/moobius/database/database_interface.py
+-rw-rw-rw-   0        0        0     4062 2024-03-25 06:01:03.000000 moobius-1.1.6/src/moobius/database/json_database.py
+-rw-rw-rw-   0        0        0      902 2024-02-16 02:53:33.000000 moobius-1.1.6/src/moobius/database/null_database.py
+-rw-rw-rw-   0        0        0     1517 2024-03-25 06:01:03.000000 moobius-1.1.6/src/moobius/database/redis_database.py
+-rw-rw-rw-   0        0        0     9559 2024-03-26 23:06:54.000000 moobius-1.1.6/src/moobius/database/storage.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.321207 moobius-1.1.6/src/moobius/network/
+-rw-rw-rw-   0        0        0    14222 2024-04-01 23:40:33.000000 moobius-1.1.6/src/moobius/network/asserts.py
+-rw-rw-rw-   0        0        0    43927 2024-04-02 20:28:42.000000 moobius-1.1.6/src/moobius/network/http_api_wrapper.py
+-rw-rw-rw-   0        0        0    25652 2024-04-02 21:30:49.000000 moobius-1.1.6/src/moobius/network/ws_client.py
+-rw-rw-rw-   0        0        0     7154 2024-04-01 23:40:33.000000 moobius-1.1.6/src/moobius/types.py
+-rw-rw-rw-   0        0        0     7399 2024-03-29 15:46:12.000000 moobius-1.1.6/src/moobius/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 05:37:41.322208 moobius-1.1.6/src/moobius.egg-info/
+-rw-rw-rw-   0        0        0     8910 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      131 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 05:37:41.000000 moobius-1.1.6/src/moobius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      329 2024-03-26 23:06:54.000000 moobius-1.1.6/src/setup.py
```

### Comparing `moobius-1.1.5/PKG-INFO` & `moobius-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.5
+Version: 1.1.6
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.5/license.md` & `moobius-1.1.6/license.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/readme.md` & `moobius-1.1.6/readme.md`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/core/sdk.py` & `moobius-1.1.6/src/moobius/core/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         self.ws_client = WSClient(ws_server_uri, on_connect=self.send_agent_login if self.is_agent else self.send_service_login, handle=self.handle_received_payload)
 
         self.queue = aioprocessing.AioQueue()
 
         self.refresh_interval = 6 * 60 * 60             # 24h expire, 6h refresh
         self.authenticate_interval = 7 * 24 * 60 * 60   # 30d expire, 7d refresh
         self.heartbeat_interval = 30                    # 30s heartbeat
+        self.checkin_interval = 90
 
         self.scheduler = None
 
     async def start(self):
         """
         Start the Service/Agent. start() fns are called with wand.run. There are 6 steps:
           1. Authenticate.
@@ -245,14 +246,16 @@
 
         self.scheduler.start()
         logger.debug("Scheduler started.")
 
         await self.on_start()
         logger.debug("on_start() finished.")
 
+        self.scheduler.add_job(self.checkin, 'interval', seconds=self.checkin_interval) # This check-in must be after on_start()
+
         await asyncio.gather(self.ws_client.receive(), self.listen_loop())
 
     async def agent_join_service_channels(self, service_config_fname):
         """Joins service channels given by service config filename."""
         if not self.is_agent:
             logger.warning('Called agent_join_service_channels when not an agent.')
         if type(service_config_fname) is dict:
@@ -331,14 +334,24 @@
         return content
 
     async def initialize_channel(self, channel_id):
         """Creates a MoobiusStorage object for a channel given by channel_id. Commonly overridden. Returns None."""
         the_channel = MoobiusStorage(self.client_id, channel_id, db_config=self.db_config)
         self.channels[channel_id] = the_channel
 
+    async def checkin(self):
+        """Called as a rate task, used to resync users, etc. Only called after on_start()"""
+        for channel_id in self.channels.keys():
+            await self.checkin_channel(channel_id)
+
+    async def checkin_channel(self, channel_id):
+        """This is called on startup and on reconnect"""
+        if channel_id == list(self.channels.keys())[0]:
+            logger.warning('checkin_channel not overriden, occasional desyncs are possible.')
+
     async def upload_avatar_and_create_character(self, name, image_path, description):
         """
         Upload an avatar image and create a character. Service function.
 
         Parameters:
           name: str
             The name of the character.
```

### Comparing `moobius-1.1.5/src/moobius/core/wand.py` & `moobius-1.1.6/src/moobius/core/wand.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/database/database_interface.py` & `moobius-1.1.6/src/moobius/database/database_interface.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/database/json_database.py` & `moobius-1.1.6/src/moobius/database/json_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/database/null_database.py` & `moobius-1.1.6/src/moobius/database/null_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/database/redis_database.py` & `moobius-1.1.6/src/moobius/database/redis_database.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/database/storage.py` & `moobius-1.1.6/src/moobius/database/storage.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/network/asserts.py` & `moobius-1.1.6/src/moobius/network/asserts.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/network/http_api_wrapper.py` & `moobius-1.1.6/src/moobius/network/http_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/network/ws_client.py` & `moobius-1.1.6/src/moobius/network/ws_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
         """
         self.websocket = None
         self.ws_server_uri = ws_server_uri
         async def _on_connect(self): logger.info(f"Connected to {self.ws_server_uri}")
         async def _default_handle(self, message): logger.debug(f"{message}")
         self.on_connect = on_connect or _on_connect
         self.handle = handle or _default_handle
+        self.is_reconnecting = False # Block sending messages until this becomes True.
 
     async def connect(self):
         """Connects to the websocket server. Call after self.authenticate(). Returns None."""
         self.websocket = await websockets.connect(self.ws_server_uri)
         await self.on_connect()
 
     async def send(self, message):
@@ -70,24 +71,28 @@
         Returns None, but if the server responds to the message it will be detected in the self.recieve() loop.
         """
         if type(message) is dict:
             message = self.dumps(message)
         asserts.socket_assert(json.loads(message))
         try:
             logger.opt(colors=True).info(f"<fg 128,0,240>{message.replace('<', '&lt;').replace('>', '&gt;')}</>")
+            while self.is_reconnecting: # Cannot use an async.lock() for this b/c doing so would make self.send() block itself.
+                await asyncio.sleep(0.01)
             await self.websocket.send(message)  # Don't use asyncio.create_task() here, or the message could not be sent in order
         except websockets.exceptions.ConnectionClosed as e:
+            self.is_reconnecting = True
             logger.info(f"Connection closed: {e}. Attempting to reconnect...")
             await self.connect()
             logger.info("Reconnected! Attempting to send message again...")
+            self.is_reconnecting = False
             await self.websocket.send(message)
         except Exception as e:
             logger.error(f'Error with websocket.send: {e}')
             await self.connect()
-            logger.info("Reconnected! Attempting to send message again...")
+            logger.info("Reconnected! Attempting to send message again, which is a long shot for non ConnectionClosed Exceptions...")
             await self.websocket.send(message)
 
     async def receive(self):
         """
         Waits in a loop for messages from the websocket server or from the wand queue. Never returns.
         If the connection is closed, reconnect and keep going.
         If an exception is raised, reconnect and keep going.
```

### Comparing `moobius-1.1.5/src/moobius/types.py` & `moobius-1.1.6/src/moobius/types.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius/utils.py` & `moobius-1.1.6/src/moobius/utils.py`

 * *Files identical despite different names*

### Comparing `moobius-1.1.5/src/moobius.egg-info/PKG-INFO` & `moobius-1.1.6/src/moobius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moobius
-Version: 1.1.5
+Version: 1.1.6
 Summary: Moobius Platform SDK
 Author-email: Kevin Kostlan <sdk@moobius.app>
 Project-URL: Homepage, https://github.com/groupultra/sdk-public
 Project-URL: Issues, https://github.com/groupultra/sdk-public/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moobius-1.1.5/src/moobius.egg-info/SOURCES.txt` & `moobius-1.1.6/src/moobius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

