# Comparing `tmp/nonebot_plugin_diffsinger-0.1.1.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.1.tar", last modified: Wed Apr  3 03:58:48 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.2.tar", last modified: Wed Apr  3 04:05:09 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.1.tar` & `nonebot_plugin_diffsinger-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.849724 nonebot_plugin_diffsinger-0.1.1/
--rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2024-04-03 03:58:48.845974 nonebot_plugin_diffsinger-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      958 2024-04-03 03:19:41.000000 nonebot_plugin_diffsinger-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.795144 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/
--rw-rw-rw-   0        0        0     2701 2024-04-03 03:56:12.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-04-03 03:12:35.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.841888 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/
--rw-rw-rw-   0        0        0     1744 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:58:48.850387 nonebot_plugin_diffsinger-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3806 2024-04-03 03:57:09.000000 nonebot_plugin_diffsinger-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:05:09.514641 nonebot_plugin_diffsinger-0.1.2/
+-rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2024-04-03 04:05:09.514111 nonebot_plugin_diffsinger-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2024-04-03 03:19:41.000000 nonebot_plugin_diffsinger-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 04:05:09.477125 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger/
+-rw-rw-rw-   0        0        0     2741 2024-04-03 04:03:13.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger/__init__.py
+-rw-rw-rw-   0        0        0     1454 2024-04-03 03:12:35.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger/data_source.py
+drwxrwxrwx   0        0        0        0 2024-04-03 04:05:09.511130 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/
+-rw-rw-rw-   0        0        0     1744 2024-04-03 04:05:09.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-03 04:05:09.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 04:05:09.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-03 04:05:09.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 04:05:09.000000 nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 04:05:09.518173 nonebot_plugin_diffsinger-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3806 2024-04-03 04:04:12.000000 nonebot_plugin_diffsinger-0.1.2/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.1/LICENSE` & `nonebot_plugin_diffsinger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.1/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.1/README.md` & `nonebot_plugin_diffsinger-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/__init__.py` & `nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 [55,16,"zhang"],
 [60,4,"AP"]
 ]
 
 """,
     type="application",
     homepage="https://github.com/zhzhongshi/nonebot-plugin-diffsinger",
+    supported_adapters={"~onebot.v11"}
 )
 
 ds = on_command("diffsinger", priority=7)
 url="http://127.0.0.1:9266/"
 
 @ds.handle()
 async def sendcmd(bot: Bot, event: MessageEvent, arg: Message=CommandArg()):
```

### Comparing `nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.2/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.1
+Version: 0.1.2
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.1/setup.py` & `nonebot_plugin_diffsinger-0.1.2/setup.py`

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
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 REQUIRED = [
     "nonebot2","nonebot-adapter-onebot","httpx","librosa"
 ]
 # What packages are optional?
 EXTRAS = {
 }
```

