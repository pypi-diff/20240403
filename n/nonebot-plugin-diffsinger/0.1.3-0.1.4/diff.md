# Comparing `tmp/nonebot_plugin_diffsinger-0.1.3.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.3.tar", last modified: Wed Apr  3 04:32:34 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.4.tar", last modified: Wed Apr  3 07:46:47 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.3.tar` & `nonebot_plugin_diffsinger-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 04:32:34.327696 nonebot_plugin_diffsinger-0.1.3/
--rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2049 2024-04-03 04:32:34.321941 nonebot_plugin_diffsinger-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1263 2024-04-03 04:10:04.000000 nonebot_plugin_diffsinger-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 04:32:34.296680 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger/
--rw-rw-rw-   0        0        0     2731 2024-04-03 04:31:28.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-04-03 03:12:35.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger/data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-03 04:32:34.321941 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/
--rw-rw-rw-   0        0        0     2049 2024-04-03 04:32:34.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-03 04:32:34.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 04:32:34.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-03 04:32:34.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 04:32:34.000000 nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 04:32:34.327696 nonebot_plugin_diffsinger-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     3806 2024-04-03 04:32:22.000000 nonebot_plugin_diffsinger-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.636407 nonebot_plugin_diffsinger-0.1.4/
+-rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2049 2024-04-03 07:46:47.635381 nonebot_plugin_diffsinger-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1263 2024-04-03 04:10:04.000000 nonebot_plugin_diffsinger-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.621312 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/
+-rw-rw-rw-   0        0        0     3300 2024-04-03 07:43:48.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/__init__.py
+-rw-rw-rw-   0        0        0      114 2024-04-03 07:43:56.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/config.py
+-rw-rw-rw-   0        0        0     1438 2024-04-03 07:44:09.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/data_source.py
+drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.633830 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/
+-rw-rw-rw-   0        0        0     2049 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 07:46:47.636407 nonebot_plugin_diffsinger-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     3806 2024-04-03 07:45:13.000000 nonebot_plugin_diffsinger-0.1.4/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.3/LICENSE` & `nonebot_plugin_diffsinger-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.3/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.3
+Version: 0.1.4
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.3/README.md` & `nonebot_plugin_diffsinger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger/__init__.py` & `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from nonebot import on_command
 from nonebot.adapters.onebot.v11.bot import Bot
 from nonebot.adapters.onebot.v11.message import Message,MessageSegment
 from nonebot.adapters.onebot.v11.event import  MessageEvent
 from nonebot.params import CommandArg
 from nonebot.plugin import PluginMetadata
+from nonebot import get_plugin_config
+from httpx import Response
+from .config import Config
 
 from .data_source import get_f0, process_notes, bpm2dur
-
+import nonebot
+import asyncio
 import json
 import httpx
 import time
 
 __plugin_meta__ = PluginMetadata(
     name="diffsinger",
     description="用DiffSinger让bot唱歌",
@@ -38,59 +42,69 @@
 """,
     type="application",
     homepage="https://github.com/zhzhongshi/nonebot-plugin-diffsinger",
     supported_adapters={"~onebot.v11"}
 )
 
 ds = on_command("diffsinger", priority=7)
-url="http://127.0.0.1:9266/"
+plugin_config = get_plugin_config(Config)
+url=plugin_config.ds_url
 
+async def send_request(method, url, data=None,params=None) ->Response:
+    async with httpx.AsyncClient() as client:
+        if method == "GET":
+            response = await client.get(url,params=params)
+        elif method == "POST":
+            response = await client.post(url, json=data,params=params)
+        return response
+    
 @ds.handle()
 async def sendcmd(bot: Bot, event: MessageEvent, arg: Message=CommandArg()):
     arg = arg.extract_plain_text()
     preps=[]
     lists=str(arg).split("|")
     for i in lists:
         notes=i.split("~")
         prep=bpm2dur(int(notes[0]),json.loads(notes[1]))
         preps.extend(prep)
     
-    phone_dict=httpx.request("GET",f"{url}getdict").json()
-    req=process_notes(preps,phone_dict)
+    phone_dict=await send_request("GET",f"{url}getdict")
+    req=process_notes(preps,phone_dict.json())
     phonemes=get_rhythm(req)
     f0=get_f0(req)
     model="1215_opencpop_ds1000_fix_label_nomidi"
     submit_req={
         "model": model,
         "phonemes":phonemes,
         "f0":{
             "timestep":0.005,
             "values":f0
         },
         "speedup": 255
     }
     
-    submit=httpx.request("POST",f"{url}submit", json=submit_req).json()
+    submit=await send_request("POST", f"{url}submit", submit_req)
     wav=None
     while True:
-        time.sleep(1)
-        stat=httpx.request("POST",f'{url}query', json={"token":submit["token"]}).json()
+        await asyncio.sleep(1)
+        stat = await send_request("POST", f'{url}query', {"token": submit.json()["token"]})
+        stat=stat.json()
         if stat["status"]=="HIT_CACHE":
             break
         elif stat["status"] == "QUEUED":
             continue
         elif stat["status"] == "RUNNING":
             continue
         elif stat["status"] == "FINISHED":
             break
         elif stat["status"] == "FAILED":
             await ds.finish("错误："+stat["message"])
         elif stat["status"] == "CANCELLED":
             await ds.finish("已取消")
         
-    wav=httpx.request("GET",f"{url}download",params={"token":submit["token"]}).content
-    await ds.finish(MessageSegment.record(wav))
+    wav=await send_request("GET",f"{url}download",params={"token":submit.json()["token"]})
+    await ds.finish(MessageSegment.record(wav.content))
     
-def get_rhythm(req):
-    resp=httpx.request("POST",url+'rhythm', json=req)
+async def get_rhythm(req):
+    resp=await send_request("POST",f"{url}rhythm",data=req)
     phonemes=resp.json()['phonemes']
     return phonemes
```

### Comparing `nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/data_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import librosa
-import httpx
-
 def process_notes(preps,phone_dict):
     notes=[]
     for prep in preps:
         if prep[2] in phone_dict:
             notes.append({"key": prep[0],"duration": prep[1],"slur": False,"phonemes": phone_dict[prep[2]]})
         else:
             if prep[2] in ["AP","SP"]:
```

### Comparing `nonebot_plugin_diffsinger-0.1.3/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.3
+Version: 0.1.4
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.3/setup.py` & `nonebot_plugin_diffsinger-0.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_diffsinger'
 DESCRIPTION = '用DiffSinger让bot唱歌'
 URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
 EMAIL = 'zhzhongshi@qq.com'
 AUTHOR = 'zhzhongshi'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 REQUIRED = [
     "nonebot2","nonebot-adapter-onebot","httpx","librosa"
 ]
 # What packages are optional?
 EXTRAS = {
 }
```

