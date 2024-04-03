# Comparing `tmp/omuserver-0.1.9.tar.gz` & `tmp/omuserver-0.2.0.tar.gz`

## Comparing `omuserver-0.1.9.tar` & `omuserver-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.1.9/.python-version
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 omuserver-0.1.9/requirements-dev.lock
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 omuserver-0.1.9/requirements.lock
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 omuserver-0.1.9/.vscode/launch.json
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.1.9/.vscode/settings.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/__init__.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/__main__.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/directories.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/helper.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/__init__.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/extension.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/asset/__init__.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/asset/asset_extension.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/endpoint/__init__.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/endpoint/endpoint_extension.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/message/__init__.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/message/message_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/plugin/__init__.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/plugin/plugin_connection.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/plugin/plugin_extension.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/plugin/plugin_session_connection.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/registry/__init__.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/registry/registry.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/registry/registry_extension.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/server/__init__.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/server/server_extension.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/__init__.py
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/cached_table.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/serialized_table.py
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/server_table.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/session_table_handler.py
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/table_extension.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/adapters/__init__.py
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/adapters/sqlitetable.py
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/extension/table/adapters/tableadapter.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/network/__init__.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/network/network.py
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/network/packet_dispatcher.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/security/__init__.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/security/permission.py
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/security/security.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/security/session_permission.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/server/__init__.py
--rw-r--r--   0        0        0     5815 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/server/omuserver.py
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/server/server.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/session/__init__.py
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/session/aiohttp_connection.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 omuserver-0.1.9/src/omuserver/session/session.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.1.9/test/helper_test.py
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 omuserver-0.1.9/.gitignore
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.1.9/README.md
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 omuserver-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 omuserver-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuserver-0.2.0/.python-version
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 omuserver-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/__init__.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/__main__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/config.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/directories.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/helper.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/__init__.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/extension.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/asset/__init__.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/asset/asset_extension.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/dashboard/__init__.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/dashboard/dashboard_extension.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/endpoint/__init__.py
+-rw-r--r--   0        0        0     6740 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/endpoint/endpoint_extension.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/message/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/message/message_extension.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/permission/__init__.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/permission/permission_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/plugin/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/plugin/plugin_connection.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/plugin/plugin_extension.py
+-rw-r--r--   0        0        0     7848 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/plugin/plugin_loader.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/plugin/plugin_session_connection.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/registry/__init__.py
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/registry/registry.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/registry/registry_extension.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/server/__init__.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/server/server_extension.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/__init__.py
+-rw-r--r--   0        0        0     8225 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/cached_table.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/serialized_table.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/server_table.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/session_table_handler.py
+-rw-r--r--   0        0        0     6805 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/table_extension.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/adapters/__init__.py
+-rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/adapters/sqlitetable.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/extension/table/adapters/tableadapter.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/network/__init__.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/network/network.py
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/network/packet_dispatcher.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/security/__init__.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/security/security.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/server/__init__.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/server/omuserver.py
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/server/server.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/session/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/session/aiohttp_connection.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 omuserver-0.2.0/src/omuserver/session/session.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 omuserver-0.2.0/test/helper_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuserver-0.2.0/.gitignore
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 omuserver-0.2.0/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 omuserver-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 omuserver-0.2.0/PKG-INFO
```

### Comparing `omuserver-0.1.9/src/omuserver/directories.py` & `omuserver-0.2.0/src/omuserver/directories.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,23 @@
 
 @dataclass
 class Directories:
     data: pathlib.Path
     assets: pathlib.Path
     plugins: pathlib.Path
 
+    @classmethod
+    def default(cls):
+        cwd = pathlib.Path.cwd()
+        return Directories(
+            data=cwd / "data",
+            assets=cwd / "assets",
+            plugins=cwd / "plugins",
+        )
+
     def mkdir(self):
         self.data.mkdir(parents=True, exist_ok=True)
         self.assets.mkdir(parents=True, exist_ok=True)
         self.plugins.mkdir(parents=True, exist_ok=True)
 
     def to_json(self):
         return {
@@ -32,16 +41,7 @@
         self.plugins = pathlib.Path(self.plugins)
 
     def __str__(self):
         return f"Directories(data={self.data}, assets={self.assets}, plugins={self.plugins})"
 
     def __repr__(self):
         return str(self)
-
-
-def get_directories():
-    cwd = pathlib.Path.cwd()
-    return Directories(
-        data=cwd / "data",
-        assets=cwd / "assets",
-        plugins=cwd / "plugins",
-    )
```

### Comparing `omuserver-0.1.9/src/omuserver/helper.py` & `omuserver-0.2.0/src/omuserver/helper.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.1.9/src/omuserver/extension/message/message_extension.py` & `omuserver-0.2.0/src/omuserver/extension/message/message_extension.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict
 
 from omu.extension.message.message_extension import (
-    MessageBroadcastPacket,
+    MESSAGE_BROADCAST_PACKET,
+    MESSAGE_LISTEN_PACKET,
     MessageData,
-    MessageListenPacket,
 )
 
 if TYPE_CHECKING:
     from omuserver import Server
     from omuserver.session.session import Session
 
 
@@ -26,20 +26,22 @@
         self.listeners.discard(session)
 
 
 class MessageExtension:
     def __init__(self, server: Server):
         self._server = server
         self._keys: Dict[str, Message] = {}
-        server.packet_dispatcher.register(MessageListenPacket, MessageBroadcastPacket)
+        server.packet_dispatcher.register(
+            MESSAGE_LISTEN_PACKET, MESSAGE_BROADCAST_PACKET
+        )
         server.packet_dispatcher.add_packet_handler(
-            MessageListenPacket, self._on_listen
+            MESSAGE_LISTEN_PACKET, self._on_listen
         )
         server.packet_dispatcher.add_packet_handler(
-            MessageBroadcastPacket, self._on_broadcast
+            MESSAGE_BROADCAST_PACKET, self._on_broadcast
         )
 
     async def _on_register(self, session: Session, key: str) -> None:
         if key in self._keys:
             return
         self._keys[key] = Message(key)
 
@@ -54,8 +56,8 @@
 
     async def _on_broadcast(self, session: Session, data: MessageData) -> None:
         key = data.key
         if key not in self._keys:
             self._keys[key] = Message(key)
         message = self._keys[key]
         for listener in message.listeners:
-            await listener.send(MessageBroadcastPacket, data)
+            await listener.send(MESSAGE_BROADCAST_PACKET, data)
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/plugin/plugin_connection.py` & `omuserver-0.2.0/src/omuserver/extension/plugin/plugin_connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from __future__ import annotations
 
 import asyncio
 
 from omu.network.connection import Connection
-from omu.network.packet import Packet
-from omu.network.packet_mapper import PacketMapper
+from omu.network.packet import Packet, PacketData
+from omu.serializer import Serializable
 
 
 class PluginConnection(Connection):
     def __init__(self) -> None:
         self._connected = False
         self._to_client_queue = asyncio.Queue[Packet]()
         self._to_server_queue = asyncio.Queue[Packet]()
 
     async def connect(self) -> None:
         self._connected = True
 
-    async def receive(self, packet_mapper: PacketMapper) -> Packet:
+    async def receive(self, packet_mapper: Serializable[Packet, PacketData]) -> Packet:
         return await self._to_client_queue.get()
 
     def add_receive(self, packet: Packet) -> None:
         self._to_client_queue.put_nowait(packet)
 
-    async def send(self, packet: Packet, packet_mapper: PacketMapper) -> None:
+    async def send(
+        self, packet: Packet, packet_mapper: Serializable[Packet, PacketData]
+    ) -> None:
         self._to_server_queue.put_nowait(packet)
 
     async def dequeue_to_server_packet(self) -> Packet:
         return await self._to_server_queue.get()
 
     @property
     def closed(self) -> bool:
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/plugin/plugin_extension.py` & `omuserver-0.2.0/src/omuserver/network/network.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,149 @@
 from __future__ import annotations
 
-import asyncio
-import json
-import re
-import subprocess
-import sys
-from importlib.util import find_spec
-from multiprocessing import Process
-from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Dict,
-    NotRequired,
-    Protocol,
-    TypedDict,
-    TypeGuard,
-)
+import socket
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Dict
 
