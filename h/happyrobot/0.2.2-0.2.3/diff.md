# Comparing `tmp/happyrobot-0.2.2.tar.gz` & `tmp/happyrobot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyrobot-0.2.2.tar", last modified: Wed Apr  3 01:54:03 2024, max compression
+gzip compressed data, was "happyrobot-0.2.3.tar", last modified: Wed Apr  3 15:51:00 2024, max compression
```

## Comparing `happyrobot-0.2.2.tar` & `happyrobot-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       88 2024-04-01 22:36:53.000000 happyrobot-0.2.2/HISTORY.rst
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1299 2024-04-01 22:36:53.000000 happyrobot-0.2.2/LICENSE
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      117 2024-04-01 22:36:53.000000 happyrobot-0.2.2/MANIFEST.in
--rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 01:54:03.762966 happyrobot-0.2.2/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       77 2024-04-01 22:38:42.000000 happyrobot-0.2.2/README.md
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.758965 happyrobot-0.2.2/happyrobot/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot/models/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/__init__.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      299 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/call.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      548 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/event.py
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     3217 2024-04-02 05:14:49.000000 happyrobot-0.2.2/happyrobot/models/message.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot/src/
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:58:29.000000 happyrobot-0.2.2/happyrobot/src/__init__.py
-drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot.egg-info/
--rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/PKG-INFO
--rw-rw-r--   0 pablo     (1000) pablo     (1000)      441 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/SOURCES.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/dependency_links.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-01 22:38:17.000000 happyrobot-0.2.2/happyrobot.egg-info/not-zip-safe
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       13 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/requires.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/top_level.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       12 2024-04-02 05:17:09.000000 happyrobot-0.2.2/requirements.txt
--rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2024-04-03 01:54:03.762966 happyrobot-0.2.2/setup.cfg
--rw-rw-r--   0 pablo     (1000) pablo     (1000)     1228 2024-04-03 01:51:57.000000 happyrobot-0.2.2/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.539030 happyrobot-0.2.3/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       88 2024-04-01 22:36:53.000000 happyrobot-0.2.3/HISTORY.rst
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1299 2024-04-01 22:36:53.000000 happyrobot-0.2.3/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      117 2024-04-01 22:36:53.000000 happyrobot-0.2.3/MANIFEST.in
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 15:51:00.539030 happyrobot-0.2.3/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       77 2024-04-01 22:38:42.000000 happyrobot-0.2.3/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.535030 happyrobot-0.2.3/happyrobot/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.3/happyrobot/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.539030 happyrobot-0.2.3/happyrobot/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.3/happyrobot/models/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      299 2024-04-01 22:36:53.000000 happyrobot-0.2.3/happyrobot/models/call.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      548 2024-04-01 22:36:53.000000 happyrobot-0.2.3/happyrobot/models/event.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3217 2024-04-02 05:14:49.000000 happyrobot-0.2.3/happyrobot/models/message.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.539030 happyrobot-0.2.3/happyrobot/src/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:58:29.000000 happyrobot-0.2.3/happyrobot/src/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.539030 happyrobot-0.2.3/happyrobot/src/utils/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:40:33.000000 happyrobot-0.2.3/happyrobot/src/utils/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      558 2024-04-02 05:18:42.000000 happyrobot-0.2.3/happyrobot/src/utils/date_utils.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1421 2024-04-01 22:58:52.000000 happyrobot-0.2.3/happyrobot/src/utils/message_utils.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 15:51:00.539030 happyrobot-0.2.3/happyrobot.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      547 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/not-zip-safe
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       13 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2024-04-03 15:51:00.000000 happyrobot-0.2.3/happyrobot.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       12 2024-04-02 05:17:09.000000 happyrobot-0.2.3/requirements.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2024-04-03 15:51:00.539030 happyrobot-0.2.3/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1228 2024-04-03 15:47:47.000000 happyrobot-0.2.3/setup.py
```

### Comparing `happyrobot-0.2.2/LICENSE` & `happyrobot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.2/PKG-INFO` & `happyrobot-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.2
+Version: 0.2.3
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `happyrobot-0.2.2/happyrobot/models/event.py` & `happyrobot-0.2.3/happyrobot/models/event.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.2/happyrobot/models/message.py` & `happyrobot-0.2.3/happyrobot/models/message.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.2/happyrobot.egg-info/PKG-INFO` & `happyrobot-0.2.3/happyrobot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.2
+Version: 0.2.3
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `happyrobot-0.2.2/setup.py` & `happyrobot-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 def read_requirements(file):
     with open(file) as f:
         return f.read().splitlines()
 
 requirements = read_requirements('requirements.txt')
 
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 setup(
     author="Happyrobot",
     author_email='founders@happyrobot.ai',
     name='happyrobot',
     python_requires='>=3.10',
     classifiers=[
```
