# Comparing `tmp/omuplugin_onecomme-0.1.9.tar.gz` & `tmp/omuplugin_onecomme-0.2.0.tar.gz`

## Comparing `omuplugin_onecomme-0.1.9.tar` & `omuplugin_onecomme-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/.python-version
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/src/omuplugin_onecomme/__init__.py
--rw-r--r--   0        0        0     5832 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/src/omuplugin_onecomme/plugin.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/README.md
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/.python-version
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/src/omuplugin_onecomme/__init__.py
+-rw-r--r--   0        0        0     5904 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/src/omuplugin_onecomme/plugin.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/README.md
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 omuplugin_onecomme-0.2.0/PKG-INFO
```

### Comparing `omuplugin_onecomme-0.1.9/src/omuplugin_onecomme/plugin.py` & `omuplugin_onecomme-0.2.0/src/omuplugin_onecomme/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from __future__ import annotations
 
 import asyncio
 from typing import Dict, List, Set, TypedDict
 
 from aiohttp import web
 from loguru import logger
+from omu.identifier import Identifier
 from omuchat import App, Client, events, model
 
+IDENTIFIER = Identifier("cc.omuchat", "plugin-onesync")
 APP = App(
-    name="plugin-onesync",
-    group="cc.omuchat",
+    IDENTIFIER,
     version="0.1.0",
 )
 client = Client(APP)
 app = web.Application()
 
 
 class Color(TypedDict):
@@ -91,32 +92,33 @@
             )
         elif isinstance(component, model.content.Parent):
             stack.extend(component.get_children())
     return "".join(parts)
 
 
 async def to_comment(message: model.Message) -> Comment | None:
-    room = await client.rooms.get(message.room_id)
-    author = message.author_id and await client.authors.get(message.author_id)
-    if not room or not room.metadata or not author:
+    room = await client.chat.rooms.get(message.room_id)
+    author = message.author_id and await client.chat.authors.get(message.author_id)
+    if not room or not author:
         return None
+    metadata = room.metadata or {}
     badges = []
     for badge in author.roles:
         if badge.icon_url:
             badges.append(
                 Badge(
                     label=badge.name,
                     url=badge.icon_url,
                 )
             )
     return Comment(
         id=room.key(),
         service=room.provider_id,
-        name=room.metadata.get("title", ""),
-        url=room.metadata.get("url", ""),
+        name=metadata.get("title", ""),
+        url=metadata.get("url", ""),
         color={"r": 190, "g": 44, "b": 255},
         data=CommentData(
             id=message.key(),
             liveId=room.id,
             userId=author.key(),
             name=author.name,
             screenName=author.name,
@@ -130,16 +132,16 @@
             displayName=author.name,
             originalProfileImage=author.avatar_url or "",
             isFirstTime=False,
         ),
         meta={"no": 1, "tc": 1},
         serviceData=CommentServiceData(
             id=room.key(),
-            name=room.metadata.get("title", ""),
-            url=room.metadata.get("url", ""),
+            name=metadata.get("title", ""),
+            url=metadata.get("url", ""),
             write=True,
             speech=False,
             options={},
             enabled=False,
             persist=False,
             translate=[],
             color={"r": 190, "g": 44, "b": 255},
@@ -155,15 +157,15 @@
 
 
 async def handle(request: web.Request) -> web.WebSocketResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
     messages = [
         await to_comment(message)
-        for message in (await client.messages.fetch_items(before=35)).values()
+        for message in (await client.chat.messages.fetch_items(before=35)).values()
     ]
 
     await ws.send_json(
         {
             "type": "connected",
             "data": CommentsData(comments=[message for message in messages if message]),
         }
@@ -176,15 +178,15 @@
             elif msg.type == web.WSMsgType.ERROR:
                 logger.error("ws connection closed with exception %s", ws.exception())
     finally:
         sessions.remove(ws)
     return ws
 
 
-@client.on(events.MessageCreate)
+@client.on(events.message.add)
 async def on_message_add(message: model.Message) -> None:
     comment = await to_comment(message)
     if not comment:
         return
     for ws in sessions:
         await ws.send_json(
             {
@@ -192,15 +194,15 @@
                 "data": CommentsData(
                     comments=[comment],
                 ),
             }
         )
 
 
-@client.on(events.MessageUpdate)
+@client.on(events.message.update)
 async def on_message_update(message: model.Message) -> None:
     comment = await to_comment(message)
     if comment is None:
         return
     for ws in sessions:
         await ws.send_json(
             {
@@ -208,24 +210,24 @@
                 "data": CommentsData(
                     comments=[comment],
                 ),
             }
         )
 
 
-@client.on(events.MessageDelete)
+@client.on(events.message.remove)
 async def on_message_delete(message: model.Message) -> None:
     for ws in sessions:
         await ws.send_json({"type": "deleted", "data": [message.key()]})
 
 
-async def main():
+@client.on(events.ready)
+async def on_ready():
     app.add_routes([web.get("/sub", handle)])
     runner = web.AppRunner(app)
     await runner.setup()
     site = web.TCPSite(runner, "localhost", 11180)
     asyncio.create_task(site.start())
-    await client.start()
 
 
 if __name__ == "__main__":
     client.run()
```