+import psutil
+from aiohttp import web
 from loguru import logger
-from omu import Address
-from omu.network.websocket_connection import WebsocketsConnection
-from omu.plugin import Plugin
-
-from omuserver.extension.plugin.plugin_connection import PluginConnection
-from omuserver.extension.plugin.plugin_session_connection import PluginSessionConnection
-from omuserver.session.session import Session
+from omu import App, Identifier
+from omu.event_emitter import EventEmitter
+from omu.helper import Coro
+from omu.network.packet import PACKET_TYPES, PacketType
+from omu.network.packet.packet_types import ConnectPacket
+
+from omuserver.network.packet_dispatcher import ServerPacketDispatcher
+from omuserver.session import Session
+from omuserver.session.aiohttp_connection import WebsocketsConnection
 
 if TYPE_CHECKING:
     from omuserver.server import Server
 
 
-class PluginModule(Protocol):
-    def get_plugin(self) -> Plugin: ...
+@dataclass(frozen=True)
+class PacketListeners[T]:
+    event_type: PacketType
+    listeners: EventEmitter[Session, T] = field(default_factory=EventEmitter)
 
 
-class PluginMetadata(TypedDict):
-    dependencies: Dict[str, str]
-    module: str
-    isolated: NotRequired[bool]
-
-
-class PluginExtension:
-    def __init__(self, server: Server) -> None:
+class Network:
+    def __init__(
+        self, server: Server, packet_dispatcher: ServerPacketDispatcher
+    ) -> None:
         self._server = server
-        self.plugins: Dict[str, PluginMetadata] = {}
-        server.listeners.start += self.on_server_start
-
-    async def on_server_start(self) -> None:
-        await self._load_plugins()
-
-    async def _load_plugins(self) -> None:
-        for plugin in self._server.directories.plugins.iterdir():
-            if not plugin.is_file():
-                continue
-            if plugin.name.startswith("_"):
-                continue
-            logger.info(f"Loading plugin: {plugin.name}")
-            metadata = self._load_plugin(plugin)
-            self.plugins[metadata["module"]] = metadata
-        await self.install_dependencies()
-        await self.run_plugins()
-
-    def _load_plugin(self, path: Path) -> PluginMetadata:
-        metadata = PluginMetadata(**json.loads(path.read_text()))
-        invalid_dependencies = []
-        for dependency in metadata.get("dependencies", []):
-            if not re.match(r"^[a-zA-Z0-9_-]+$", dependency):
-                invalid_dependencies.append(dependency)
-        if invalid_dependencies:
-            raise ValueError(f"Invalid dependencies in {path}: {invalid_dependencies}")
-        if not re.match(r"^[a-zA-Z0-9_-]+$", metadata["module"]):
-            raise ValueError(f"Invalid module in {path}: {metadata['module']}")
-        return metadata
-
-    async def install_dependencies(self) -> None:
-        # https://stackoverflow.com/a/44210735
-        dependencies: Dict[str, str] = {}
-        for metadata in self.plugins.values():
-            dependencies.update(metadata["dependencies"])
-        to_install: Dict[str, str] = {}
-        for dependency, version in dependencies.items():
-            spec = find_spec(dependency)
-            if spec is None:
-                to_install[dependency] = version
-        if len(to_install) == 0:
+        self._packet_dispatcher = packet_dispatcher
+        self._listeners = NetworkListeners()
+        self._sessions: Dict[str, Session] = {}
+        self._app = web.Application()
+        self.add_websocket_route("/ws")
+        self.register_packet(PACKET_TYPES.CONNECT, PACKET_TYPES.READY)
+        self.listeners.connected += self._packet_dispatcher.process_connection
+
+    def register_packet(self, *packet_types: PacketType) -> None:
+        self._packet_dispatcher.register(*packet_types)
+
+    def add_http_route(
+        self, path: str, handle: Coro[[web.Request], web.StreamResponse]
+    ) -> None:
+        self._app.router.add_get(path, handle)
+
+    def _validate_origin(self, request: web.Request, session: Session) -> None:
+        origin = request.headers.get("origin")
+        if origin is None:
+            return
+        origin_namespace = Identifier.namespace_from_url(origin)
+        namespace = session.app.identifier.namespace
+        if origin_namespace == namespace:
             return
-        logger.info(f"Installing dependencies {to_install}")
-        subprocess.run(
-            [
-                sys.executable,
-                "-m",
-                "pip",
-                "install",
-                *to_install,
-            ],
-            check=True,
-        )
 
-    async def run_plugins(self) -> None:
-        for metadata in self.plugins.values():
-            await self.run_plugin(metadata)
-
-    async def run_plugin(self, metadata: PluginMetadata):
-        if metadata.get("isolated"):
-            process = Process(
-                target=run_plugin_process,
-                args=(
-                    metadata,
-                    Address(
-                        "127.0.0.1",
-                        self._server.address.port,
-                    ),
-                ),
-            )
-            process.start()
+        if self._server.config.strict_origin:
+            raise ValueError(f"Invalid origin: {origin_namespace} != {namespace}")
         else:
-            module = __import__(metadata["module"])
-            if not validate_plugin_module(module):
-                return
-            plugin = module.get_plugin()
-            client = plugin.client
-            connection = PluginConnection()
-            client.network.set_connection(connection)
-            await client.start()
-            session_connection = PluginSessionConnection(connection)
+            logger.warning(f"Invalid origin: {origin_namespace} != {namespace}")
+
+    def add_websocket_route(self, path: str) -> None:
+        async def websocket_handler(request: web.Request) -> web.WebSocketResponse:
+            ws = web.WebSocketResponse()
+            await ws.prepare(request)
+            connection = WebsocketsConnection(ws)
             session = await Session.from_connection(
                 self._server,
-                self._server.packet_dispatcher.packet_mapper,
-                session_connection,
+                self._packet_dispatcher.packet_mapper,
+                connection,
             )
