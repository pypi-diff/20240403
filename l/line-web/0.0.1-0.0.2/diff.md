# Comparing `tmp/line-web-0.0.1.tar.gz` & `tmp/line-web-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "line-web-0.0.1.tar", last modified: Wed Apr  3 10:06:01 2024, max compression
+gzip compressed data, was "line-web-0.0.2.tar", last modified: Wed Apr  3 10:11:05 2024, max compression
```

## Comparing `line-web-0.0.1.tar` & `line-web-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:06:01.595899 line-web-0.0.1/
--rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1661 2024-04-03 10:06:01.594916 line-web-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      960 2024-04-03 10:05:42.000000 line-web-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 10:06:01.570305 line-web-0.0.1/line/
--rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.1/line/__init__.py
--rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.1/line/authentications.py
--rw-rw-rw-   0        0        0    33222 2024-04-03 09:07:35.000000 line-web-0.0.1/line/core.py
--rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.1/line/exceptions.py
--rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.1/line/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:06:01.593916 line-web-0.0.1/line_web.egg-info/
--rw-rw-rw-   0        0        0     1661 2024-04-03 10:06:01.000000 line-web-0.0.1/line_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-04-03 10:06:01.000000 line-web-0.0.1/line_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:06:01.000000 line-web-0.0.1/line_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-04-03 10:06:01.000000 line-web-0.0.1/line_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 10:06:01.000000 line-web-0.0.1/line_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 10:06:01.595899 line-web-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3899 2024-04-03 10:05:42.000000 line-web-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:11:05.904130 line-web-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2024-04-02 09:34:47.000000 line-web-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       25 2024-04-02 09:34:47.000000 line-web-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1661 2024-04-03 10:11:05.903095 line-web-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2024-04-03 10:07:33.000000 line-web-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 10:11:05.888579 line-web-0.0.2/line/
+-rw-rw-rw-   0        0        0       22 2024-04-02 09:34:47.000000 line-web-0.0.2/line/__init__.py
+-rw-rw-rw-   0        0        0     5465 2024-04-03 03:03:50.000000 line-web-0.0.2/line/authentications.py
+-rw-rw-rw-   0        0        0    33222 2024-04-03 09:07:35.000000 line-web-0.0.2/line/core.py
+-rw-rw-rw-   0        0        0      215 2024-04-03 03:11:50.000000 line-web-0.0.2/line/exceptions.py
+-rw-rw-rw-   0        0        0      223 2024-04-03 08:52:24.000000 line-web-0.0.2/line/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:11:05.902059 line-web-0.0.2/line_web.egg-info/
+-rw-rw-rw-   0        0        0     1661 2024-04-03 10:11:05.000000 line-web-0.0.2/line_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-03 10:11:05.000000 line-web-0.0.2/line_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:11:05.000000 line-web-0.0.2/line_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2024-04-03 10:11:05.000000 line-web-0.0.2/line_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 10:11:05.000000 line-web-0.0.2/line_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 10:11:05.904130 line-web-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3899 2024-04-03 10:07:33.000000 line-web-0.0.2/setup.py
```

### Comparing `line-web-0.0.1/LICENSE` & `line-web-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `line-web-0.0.1/PKG-INFO` & `line-web-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.1
+Version: 0.0.2
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -34,15 +34,15 @@
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
 bot = Line(
     authentication=BusinessAuthentication("<username>", "<password>"), # Business Account
-    bot="<shop>" # shop name
+    bot="<shop>" # Shop Name
 )
 
 
 # event
 # chat(message, messageSent, read, typing, typingVanished, noteUpdated, markedAsManualChat, unmarkedAsManualChat, chatRead, assigneeUpdated, tagged, ...)
 # botUnreadChatCount(increment, ...)
 # botInfo(hasChatRoomChanged, ...)
```

### Comparing `line-web-0.0.1/README.md` & `line-web-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
 bot = Line(
     authentication=BusinessAuthentication("<username>", "<password>"), # Business Account
-    bot="<shop>" # shop name
+    bot="<shop>" # Shop Name
 )
 
 
 # event
 # chat(message, messageSent, read, typing, typingVanished, noteUpdated, markedAsManualChat, unmarkedAsManualChat, chatRead, assigneeUpdated, tagged, ...)
 # botUnreadChatCount(increment, ...)
 # botInfo(hasChatRoomChanged, ...)
```

### Comparing `line-web-0.0.1/line/authentications.py` & `line-web-0.0.2/line/authentications.py`

 * *Files identical despite different names*

### Comparing `line-web-0.0.1/line/core.py` & `line-web-0.0.2/line/core.py`

 * *Files identical despite different names*

### Comparing `line-web-0.0.1/line_web.egg-info/PKG-INFO` & `line-web-0.0.2/line_web.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: line-web
-Version: 0.0.1
+Version: 0.0.2
 Summary: Line chatbot framework.
 Home-page: https://github.com/miloira/line-web
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -34,15 +34,15 @@
 
 ```python
 from line import Line
 from line.authentications import BusinessAuthentication
 
 bot = Line(
     authentication=BusinessAuthentication("<username>", "<password>"), # Business Account
-    bot="<shop>" # shop name
+    bot="<shop>" # Shop Name
 )
 
 
 # event
 # chat(message, messageSent, read, typing, typingVanished, noteUpdated, markedAsManualChat, unmarkedAsManualChat, chatRead, assigneeUpdated, tagged, ...)
 # botUnreadChatCount(increment, ...)
 # botInfo(hasChatRoomChanged, ...)
```

### Comparing `line-web-0.0.1/setup.py` & `line-web-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'line-web'
 DESCRIPTION = 'Line chatbot framework.'
 URL = 'https://github.com/miloira/line-web'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'requests',
     'loguru',
     'pyee'
 ]
```

