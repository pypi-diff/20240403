# Comparing `tmp/nonebot_plugin_diffsinger-0.1.7.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.7.tar", last modified: Wed Apr  3 09:51:12 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.8.tar", last modified: Wed Apr  3 14:54:15 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.7.tar` & `nonebot_plugin_diffsinger-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 09:51:12.000000 nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:51:12.544901 nonebot_plugin_diffsinger-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-03 09:51:08.000000 nonebot_plugin_diffsinger-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 14:54:15.000000 nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:54:15.541440 nonebot_plugin_diffsinger-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-04-03 14:54:11.000000 nonebot_plugin_diffsinger-0.1.8/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.7/LICENSE` & `nonebot_plugin_diffsinger-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.7/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.7
+Version: 0.1.8
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.7/README.md` & `nonebot_plugin_diffsinger-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/__init__.py` & `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     homepage="https://github.com/zhzhongshi/nonebot-plugin-diffsinger",
     supported_adapters={"~onebot.v11"}
 )
 
 ds = on_command("diffsinger", priority=7)
 plugin_config = get_plugin_config(Config)
 url=plugin_config.ds_url
+ds_speedup=plugin_config.ds_speedup
 
 async def send_request(method, url, data=None,params=None):
     async with httpx.AsyncClient() as client:
         if method == "GET":
             response = await client.get(url,params=params)
         elif method == "POST":
             response = await client.post(url, json=data)
@@ -72,15 +73,15 @@
     submit_req={
         "model": model,
         "phonemes":phonemes,
         "f0":{
             "timestep":0.005,
             "values":f0
         },
-        "speedup": 255
+        "speedup": ds_speedup
     }
     
     submit=await send_request("POST",f"{url}submit", submit_req)
     submit=submit.json()
     wav=None
     while True:
         await asyncio.sleep(1)
```

### Comparing `nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.7/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.8/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.7
+Version: 0.1.8
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.7/setup.py` & `nonebot_plugin_diffsinger-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_diffsinger'
 DESCRIPTION = '用DiffSinger让bot唱歌'
 URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
 EMAIL = 'zhzhongshi@qq.com'
 AUTHOR = 'zhzhongshi'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 REQUIRED = [
     "nonebot2","nonebot-adapter-onebot","httpx","librosa"
 ]
 # What packages are optional?
 EXTRAS = {
 }
```