-            self._server.loop.create_task(self._server.network.process_session(session))
+            self._validate_origin(request, session)
+            await self.process_session(session)
+            return ws
+
+        self._app.router.add_get(path, websocket_handler)
+
+    async def process_session(self, session: Session) -> None:
+        if self.is_connected(session.app):
+            logger.warning(f"Session {session.app} already connected")
+            await self._sessions[session.app.key()].disconnect()
+            return
+        self._sessions[session.app.key()] = session
+        session.listeners.disconnected += self.handle_disconnection
+        await self._listeners.connected.emit(session)
+        await session.send(PACKET_TYPES.CONNECT, ConnectPacket(app=session.app))
+        await session.listen()
+
+    def is_connected(self, app: App) -> bool:
+        return app.key() in self._sessions
+
+    async def handle_disconnection(self, session: Session) -> None:
+        if session.app.key() not in self._sessions:
+            return
+        self._sessions.pop(session.app.key())
+        await self._listeners.disconnected.emit(session)
+
+    async def _handle_start(self, app: web.Application) -> None:
+        await self._listeners.start.emit()
+
+    def is_port_available(self) -> bool:
+        try:
+            with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+                s.bind(
+                    (
+                        self._server.address.host or "127.0.0.1",
+                        self._server.address.port,
+                    )
+                )
+                return True
+        except OSError:
+            return False
+
+    def get_process_by_port(self, port: int) -> psutil.Process | None:
+        for connection in psutil.net_connections():
+            if connection.laddr and connection.laddr.port == port:
+                return psutil.Process(connection.pid)
+        return None
+
+    async def start(self) -> None:
+        if not self.is_port_available():
+            process = self.get_process_by_port(self._server.address.port)
+            if process is None:
+                raise OSError(f"Port {self._server.address.port} already in use")
+            port = self._server.address.port
+            name = process.name()
+            pid = process.pid
+            raise OSError(f"Port {port} already in use by {name} ({pid=})")
+        self._app.on_startup.append(self._handle_start)
+        runner = web.AppRunner(self._app)
+        await runner.setup()
+        site = web.TCPSite(
+            runner, host=self._server.address.host, port=self._server.address.port
+        )
+        await site.start()
+
+    @property
+    def listeners(self) -> NetworkListeners:
+        return self._listeners
 
 
-def validate_plugin_module(module: PluginModule) -> TypeGuard[PluginModule]:
-    get_plugin = getattr(module, "get_plugin", None)
-    if get_plugin is None:
-        raise ValueError(f"Plugin {get_plugin} does not have a get_plugin method")
-    return True
-
-
-def handle_exception(loop: asyncio.AbstractEventLoop, context: dict) -> None:
-    logger.error(context["message"])
-    exception = context.get("exception")
-    if exception:
-        raise exception
-
-
-def run_plugin_process(
-    metadata: PluginMetadata,
-    address: Address,
-) -> None:
-    module = __import__(metadata["module"])
-    if not validate_plugin_module(module):
-        raise ValueError(f"Invalid plugin module {metadata['module']}")
-    plugin = module.get_plugin()
-    client = plugin.client
-    connection = WebsocketsConnection(client, address)
-    client.network.set_connection(connection)
-    loop = asyncio.get_event_loop()
-    loop.set_exception_handler(handle_exception)
-    loop.run_until_complete(client.start())
-    loop.run_forever()
-    loop.close()
+class NetworkListeners:
+    def __init__(self) -> None:
+        self.start = EventEmitter()
+        self.connected = EventEmitter[Session]()
+        self.disconnected = EventEmitter[Session]()
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/plugin/plugin_session_connection.py` & `omuserver-0.2.0/src/omuserver/extension/plugin/plugin_session_connection.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.1.9/src/omuserver/extension/registry/registry.py` & `omuserver-0.2.0/src/omuserver/extension/registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Dict
 
 from omu import Identifier
 from omu.extension.registry.registry_extension import (
+    REGISTRY_UPDATE_PACKET,
     RegistryData,
-    RegistryUpdateEvent,
 )
 from omu.serializer import Serializable
 
 from omuserver.server import Server
 from omuserver.session import Session
 
 
@@ -37,25 +37,25 @@
         await self._notify()
 
     async def _notify(self) -> None:
         for listener in self._listeners.values():
             if listener.closed:
                 raise Exception(f"Session {listener.app=} closed")
             await listener.send(
-                RegistryUpdateEvent,
+                REGISTRY_UPDATE_PACKET,
                 RegistryData(key=self._key, existing=self.existing, value=self.data),
             )
 
     async def attach_session(self, session: Session) -> None:
         if session.app.key() in self._listeners:
             del self._listeners[session.app.key()]
         self._listeners[session.app.key()] = session
         session.listeners.disconnected += self.detach_session
         await session.send(
-            RegistryUpdateEvent,
+            REGISTRY_UPDATE_PACKET,
             RegistryData(key=self._key, existing=self.existing, value=self.data),
         )
 
     async def detach_session(self, session: Session) -> None:
         if session.app.key() not in self._listeners:
             raise Exception("Session not attached")
         del self._listeners[session.app.key()]
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/registry/registry_extension.py` & `omuserver-0.2.0/src/omuserver/extension/registry/registry_extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Dict
 
 from omu.extension.registry.registry_extension import (
+    REGISTRY_GET_ENDPOINT,
+    REGISTRY_LISTEN_PACKET,
+    REGISTRY_UPDATE_PACKET,
     RegistryData,
-    RegistryGetEndpoint,
-    RegistryListenEvent,
-    RegistryUpdateEvent,
 )
 from omu.identifier import Identifier
 from omu.serializer import Serializable
 
 from omuserver.session import Session
 
 from .registry import Registry, ServerRegistry
@@ -18,22 +18,24 @@
 if TYPE_CHECKING:
     from omuserver.server import Server
 
 
 class RegistryExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
-        server.packet_dispatcher.register(RegistryListenEvent, RegistryUpdateEvent)
+        server.packet_dispatcher.register(
+            REGISTRY_LISTEN_PACKET, REGISTRY_UPDATE_PACKET
+        )
         server.packet_dispatcher.add_packet_handler(
-            RegistryListenEvent, self._on_listen
+            REGISTRY_LISTEN_PACKET, self._on_listen
         )
         server.packet_dispatcher.add_packet_handler(
-            RegistryUpdateEvent, self._on_update
+            REGISTRY_UPDATE_PACKET, self._on_update
         )
-        server.endpoints.bind_endpoint(RegistryGetEndpoint, self._on_get)
+        server.endpoints.bind_endpoint(REGISTRY_GET_ENDPOINT, self._on_get)
         self.registries: Dict[Identifier, ServerRegistry] = {}
 
     async def _on_listen(self, session: Session, key: str) -> None:
         registry = await self.get(key)
         await registry.attach_session(session)
 
     async def _on_update(self, session: Session, event: RegistryData) -> None:
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/server/server_extension.py` & `omuserver-0.2.0/src/omuserver/extension/server/server_extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
-import asyncio
 from typing import TYPE_CHECKING
 
 from loguru import logger
 from omu.extension.server.server_extension import (
-    AppsTableType,
-    PrintTasksEndpointType,
-    ShutdownEndpointType,
+    APPS_TABLE_TYPE,
+    SHUTDOWN_ENDPOINT_TYPE,
 )
 from omu.serializer import Serializer
 
 from omuserver import __version__
 from omuserver.helper import get_launch_command
 
 if TYPE_CHECKING:
@@ -21,21 +19,15 @@
 
 class ServerExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         server.network.listeners.connected += self.on_connected
         server.network.listeners.disconnected += self.on_disconnected
         server.listeners.start += self.on_start
-        server.endpoints.bind_endpoint(ShutdownEndpointType, self.shutdown)
-        server.endpoints.bind_endpoint(PrintTasksEndpointType, self.print_tasks)
-
-    async def print_tasks(self, session: Session, _) -> None:
-        logger.info("Tasks:")
-        for task in asyncio.all_tasks(self._server.loop):
-            logger.info(task)
+        server.endpoints.bind_endpoint(SHUTDOWN_ENDPOINT_TYPE, self.shutdown)
 
     async def shutdown(self, session: Session, restart: bool = False) -> bool:
         await self._server.shutdown()
         self._server.loop.create_task(self._shutdown(restart))
         return True
 
     async def _shutdown(self, restart: bool = False) -> None:
@@ -44,15 +36,15 @@
             import sys
 
             os.execv(sys.executable, get_launch_command()["args"])
         else:
             self._server.loop.stop()
 
     async def on_start(self) -> None:
-        self.apps = await self._server.tables.register_table(AppsTableType)
+        self.apps = await self._server.tables.register_table(APPS_TABLE_TYPE)
         version = await self._server.registry.create(
             "server:version", __version__, Serializer.json()
         )
         await version.set(__version__)
         directories = await self._server.registry.create(
             "server:directories", self._server.directories.to_json(), Serializer.json()
         )
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/table/cached_table.py` & `omuserver-0.2.0/src/omuserver/extension/table/cached_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 import asyncio
-from typing import TYPE_CHECKING, AsyncIterator, Dict, List
+from typing import TYPE_CHECKING, AsyncGenerator, Dict, List
 
 from omu.extension.table import TableConfig
