# Comparing `tmp/shuttleai-3.7.tar.gz` & `tmp/shuttleai-3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shuttleai-3.7.tar", last modified: Wed Apr  3 08:42:34 2024, max compression
+gzip compressed data, was "shuttleai-3.8.tar", last modified: Wed Apr  3 08:50:28 2024, max compression
```

## Comparing `shuttleai-3.7.tar` & `shuttleai-3.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.871885 shuttleai-3.7/
--rw-rw-rw-   0        0        0     4082 2024-04-03 08:42:34.869886 shuttleai-3.7/PKG-INFO
--rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 08:42:34.871885 shuttleai-3.7/setup.cfg
--rw-rw-rw-   0        0        0     1264 2024-04-03 08:26:16.000000 shuttleai-3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.792884 shuttleai-3.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.799882 shuttleai-3.7/src/shuttleai/
--rw-rw-rw-   0        0        0      574 2024-04-03 08:42:16.000000 shuttleai-3.7/src/shuttleai/__init__.py
--rw-rw-rw-   0        0        0     4411 2024-04-03 08:25:30.000000 shuttleai-3.7/src/shuttleai/cli.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.859885 shuttleai-3.7/src/shuttleai/client/
--rw-rw-rw-   0        0        0       72 2024-04-02 07:23:05.000000 shuttleai-3.7/src/shuttleai/client/__init__.py
--rw-rw-rw-   0        0        0    17196 2024-04-03 08:32:47.000000 shuttleai-3.7/src/shuttleai/client/_async.py
--rw-rw-rw-   0        0        0     3329 2024-04-03 08:21:53.000000 shuttleai-3.7/src/shuttleai/client/_sync.py
--rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.7/src/shuttleai/log.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.864883 shuttleai-3.7/src/shuttleai/schemas/
--rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.7/src/shuttleai/schemas/__init__.py
--rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.7/src/shuttleai/schemas/schemas.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:42:34.867883 shuttleai-3.7/src/shuttleai.egg-info/
--rw-rw-rw-   0        0        0     4082 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-03 08:42:34.000000 shuttleai-3.7/src/shuttleai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.329437 shuttleai-3.8/
+-rw-rw-rw-   0        0        0     4082 2024-04-03 08:50:28.326427 shuttleai-3.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3226 2024-04-03 08:41:19.000000 shuttleai-3.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:50:28.329437 shuttleai-3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2024-04-03 08:26:16.000000 shuttleai-3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.267432 shuttleai-3.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.278435 shuttleai-3.8/src/shuttleai/
+-rw-rw-rw-   0        0        0      574 2024-04-03 08:49:43.000000 shuttleai-3.8/src/shuttleai/__init__.py
+-rw-rw-rw-   0        0        0     4419 2024-04-03 08:49:21.000000 shuttleai-3.8/src/shuttleai/cli.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.319428 shuttleai-3.8/src/shuttleai/client/
+-rw-rw-rw-   0        0        0       72 2024-04-02 07:23:05.000000 shuttleai-3.8/src/shuttleai/client/__init__.py
+-rw-rw-rw-   0        0        0    17196 2024-04-03 08:32:47.000000 shuttleai-3.8/src/shuttleai/client/_async.py
+-rw-rw-rw-   0        0        0     3329 2024-04-03 08:21:53.000000 shuttleai-3.8/src/shuttleai/client/_sync.py
+-rw-rw-rw-   0        0        0     1636 2024-04-01 03:32:40.000000 shuttleai-3.8/src/shuttleai/log.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.323428 shuttleai-3.8/src/shuttleai/schemas/
+-rw-rw-rw-   0        0        0      230 2024-04-03 02:14:24.000000 shuttleai-3.8/src/shuttleai/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2030 2024-04-03 02:15:03.000000 shuttleai-3.8/src/shuttleai/schemas/schemas.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:28.325427 shuttleai-3.8/src/shuttleai.egg-info/
+-rw-rw-rw-   0        0        0     4082 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      471 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 08:50:28.000000 shuttleai-3.8/src/shuttleai.egg-info/top_level.txt
```

### Comparing `shuttleai-3.7/PKG-INFO` & `shuttleai-3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.7
+Version: 3.8
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shuttleai-3.7/README.md` & `shuttleai-3.8/README.md`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/setup.py` & `shuttleai-3.8/setup.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/src/shuttleai/__init__.py` & `shuttleai-3.8/src/shuttleai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .client import ShuttleAsyncClient, ShuttleClient
 
 from sys import executable
 from os import system
 from httpx import get
 
-__version__ = "3.7"
+__version__ = "3.8"
 
 try:
     CURRENT_VERSION = get(
         "https://pypi.org/pypi/shuttleai/json").json().get("info").get("version")
 except:
     CURRENT_VERSION = __version__
```

### Comparing `shuttleai-3.7/src/shuttleai/cli.py` & `shuttleai-3.8/src/shuttleai/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
                 break
 
         if system is not None:
             messages.add_message(system, "system")
         if prompt is not None:
             messages.add_message(prompt, "user")
 
-        async with ShuttleAsyncClient(key, 120) as shuttle:
+        async with ShuttleAsyncClient(key, timeout=120) as shuttle:
             response = await shuttle.chat_completion(
                 model=model,
                 messages=messages.messages,
                 stream=stream
             )
 
             print(f"{TerminalColor.DARKPURPLE}ShuttleAI{TerminalColor.ENDC}: ", end="")
```

### Comparing `shuttleai-3.7/src/shuttleai/client/_async.py` & `shuttleai-3.8/src/shuttleai/client/_async.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/src/shuttleai/client/_sync.py` & `shuttleai-3.8/src/shuttleai/client/_sync.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/src/shuttleai/log.py` & `shuttleai-3.8/src/shuttleai/log.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/src/shuttleai/schemas/schemas.py` & `shuttleai-3.8/src/shuttleai/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `shuttleai-3.7/src/shuttleai.egg-info/PKG-INFO` & `shuttleai-3.8/src/shuttleai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shuttleai
-Version: 3.7
+Version: 3.8
 Summary: Access Shuttle AI's API via a simple and user-friendly lib. Dashboard: https://shuttleai.app Discord: https://discord.gg/shuttleai
 Home-page: https://github.com/shuttleai/shuttleai-python
 Author: shuttle
 Author-email: noreply@shuttleai.app
 Keywords: shuttleai,ai,gpt,claude,api,free,chatgpt,gpt-4
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

