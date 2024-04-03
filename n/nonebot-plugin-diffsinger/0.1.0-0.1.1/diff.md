# Comparing `tmp/nonebot_plugin_diffsinger-0.1.0.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.0.tar", last modified: Wed Apr  3 03:36:39 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.1.tar", last modified: Wed Apr  3 03:58:48 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.0.tar` & `nonebot_plugin_diffsinger-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:36:39.168099 nonebot_plugin_diffsinger-0.1.0/
--rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1744 2024-04-03 03:36:39.167059 nonebot_plugin_diffsinger-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      958 2024-04-03 03:19:41.000000 nonebot_plugin_diffsinger-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 03:36:39.119557 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger/
--rw-rw-rw-   0        0        0     2089 2024-04-03 03:19:49.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-04-03 03:12:35.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger/data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-03 03:36:39.165697 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/
--rw-rw-rw-   0        0        0     1744 2024-04-03 03:36:39.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      361 2024-04-03 03:36:39.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:36:39.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-03 03:36:39.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 03:36:39.000000 nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 03:36:39.168099 nonebot_plugin_diffsinger-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3872 2024-04-03 03:33:55.000000 nonebot_plugin_diffsinger-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.849724 nonebot_plugin_diffsinger-0.1.1/
+-rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1744 2024-04-03 03:58:48.845974 nonebot_plugin_diffsinger-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2024-04-03 03:19:41.000000 nonebot_plugin_diffsinger-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.795144 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/
+-rw-rw-rw-   0        0        0     2701 2024-04-03 03:56:12.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/__init__.py
+-rw-rw-rw-   0        0        0     1454 2024-04-03 03:12:35.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/data_source.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:58:48.841888 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/
+-rw-rw-rw-   0        0        0     1744 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      361 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 03:58:48.000000 nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 03:58:48.850387 nonebot_plugin_diffsinger-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3806 2024-04-03 03:57:09.000000 nonebot_plugin_diffsinger-0.1.1/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.0/LICENSE` & `nonebot_plugin_diffsinger-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.0/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.0
+Version: 0.1.1
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.0/README.md` & `nonebot_plugin_diffsinger-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.0/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.1/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.0
+Version: 0.1.1
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `nonebot_plugin_diffsinger-0.1.0/setup.py` & `nonebot_plugin_diffsinger-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,18 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_diffsinger'
 DESCRIPTION = '用DiffSinger让bot唱歌'
 URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
 EMAIL = 'zhzhongshi@qq.com'
 AUTHOR = 'zhzhongshi'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.0'
-
-# What packages are required for this module to be executed?
+VERSION = '0.1.1'
 REQUIRED = [
     "nonebot2","nonebot-adapter-onebot","httpx","librosa"
 ]
-
 # What packages are optional?
 EXTRAS = {
 }
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
```