-from omu.extension.table.table_extension import TableProxyData, TableProxyEvent
+from omu.extension.table.table_extension import TABLE_PROXY_PACKET, TableProxyData
 from omu.identifier import Identifier
 
 from .adapters.tableadapter import TableAdapter
-from .server_table import ServerTable, ServerTableListener
+from .server_table import ServerTable, ServerTableListeners
 from .session_table_handler import SessionTableListener
 
 if TYPE_CHECKING:
     from omuserver.server import Server
     from omuserver.session import Session
 
 
@@ -20,15 +20,15 @@
     def __init__(
         self,
         server: Server,
         identifier: Identifier,
     ):
         self._server = server
         self._identifier = identifier
-        self._listeners: List[ServerTableListener] = []
+        self._listeners = ServerTableListeners()
         self._sessions: Dict[Session, SessionTableListener] = {}
         self._proxy_sessions: Dict[str, Session] = {}
         self._changed = False
         self._proxy_id = 0
         self._save_task: asyncio.Task | None = None
         self._adapter: TableAdapter | None = None
         self._config: TableConfig = {}
@@ -58,25 +58,24 @@
             return
         self._changed = False
         await self._adapter.store()
 
     def attach_session(self, session: Session) -> None:
         if session in self._sessions:
             return
-        handler = SessionTableListener(self._identifier.key(), session)
+        handler = SessionTableListener(self._identifier.key(), session, self)
         self._sessions[session] = handler
-        self.add_listener(handler)
         session.listeners.disconnected += self.handle_disconnection
 
     def detach_session(self, session: Session) -> None:
         if session in self._proxy_sessions:
             del self._proxy_sessions[session.app.key()]
         if session in self._sessions:
             handler = self._sessions.pop(session)
-            self.remove_listener(handler)
+            handler.close()
 
     async def handle_disconnection(self, session: Session) -> None:
         self.detach_session(session)
 
     def attach_proxy_session(self, session: Session) -> None:
         self._proxy_sessions[session.app.key()] = session
 
