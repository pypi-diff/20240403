# Comparing `tmp/nonebot_plugin_diffsinger-0.1.4.tar.gz` & `tmp/nonebot_plugin_diffsinger-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_diffsinger-0.1.4.tar", last modified: Wed Apr  3 07:46:47 2024, max compression
+gzip compressed data, was "nonebot_plugin_diffsinger-0.1.5.tar", last modified: Wed Apr  3 08:29:10 2024, max compression
```

## Comparing `nonebot_plugin_diffsinger-0.1.4.tar` & `nonebot_plugin_diffsinger-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.636407 nonebot_plugin_diffsinger-0.1.4/
--rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2049 2024-04-03 07:46:47.635381 nonebot_plugin_diffsinger-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1263 2024-04-03 04:10:04.000000 nonebot_plugin_diffsinger-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.621312 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/
--rw-rw-rw-   0        0        0     3300 2024-04-03 07:43:48.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/__init__.py
--rw-rw-rw-   0        0        0      114 2024-04-03 07:43:56.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/config.py
--rw-rw-rw-   0        0        0     1438 2024-04-03 07:44:09.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/data_source.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:46:47.633830 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/
--rw-rw-rw-   0        0        0     2049 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-04-03 07:46:47.000000 nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 07:46:47.636407 nonebot_plugin_diffsinger-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     3806 2024-04-03 07:45:13.000000 nonebot_plugin_diffsinger-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:29:10.390030 nonebot_plugin_diffsinger-0.1.5/
+-rw-rw-rw-   0        0        0     1055 2024-04-03 03:16:46.000000 nonebot_plugin_diffsinger-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-03 03:17:16.000000 nonebot_plugin_diffsinger-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     2049 2024-04-03 08:29:10.388167 nonebot_plugin_diffsinger-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1263 2024-04-03 04:10:04.000000 nonebot_plugin_diffsinger-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:29:10.367327 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/
+-rw-rw-rw-   0        0        0     3300 2024-04-03 07:43:48.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/__init__.py
+-rw-rw-rw-   0        0        0       97 2024-04-03 08:27:42.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/config.py
+-rw-rw-rw-   0        0        0     1438 2024-04-03 07:44:09.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/data_source.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:29:10.388167 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/
+-rw-rw-rw-   0        0        0     2049 2024-04-03 08:29:10.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      397 2024-04-03 08:29:10.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:29:10.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-04-03 08:29:10.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-04-03 08:29:10.000000 nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:29:10.390030 nonebot_plugin_diffsinger-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     3806 2024-04-03 08:28:46.000000 nonebot_plugin_diffsinger-0.1.5/setup.py
```

### Comparing `nonebot_plugin_diffsinger-0.1.4/LICENSE` & `nonebot_plugin_diffsinger-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.4/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.4
+Version: 0.1.5
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-adapter-onebot
```

### Comparing `nonebot_plugin_diffsinger-0.1.4/README.md` & `nonebot_plugin_diffsinger-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/__init__.py` & `nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger/data_source.py` & `nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_diffsinger-0.1.4/nonebot_plugin_diffsinger.egg-info/PKG-INFO` & `nonebot_plugin_diffsinger-0.1.5/nonebot_plugin_diffsinger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_diffsinger
-Version: 0.1.4
+Version: 0.1.5
 Summary: 用DiffSinger让bot唱歌
 Home-page: https://github.com/zhzhongshi/nonebot-plugin-diffsinger
 Author: zhzhongshi
 Author-email: zhzhongshi@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-adapter-onebot
```

### Comparing `nonebot_plugin_diffsinger-0.1.4/setup.py` & `nonebot_plugin_diffsinger-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Package meta-data.
 NAME = 'nonebot_plugin_diffsinger'
 DESCRIPTION = '用DiffSinger让bot唱歌'
 URL = 'https://github.com/zhzhongshi/nonebot-plugin-diffsinger'
 EMAIL = 'zhzhongshi@qq.com'
 AUTHOR = 'zhzhongshi'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 REQUIRED = [
     "nonebot2","nonebot-adapter-onebot","httpx","librosa"
 ]
 # What packages are optional?
 EXTRAS = {
 }
 
@@ -108,15 +108,15 @@
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