@@ -110,24 +109,23 @@
     async def add(self, items: Dict[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         if len(self._proxy_sessions) > 0:
             await self.send_proxy_event(items)
             return
         await self._adapter.set_all(items)
-        for listener in self._listeners:
-            await listener.on_add(items)
+        await self._listeners.add(items)
         await self.update_cache(items)
         self.mark_changed()
 
     async def send_proxy_event(self, items: Dict[str, bytes]) -> None:
         session = tuple(self._proxy_sessions.values())[0]
         self._proxy_id += 1
         await session.send(
-            TableProxyEvent,
+            TABLE_PROXY_PACKET,
             TableProxyData(
                 items=items,
                 type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
 
@@ -140,88 +138,90 @@
         session_key = session.app.key()
         index = tuple(self._proxy_sessions.keys()).index(session_key)
         if index == len(self._proxy_sessions) - 1:
             adapter = self._adapter
             if adapter is None:
                 raise Exception("Table not set")
             await adapter.set_all(items)
-            for listener in self._listeners:
-                await listener.on_add(items)
+            await self._listeners.add(items)
             await self.update_cache(items)
             self.mark_changed()
             return 0
         session = tuple(self._proxy_sessions.values())[index + 1]
         await session.send(
-            TableProxyEvent,
+            TABLE_PROXY_PACKET,
             TableProxyData(
                 items=items,
                 type=self._identifier.key(),
                 key=self._proxy_id,
             ),
         )
         return self._proxy_id
 
     async def update(self, items: Dict[str, bytes]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         await self._adapter.set_all(items)
-        for listener in self._listeners:
-            await listener.on_update(items)
+        await self._listeners.update(items)
         await self.update_cache(items)
         self.mark_changed()
 
-    async def remove(self, items: list[str]) -> None:
+    async def remove(self, keys: List[str]) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
-        removed = await self._adapter.get_all(items)
-        await self._adapter.remove_all(items)
-        for key in items:
+        removed = await self._adapter.get_all(keys)
+        await self._adapter.remove_all(keys)
+        for key in keys:
             if key in self._cache:
                 del self._cache[key]
-        for listener in self._listeners:
-            await listener.on_remove(removed)
+        await self._listeners.remove(removed)
         self.mark_changed()
 
     async def clear(self) -> None:
         if self._adapter is None:
             raise Exception("Table not set")
         await self._adapter.clear()
-        for listener in self._listeners:
-            await listener.on_clear()
+        await self._listeners.clear()
         self._cache.clear()
         self.mark_changed()
 
     async def fetch_items(
         self,
         before: int | None = None,
-        after: str | None = None,
+        after: int | None = None,
         cursor: str | None = None,
     ) -> Dict[str, bytes]:
         if self._adapter is None:
             raise Exception("Table not set")
         return await self._adapter.fetch_items(before, after, cursor)
 
-    async def iterate(self) -> AsyncIterator[bytes]:
+    async def fetch_all(self) -> Dict[str, bytes]:
+        if self._adapter is None:
+            raise Exception("Table not set")
+        return await self._adapter.fetch_all()
+
+    async def iterate(self) -> AsyncGenerator[bytes, None]:
         cursor: str | None = None
         while True:
-            items = await self.fetch_items(self._cache_size, cursor)
+            items = await self.fetch_items(
+                before=self._config.get("chunk_size", 100),
+                cursor=cursor,
+            )
             if len(items) == 0:
                 break
             for item in items.values():
                 yield item
             *_, cursor = items.keys()
 
     async def size(self) -> int:
         return len(self._cache)
 
-    def add_listener(self, listener: ServerTableListener) -> None:
-        self._listeners.append(listener)
-
-    def remove_listener(self, listener: ServerTableListener) -> None:
-        self._listeners.remove(listener)
+    @property
+    def listeners(self) -> ServerTableListeners:
+        return self._listeners
 
     async def save_task(self) -> None:
         while self._changed:
             await self.store()
             await asyncio.sleep(30)
 
     def mark_changed(self) -> None:
@@ -235,9 +235,8 @@
     async def update_cache(self, items: Dict[str, bytes]) -> None:
         if self._cache_size is None or self._cache_size <= 0:
             return
         for key, item in items.items():
             self._cache[key] = item
             if len(self._cache) > self._cache_size:
                 del self._cache[next(iter(self._cache))]
-        for listener in self._listeners:
-            await listener.on_cache_update(self._cache)
+        await self._listeners.cache_update(self._cache)
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/table/serialized_table.py` & `omuserver-0.2.0/src/omuserver/extension/table/serialized_table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from typing import AsyncGenerator, Callable, Dict, List, Mapping
 
-from omu.extension.table import Table, TableConfig, TableListener, TableType
+from omu.extension.table import Table, TableConfig, TableListeners, TableType
 from omu.helper import AsyncCallback, Coro
 from omu.interface import Keyable
 from omu.serializer import Serializable
 
-from .server_table import ServerTable, ServerTableListener
+from .server_table import ServerTable
 
 
 class SerializeAdapter[T: Keyable](Mapping[str, T]):
     def __init__(self, cache: Mapping[str, bytes], serializer: Serializable[T, bytes]):
         self._cache = cache
         self._serializer = serializer
 
     def __getitem__(self, key: str) -> T:
         return self._serializer.deserialize(self._cache[key])
 
 
-class SerializedTable[T: Keyable](Table[T], ServerTableListener):
+class SerializedTable[T: Keyable](Table[T]):
     def __init__(self, table: ServerTable, type: TableType[T]):
         self._table = table
         self._type = type
-        self._listeners: List[TableListener[T]] = []
+        self._listeners = TableListeners[T](self)
         self._proxies: List[Coro[[T], T | None]] = []
         self._chunk_size = 100
         self.key = type.identifier.key()
-        table.add_listener(self)
+        table.listeners.cache_update += self.on_cache_update
+        table.listeners.add += self.on_add
+        table.listeners.update += self.on_update
+        table.listeners.remove += self.on_remove
+        table.listeners.clear += self.on_clear
 
     @property
     def cache(self) -> Mapping[str, T]:
         return SerializeAdapter(self._table.cache, self._type.serializer)
 
     def set_config(self, config: TableConfig) -> None:
         self._table.set_config(config)
@@ -64,14 +68,18 @@
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
     ) -> Dict[str, T]:
         items = await self._table.fetch_items(before, after, cursor)
         return self._parse_items(items)
 
+    async def fetch_all(self) -> Dict[str, T]:
+        items = await self._table.fetch_all()
+        return self._parse_items(items)
+
     async def iterate(
         self,
         backward: bool = False,
         cursor: str | None = None,
     ) -> AsyncGenerator[T, None]:
         items = await self.fetch_items(
             before=self._chunk_size if backward else None,
@@ -90,51 +98,44 @@
             for item in items.values():
                 yield item
             items.pop(cursor, None)
 
     async def size(self) -> int:
         return await self._table.size()
 
-    def add_listener(self, listener: TableListener[T]) -> None:
-        self._listeners.append(listener)
-        self._listening = True
-
-    def remove_listener(self, listener: TableListener[T]) -> None:
-        self._listeners.remove(listener)
+    @property
+    def listeners(self) -> TableListeners[T]:
+        return self._listeners
 
     def listen(
-        self, callback: AsyncCallback[Mapping[str, T]] | None = None
+        self, listener: AsyncCallback[Mapping[str, T]] | None = None
     ) -> Callable[[], None]:
         self._listening = True
-        listener = TableListener(on_cache_update=callback)
-        self._listeners.append(listener)
-        return lambda: self._listeners.remove(listener)
+        if listener:
+            self._listeners.cache_update += listener
+            return lambda: self._listeners.cache_update.unsubscribe(listener)
+        return lambda: None
 
     async def on_add(self, items: Dict[str, bytes]) -> None:
         _items = self._parse_items(items)
-        for listener in self._listeners:
-            await listener.on_add(_items)
+        await self._listeners.add(_items)
 
     async def on_update(self, items: Dict[str, bytes]) -> None:
         _items = self._parse_items(items)
-        for listener in self._listeners:
-            await listener.on_update(_items)
+        await self._listeners.update(_items)
 
     async def on_remove(self, items: Dict[str, bytes]) -> None:
         _items = self._parse_items(items)
-        for listener in self._listeners:
-            await listener.on_remove(_items)
+        await self._listeners.remove(_items)
 
     async def on_clear(self) -> None:
-        for listener in self._listeners:
-            await listener.on_clear()
+        await self._listeners.clear()
 
     async def on_cache_update(self, cache: Dict[str, bytes]) -> None:
-        for listener in self._listeners:
-            await listener.on_cache_update(self._parse_items(cache))
+        await self._listeners.cache_update(self._parse_items(cache))
 
     def proxy(self, callback: Coro[[T], T | None]) -> Callable[[], None]:
         raise NotImplementedError
 
     def _parse_items(self, items: Dict[str, bytes]) -> Dict[str, T]:
         parsed: Dict[str, T] = {}
         for key, item in items.items():
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/table/server_table.py` & `omuserver-0.2.0/src/omuserver/extension/table/server_table.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 import abc
-from typing import TYPE_CHECKING, AsyncIterator, Dict, List, Union
+from typing import TYPE_CHECKING, AsyncGenerator, Dict, List, Union
+
+from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
     from omu.extension.table import TableConfig
 
     from omuserver.session import Session
 
     from .adapters.tableadapter import TableAdapter
@@ -71,29 +73,27 @@
         self,
         before: int | None = None,
         after: int | None = None,
         cursor: str | None = None,
     ) -> Dict[str, bytes]: ...
 
     @abc.abstractmethod
-    async def iterate(self) -> AsyncIterator[bytes]: ...
+    async def fetch_all(self) -> Dict[str, bytes]: ...
 
     @abc.abstractmethod
-    async def size(self) -> int: ...
+    async def iterate(self) -> AsyncGenerator[bytes, None]: ...
 
     @abc.abstractmethod
-    def add_listener(self, listener: ServerTableListener) -> None: ...
+    async def size(self) -> int: ...
 
+    @property
     @abc.abstractmethod
-    def remove_listener(self, listener: ServerTableListener) -> None: ...
-
-
-class ServerTableListener:
-    async def on_add(self, items: Dict[str, bytes]) -> None: ...
-
-    async def on_update(self, items: Dict[str, bytes]) -> None: ...
-
-    async def on_remove(self, items: Dict[str, bytes]) -> None: ...
+    def listeners(self) -> ServerTableListeners: ...
 
-    async def on_clear(self) -> None: ...
 
-    async def on_cache_update(self, cache: Dict[str, bytes]) -> None: ...
+class ServerTableListeners:
+    def __init__(self) -> None:
+        self.add: EventEmitter[Dict[str, bytes]] = EventEmitter()
+        self.update: EventEmitter[Dict[str, bytes]] = EventEmitter()
+        self.remove: EventEmitter[Dict[str, bytes]] = EventEmitter()
+        self.clear: EventEmitter[[]] = EventEmitter()
+        self.cache_update: EventEmitter[Dict[str, bytes]] = EventEmitter()
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/table/table_extension.py` & `omuserver-0.2.0/src/omuserver/extension/table/table_extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Dict, List
 
 from omu.extension.table import Table, TableType
 from omu.extension.table.table_extension import (
+    TABLE_CONFIG_SET_PACKET,
+    TABLE_ITEM_ADD_PACKET,
+    TABLE_ITEM_CLEAR_PACKET,
+    TABLE_ITEM_FETCH_ALL_ENDPOINT,
+    TABLE_ITEM_FETCH_ENDPOINT,
+    TABLE_ITEM_GET_ENDPOINT,
+    TABLE_ITEM_REMOVE_EVENT,
+    TABLE_ITEM_SIZE_ENDPOINT,
+    TABLE_ITEM_UPDATE_PACKET,
+    TABLE_LISTEN_PACKET,
+    TABLE_PROXY_ENDPOINT,
+    TABLE_PROXY_LISTEN_PACKET,
+    TABLE_PROXY_PACKET,
     SetConfigReq,
-    TableConfigSetEvent,
     TableEventData,
     TableFetchReq,
-    TableItemAddEvent,
-    TableItemClearEvent,
-    TableItemFetchEndpoint,
-    TableItemGetEndpoint,
-    TableItemRemoveEvent,
     TableItemsData,
-    TableItemSizeEndpoint,
-    TableItemUpdateEvent,
     TableKeysData,
-    TableListenEvent,
     TableProxyData,
-    TableProxyEndpoint,
-    TableProxyEvent,
-    TableProxyListenEvent,
 )
 from omu.identifier import Identifier
 from omu.interface import Keyable
 
 from omuserver.extension.table.serialized_table import SerializedTable
 from omuserver.server import Server
 from omuserver.session import Session
@@ -39,50 +40,55 @@
 
 class TableExtension:
     def __init__(self, server: Server) -> None:
         self._server = server
         self._tables: Dict[Identifier, ServerTable] = {}
         self._adapters: List[TableAdapter] = []
         server.packet_dispatcher.register(
-            TableConfigSetEvent,
-            TableListenEvent,
-            TableProxyListenEvent,
-            TableProxyEvent,
-            TableItemAddEvent,
-            TableItemUpdateEvent,
-            TableItemRemoveEvent,
-            TableItemClearEvent,
+            TABLE_CONFIG_SET_PACKET,
+            TABLE_LISTEN_PACKET,
+            TABLE_PROXY_LISTEN_PACKET,
+            TABLE_PROXY_PACKET,
+            TABLE_ITEM_ADD_PACKET,
+            TABLE_ITEM_UPDATE_PACKET,
+            TABLE_ITEM_REMOVE_EVENT,
+            TABLE_ITEM_CLEAR_PACKET,
         )
         server.packet_dispatcher.add_packet_handler(
-            TableConfigSetEvent, self._on_table_set_config
+            TABLE_CONFIG_SET_PACKET, self._on_table_set_config
         )
         server.packet_dispatcher.add_packet_handler(
-            TableListenEvent, self._on_table_listen
+            TABLE_LISTEN_PACKET, self._on_table_listen
         )
         server.packet_dispatcher.add_packet_handler(
-            TableProxyListenEvent, self._on_table_proxy_listen
+            TABLE_PROXY_LISTEN_PACKET, self._on_table_proxy_listen
         )
         server.packet_dispatcher.add_packet_handler(
-            TableItemAddEvent, self._on_table_item_add
+            TABLE_ITEM_ADD_PACKET, self._on_table_item_add
         )
         server.packet_dispatcher.add_packet_handler(
-            TableItemUpdateEvent, self._on_table_item_update
+            TABLE_ITEM_UPDATE_PACKET, self._on_table_item_update
         )
         server.packet_dispatcher.add_packet_handler(
-            TableItemRemoveEvent, self._on_table_item_remove
+            TABLE_ITEM_REMOVE_EVENT, self._on_table_item_remove
         )
         server.packet_dispatcher.add_packet_handler(
-            TableItemClearEvent, self._on_table_item_clear
+            TABLE_ITEM_CLEAR_PACKET, self._on_table_item_clear
         )
-        server.endpoints.bind_endpoint(TableItemGetEndpoint, self._on_table_item_get)
+        server.endpoints.bind_endpoint(TABLE_ITEM_GET_ENDPOINT, self._on_table_item_get)
         server.endpoints.bind_endpoint(
-            TableItemFetchEndpoint, self._on_table_item_fetch
+            TABLE_ITEM_FETCH_ENDPOINT, self._on_table_item_fetch
         )
-        server.endpoints.bind_endpoint(TableItemSizeEndpoint, self._on_table_item_size)
-        server.endpoints.bind_endpoint(TableProxyEndpoint, self._on_table_proxy)
+        server.endpoints.bind_endpoint(
+            TABLE_ITEM_FETCH_ALL_ENDPOINT, self._on_table_item_fetch_all
+        )
+        server.endpoints.bind_endpoint(
+            TABLE_ITEM_SIZE_ENDPOINT, self._on_table_item_size
+        )
+        server.endpoints.bind_endpoint(TABLE_PROXY_ENDPOINT, self._on_table_proxy)
         server.listeners.stop += self.on_server_stop
 
     async def _on_table_item_get(
         self, session: Session, req: TableKeysData
     ) -> TableItemsData:
         table = await self.get_table(req["type"])
         items = await table.get_all(req["keys"])
@@ -101,14 +107,24 @@
             cursor=req.get("cursor"),
         )
         return TableItemsData(
             type=req["type"],
             items=items,
         )
 
+    async def _on_table_item_fetch_all(
+        self, session: Session, req: TableEventData
+    ) -> TableItemsData:
+        table = await self.get_table(req["type"])
+        items = await table.fetch_all()
+        return TableItemsData(
+            type=req["type"],
+            items=items,
+        )
+
     async def _on_table_item_size(self, session: Session, req: TableEventData) -> int:
         table = await self.get_table(req["type"])
         return await table.size()
 
     async def _on_table_set_config(
         self, session: Session, config: SetConfigReq
     ) -> None:
```

### Comparing `omuserver-0.1.9/src/omuserver/extension/table/adapters/sqlitetable.py` & `omuserver-0.2.0/src/omuserver/extension/table/adapters/sqlitetable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import sqlite3
 from pathlib import Path
-from typing import Dict, Tuple
+from typing import Dict, Mapping, Tuple
 
 from .tableadapter import TableAdapter
 
 
 class SqliteTableAdapter(TableAdapter):
     def __init__(self, path: Path) -> None:
         self._path = path
@@ -48,15 +48,15 @@
 
     async def set(self, key: str, value: bytes) -> None:
         self._conn.execute(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
             (key, (value)),
         )
 
-    async def set_all(self, items: Dict[str, bytes]) -> None:
+    async def set_all(self, items: Mapping[str, bytes]) -> None:
         query = [(key, value) for key, value in items.items()]
         self._conn.executemany(
             "INSERT OR REPLACE INTO data (key, value) VALUES (?, ?)",
             query,
         )
 
     async def remove(self, key: str) -> None:
@@ -106,14 +106,18 @@
                 _cursor = self._conn.execute(
                     "SELECT id, key, value FROM data WHERE id >= ? ORDER BY id LIMIT ?",
                     (cursor_id, after),
                 )
             items.update({row[0]: (row[1], (row[2])) for row in _cursor.fetchall()})
         return {key: value for _, (key, value) in sorted(items.items(), reverse=True)}
 
+    async def fetch_all(self) -> Dict[str, bytes]:
+        _cursor = self._conn.execute("SELECT key, value FROM data")
+        return {row[0]: (row[1]) for row in _cursor.fetchall()}
+
     async def first(self) -> str | None:
         _cursor = self._conn.execute("SELECT key FROM data ORDER BY id LIMIT 1")
         row = _cursor.fetchone()
         if row is None:
             return None
         return row[0]
```

### Comparing `omuserver-0.1.9/src/omuserver/network/network.py` & `omuserver-0.2.0/src/omuserver/session/session.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,117 +1,107 @@
 from __future__ import annotations
 
-import socket
-from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Dict
-
-from aiohttp import web
-from loguru import logger
-from omu import App
+import abc
+import asyncio
+from typing import TYPE_CHECKING
+
 from omu.event_emitter import EventEmitter
-from omu.helper import Coro
-from omu.network.packet import PACKET_TYPES, PacketType
+from omu.network.packet import PACKET_TYPES, Packet, PacketType
 from omu.network.packet.packet_types import ConnectPacket
+from omu.network.packet_mapper import PacketMapper
 
-from omuserver.network.packet_dispatcher import ServerPacketDispatcher
-from omuserver.session import Session
-from omuserver.session.aiohttp_connection import WebsocketsConnection
+from omuserver.server.server import Server
 
 if TYPE_CHECKING:
-    from omuserver.server import Server
+    from omu import App
 
 
-@dataclass(frozen=True)
-class PacketListeners[T]:
-    event_type: PacketType
-    listeners: EventEmitter[Session, T] = field(default_factory=EventEmitter)
+class SessionConnection(abc.ABC):
+    @abc.abstractmethod
+    async def send(self, packet: Packet, packet_mapper: PacketMapper) -> None: ...
 
+    @abc.abstractmethod
+    async def receive(self, packet_mapper: PacketMapper) -> Packet | None: ...
 
-class Network:
-    def __init__(
-        self, server: Server, packet_dispatcher: ServerPacketDispatcher
-    ) -> None:
-        self._server = server
-        self._packet_dispatcher = packet_dispatcher
-        self._listeners = NetworkListeners()
-        self._sessions: Dict[str, Session] = {}
-        self._app = web.Application()
-        self.add_websocket_route("/ws")
-        self.register_packet(PACKET_TYPES.CONNECT, PACKET_TYPES.READY)
-        self.listeners.connected += self._packet_dispatcher.process_connection
+    @abc.abstractmethod
+    async def close(self) -> None: ...
 
-    def register_packet(self, *packet_types: PacketType) -> None:
-        self._packet_dispatcher.register(*packet_types)
+    @property
+    @abc.abstractmethod
+    def closed(self) -> bool: ...
 
-    def add_http_route(
-        self, path: str, handle: Coro[[web.Request], web.StreamResponse]
-    ) -> None:
-        self._app.router.add_get(path, handle)
 
-    def add_websocket_route(self, path: str) -> None:
-        async def websocket_handler(request: web.Request) -> web.WebSocketResponse:
-            ws = web.WebSocketResponse()
-            await ws.prepare(request)
-            connection = WebsocketsConnection(ws)
-            session = await Session.from_connection(
-                self._server,
-                self._packet_dispatcher.packet_mapper,
-                connection,
+class Session:
+    def __init__(
+        self,
+        packet_mapper: PacketMapper,
+        app: App,
+        token: str,
+        connection: SessionConnection,
+    ) -> None:
+        self.serializer = packet_mapper
+        self.app = app
+        self.token = token
+        self._connection = connection
+        self._listeners = SessionListeners()
+
+    @classmethod
+    async def from_connection(
+        cls,
+        server: Server,
+        packet_mapper: PacketMapper,
+        connection: SessionConnection,
+    ) -> Session:
+        packet = await connection.receive(packet_mapper)
+        if packet is None:
+            raise RuntimeError("Socket closed before connect")
+        if packet.type != PACKET_TYPES.CONNECT:
+            raise RuntimeError(
+                f"Expected {PACKET_TYPES.CONNECT.identifier} but got {packet.type}"
             )
-            await self.process_session(session)
-            return ws
-
-        self._app.router.add_get(path, websocket_handler)
+        if not isinstance(packet.data, ConnectPacket):
+            raise RuntimeError(f"Invalid packet data: {packet.data}")
+        event = packet.data
+        token = event.token
+        if token is None:
+            token = await server.security.generate_app_token(event.app)
+        else:
+            verified = await server.security.validate_app_token(event.app, token)
+            if not verified:
+                raise RuntimeError("Invalid token")
+        session = Session(packet_mapper, event.app, token, connection)
+        await session.send(PACKET_TYPES.TOKEN, token)
+        return session
 
-    async def process_session(self, session: Session) -> None:
-        if self.is_connected(session.app):
-            logger.warning(f"Session {session.app} already connected")
-            await self._sessions[session.app.key()].disconnect()
-            return
-        self._sessions[session.app.key()] = session
-        session.listeners.disconnected += self.handle_disconnection
-        await self._listeners.connected.emit(session)
-        await session.send(PACKET_TYPES.CONNECT, ConnectPacket(app=session.app))
-        await session.listen()
-
-    def is_connected(self, app: App) -> bool:
-        return app.key() in self._sessions
-
-    async def handle_disconnection(self, session: Session) -> None:
-        if session.app.key() not in self._sessions:
-            return
-        self._sessions.pop(session.app.key())
-        await self._listeners.disconnected.emit(session)
+    @property
+    def closed(self) -> bool:
+        return self._connection.closed
 
-    async def _handle_start(self, app: web.Application) -> None:
-        await self._listeners.start.emit()
+    async def disconnect(self) -> None:
+        await self._connection.close()
+        await self._listeners.disconnected.emit(self)
 
-    def is_port_available(self) -> bool:
+    async def listen(self) -> None:
         try:
-            socket_connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-            result = socket_connection.connect_ex(("127.0.0.1", 80))
-            socket_connection.close()
-            return result != 0
-        except OSError:
-            return False
-
-    async def start(self) -> None:
-        if not self.is_port_available():
-            raise OSError(f"Port {self._server.address.port} already in use")
-        self._app.on_startup.append(self._handle_start)
-        runner = web.AppRunner(self._app)
-        await runner.setup()
-        site = web.TCPSite(
-            runner, host=self._server.address.host, port=self._server.address.port
-        )
-        await site.start()
+            while not self._connection.closed:
+                packet = await self._connection.receive(self.serializer)
+                if packet is None:
+                    break
+                asyncio.create_task(self._dispatch_packet(packet))
+        finally:
+            await self.disconnect()
+
+    async def _dispatch_packet(self, packet: Packet) -> None:
+        await self._listeners.packet.emit(self, packet)
+
+    async def send[T](self, packet_type: PacketType[T], data: T) -> None:
+        await self._connection.send(Packet(packet_type, data), self.serializer)
 
     @property
-    def listeners(self) -> NetworkListeners:
+    def listeners(self) -> SessionListeners:
         return self._listeners
 
 
-class NetworkListeners:
+class SessionListeners:
     def __init__(self) -> None:
-        self.start = EventEmitter()
-        self.connected = EventEmitter[Session]()
+        self.packet = EventEmitter[Session, Packet]()
         self.disconnected = EventEmitter[Session]()
```

### Comparing `omuserver-0.1.9/src/omuserver/network/packet_dispatcher.py` & `omuserver-0.2.0/src/omuserver/network/packet_dispatcher.py`

 * *Files identical despite different names*

### Comparing `omuserver-0.1.9/src/omuserver/server/omuserver.py` & `omuserver-0.2.0/src/omuserver/server/omuserver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 import asyncio
 import json
-from typing import Optional
+from typing import Mapping, Optional
 
 import aiohttp
 from aiohttp import web
 from loguru import logger
+from omu import Identifier
 from omu.network import Address
 
 from omuserver import __version__
-from omuserver.directories import Directories, get_directories
+from omuserver.config import Config
+from omuserver.directories import Directories
 from omuserver.extension.asset import AssetExtension
+from omuserver.extension.dashboard import DashboardExtension
 from omuserver.extension.endpoint import EndpointExtension
 from omuserver.extension.message import MessageExtension
+from omuserver.extension.permission import PermissionExtension
 from omuserver.extension.plugin import PluginExtension
 from omuserver.extension.registry import RegistryExtension
 from omuserver.extension.server import ServerExtension
 from omuserver.extension.table import TableExtension
 from omuserver.helper import safe_path_join
 from omuserver.network import Network
 from omuserver.network.packet_dispatcher import ServerPacketDispatcher
-from omuserver.security.security import ServerSecurity
+from omuserver.security.security import Security, ServerAuthenticator
 
 from .server import Server, ServerListeners
 
 client = aiohttp.ClientSession(
     headers={
         "User-Agent": json.dumps(
             [
@@ -37,36 +41,38 @@
     }
 )
 
 
 class OmuServer(Server):
     def __init__(
         self,
-        address: Address,
-        directories: Optional[Directories] = None,
+        config: Config,
         loop: Optional[asyncio.AbstractEventLoop] = None,
     ) -> None:
+        self._config = config
         self._loop = loop or asyncio.get_event_loop()
-        self._address = address
+        self._address = config.address
         self._listeners = ServerListeners()
-        self._directories = directories or get_directories()
+        self._directories = config.directories
         self._directories.mkdir()
         self._packet_dispatcher = ServerPacketDispatcher()
         self._network = Network(self, self._packet_dispatcher)
         self._network.listeners.start += self._handle_network_start
         self._network.add_http_route("/proxy", self._handle_proxy)
-        self._network.add_http_route("/assets", self._handle_assets)
-        self._security = ServerSecurity(self)
+        self._network.add_http_route("/asset", self._handle_assets)
+        self._security = ServerAuthenticator(self)
         self._running = False
-        self._endpoint = EndpointExtension(self)
+        self._endpoints = EndpointExtension(self)
+        self._dashboard = DashboardExtension(self)
+        self._permissions = PermissionExtension(self)
         self._tables = TableExtension(self)
         self._server = ServerExtension(self)
         self._registry = RegistryExtension(self)
-        self._message = MessageExtension(self)
-        self._plugin = PluginExtension(self)
+        self._messages = MessageExtension(self)
+        self._plugins = PluginExtension(self)
         self._assets = AssetExtension(self)
 
     async def _handle_proxy(self, request: web.Request) -> web.StreamResponse:
         url = request.query.get("url")
         no_cache = bool(request.query.get("no_cache"))
         if not url:
             return web.Response(status=400)
@@ -85,17 +91,19 @@
         except aiohttp.ClientResponseError as e:
             return web.Response(status=e.status, text=e.message)
         except Exception as e:
             logger.error(e)
             return web.Response(status=500)
 
     async def _handle_assets(self, request: web.Request) -> web.StreamResponse:
-        path = request.query.get("path")
-        if not path:
+        id = request.query.get("id")
+        if not id:
             return web.Response(status=400)
+        identifier = Identifier.from_key(id)
+        path = identifier.to_path()
         try:
             path = safe_path_join(self._directories.assets, path)
 
             if not path.exists():
                 return web.Response(status=404)
             return web.FileResponse(path)
         except Exception as e:
@@ -109,42 +117,53 @@
             loop.set_exception_handler(self.handle_exception)
             loop.create_task(self.start())
             loop.run_forever()
         finally:
             loop.close()
             asyncio.run(self.shutdown())
 
-    def handle_exception(self, loop: asyncio.AbstractEventLoop, context: dict) -> None:
+    def handle_exception(
+        self, loop: asyncio.AbstractEventLoop, context: Mapping
+    ) -> None:
         logger.error(context["message"])
         exception = context.get("exception")
         if exception:
             raise exception
 
+    async def _handle_network_start(self) -> None:
+        logger.info(f"Listening on {self.address}")
+        try:
+            await self._listeners.start()
+        except Exception as e:
+            await self.shutdown()
+            self.loop.stop()
+            raise e
+
     async def start(self) -> None:
         self._running = True
         await self._network.start()
 
     async def shutdown(self) -> None:
         self._running = False
         await self._listeners.stop()
 
-    async def _handle_network_start(self) -> None:
-        logger.info(f"Listening on {self.address}")
-        await self._listeners.start()
+    @property
+    def config(self) -> Config:
+        return self._config
 
     @property
     def loop(self) -> asyncio.AbstractEventLoop:
         return self._loop
 
     @property
     def address(self) -> Address:
         return self._address
 
     @property
-    def security(self) -> ServerSecurity:
+    def security(self) -> Security:
         return self._security
 
     @property
     def directories(self) -> Directories:
         return self._directories
 
     @property
@@ -153,31 +172,39 @@
 
     @property
     def packet_dispatcher(self) -> ServerPacketDispatcher:
         return self._packet_dispatcher
 
     @property
     def endpoints(self) -> EndpointExtension:
-        return self._endpoint
+        return self._endpoints
+
+    @property
+    def dashboard(self) -> DashboardExtension:
+        return self._dashboard
+
+    @property
+    def permissions(self) -> PermissionExtension:
+        return self._permissions
 
     @property
     def tables(self) -> TableExtension:
         return self._tables
 
     @property
     def registry(self) -> RegistryExtension:
         return self._registry
 
     @property
     def messages(self) -> MessageExtension:
-        return self._message
+        return self._messages
 
     @property
     def plugins(self) -> PluginExtension:
-        return self._plugin
+        return self._plugins
 
     @property
     def assets(self) -> AssetExtension:
         return self._assets
 
     @property
     def running(self) -> bool:
```

### Comparing `omuserver-0.1.9/src/omuserver/server/server.py` & `omuserver-0.2.0/src/omuserver/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,22 @@
 from typing import TYPE_CHECKING
 
 from omu.event_emitter import EventEmitter
 
 if TYPE_CHECKING:
     from omu.network import Address
 
+    from omuserver.config import Config
     from omuserver.directories import Directories
-    from omuserver.extension.asset.asset_extension import AssetExtension
+    from omuserver.extension.asset import AssetExtension
+    from omuserver.extension.dashboard import DashboardExtension
     from omuserver.extension.endpoint import EndpointExtension
-    from omuserver.extension.message.message_extension import MessageExtension
-    from omuserver.extension.plugin.plugin_extension import PluginExtension
+    from omuserver.extension.message import MessageExtension
+    from omuserver.extension.permission import PermissionExtension
+    from omuserver.extension.plugin import PluginExtension
     from omuserver.extension.registry import RegistryExtension
     from omuserver.extension.table import TableExtension
     from omuserver.network import Network
     from omuserver.network.packet_dispatcher import ServerPacketDispatcher
     from omuserver.security import Security
 
 
@@ -26,14 +29,18 @@
         self.start = EventEmitter()
         self.stop = EventEmitter()
 
 
 class Server(abc.ABC):
     @property
     @abc.abstractmethod
+    def config(self) -> Config: ...
+
+    @property
+    @abc.abstractmethod
     def loop(self) -> asyncio.AbstractEventLoop: ...
 
     @property
     @abc.abstractmethod
     def address(self) -> Address: ...
 
     @property
@@ -50,18 +57,26 @@
 
     @property
     @abc.abstractmethod
     def packet_dispatcher(self) -> ServerPacketDispatcher: ...
 
     @property
     @abc.abstractmethod
+    def permissions(self) -> PermissionExtension: ...
+
+    @property
+    @abc.abstractmethod
     def endpoints(self) -> EndpointExtension: ...
 
     @property
     @abc.abstractmethod
+    def dashboard(self) -> DashboardExtension: ...
+
+    @property
+    @abc.abstractmethod
     def tables(self) -> TableExtension: ...
 
     @property
     @abc.abstractmethod
     def registry(self) -> RegistryExtension: ...
 
     @property
```

### Comparing `omuserver-0.1.9/src/omuserver/session/aiohttp_connection.py` & `omuserver-0.2.0/src/omuserver/session/aiohttp_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,35 @@
 
 from aiohttp import web
 from loguru import logger
 from omu.network.bytebuffer import ByteReader, ByteWriter
 from omu.network.packet import Packet, PacketData
 from omu.network.packet_mapper import PacketMapper
 
-from omuserver.security import Permission
-
 from .session import SessionConnection
 
 
 class WebsocketsConnection(SessionConnection):
     def __init__(self, socket: web.WebSocketResponse) -> None:
         self.socket = socket
 
     @property
     def closed(self) -> bool:
         return self.socket.closed
 
-    @property
-    def permissions(self) -> Permission:
-        return self.permissions
-
-    async def receive(self, packet_mapper: PacketMapper) -> Packet:
+    async def receive(self, packet_mapper: PacketMapper) -> Packet | None:
         msg = await self.socket.receive()
         if msg.type in {
             web.WSMsgType.CLOSE,
-            web.WSMsgType.ERROR,
-            web.WSMsgType.CLOSED,
             web.WSMsgType.CLOSING,
+            web.WSMsgType.CLOSED,
         }:
-            raise RuntimeError(f"Socket {msg.type.name.lower()}")
+            return None
+        if msg.type != web.WSMsgType.BINARY:
+            raise RuntimeError(f"Unknown message type {msg.type}")
 
         if msg.data is None:
             raise RuntimeError("Received empty message")
         if msg.type == web.WSMsgType.TEXT:
             raise RuntimeError("Received text message")
         elif msg.type == web.WSMsgType.BINARY:
             with ByteReader(msg.data) as reader:
```

### Comparing `omuserver-0.1.9/pyproject.toml` & `omuserver-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 [project]
 name = "omuserver"
-version = "0.1.9"
+version = "0.2.0"
 description = "Add your description here"
 authors = [
     { name = "am230", email = "111672334+am230@users.noreply.github.com" },
 ]
 dependencies = [
     "sqlitedict>=2.1.0",
     "click>=8.1.7",
     "aiosqlite>=0.19.0",
     "loguru>=0.7.2",
     "omu>=0.1.4",
     "pip>=24.0",
     "aiohttp>=3.9.3",
+    "packaging>=24.0",
+    "psutil>=5.9.8",
 ]
 readme = "README.md"
 requires-python = ">= 3.12"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

