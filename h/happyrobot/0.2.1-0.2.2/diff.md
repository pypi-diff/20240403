# Comparing `tmp/happyrobot-0.2.1.tar.gz` & `tmp/happyrobot-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "happyrobot-0.2.1.tar", last modified: Tue Mar 12 04:51:28 2024, max compression
+gzip compressed data, was "happyrobot-0.2.2.tar", last modified: Wed Apr  3 01:54:03 2024, max compression
```

## Comparing `happyrobot-0.2.1.tar` & `happyrobot-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-12 04:51:28.702824 happyrobot-0.2.1/
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)       88 2024-03-11 23:34:05.000000 happyrobot-0.2.1/HISTORY.rst
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)     1299 2024-03-11 23:15:48.000000 happyrobot-0.2.1/LICENSE
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      117 2024-03-11 23:35:42.000000 happyrobot-0.2.1/MANIFEST.in
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      751 2024-03-12 04:51:28.702726 happyrobot-0.2.1/PKG-INFO
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)       23 2024-03-12 03:42:43.000000 happyrobot-0.2.1/README.md
-drwxr-xr-x   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-12 04:51:28.700630 happyrobot-0.2.1/happyrobot/
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-11 23:46:43.000000 happyrobot-0.2.1/happyrobot/__init__.py
-drwxr-xr-x   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-12 04:51:28.702260 happyrobot-0.2.1/happyrobot/models/
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-11 23:45:43.000000 happyrobot-0.2.1/happyrobot/models/__init__.py
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      299 2024-03-11 23:58:49.000000 happyrobot-0.2.1/happyrobot/models/call.py
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      548 2024-03-12 03:44:05.000000 happyrobot-0.2.1/happyrobot/models/event.py
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      575 2024-03-12 04:50:00.000000 happyrobot-0.2.1/happyrobot/models/message.py
-drwxr-xr-x   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-12 04:51:28.701393 happyrobot-0.2.1/happyrobot.egg-info/
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      751 2024-03-12 04:51:28.000000 happyrobot-0.2.1/happyrobot.egg-info/PKG-INFO
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)      381 2024-03-12 04:51:28.000000 happyrobot-0.2.1/happyrobot.egg-info/SOURCES.txt
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)        1 2024-03-12 04:51:28.000000 happyrobot-0.2.1/happyrobot.egg-info/dependency_links.txt
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)        1 2024-03-12 03:44:16.000000 happyrobot-0.2.1/happyrobot.egg-info/not-zip-safe
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)       11 2024-03-12 04:51:28.000000 happyrobot-0.2.1/happyrobot.egg-info/top_level.txt
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)        0 2024-03-11 23:31:58.000000 happyrobot-0.2.1/requirements.txt
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)       79 2024-03-12 04:51:28.703157 happyrobot-0.2.1/setup.cfg
--rw-r--r--   0 pablorodriguezpalafox   (501) staff       (20)     1209 2024-03-12 04:51:15.000000 happyrobot-0.2.1/setup.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       88 2024-04-01 22:36:53.000000 happyrobot-0.2.2/HISTORY.rst
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1299 2024-04-01 22:36:53.000000 happyrobot-0.2.2/LICENSE
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      117 2024-04-01 22:36:53.000000 happyrobot-0.2.2/MANIFEST.in
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 01:54:03.762966 happyrobot-0.2.2/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       77 2024-04-01 22:38:42.000000 happyrobot-0.2.2/README.md
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.758965 happyrobot-0.2.2/happyrobot/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot/models/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/__init__.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      299 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/call.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      548 2024-04-01 22:36:53.000000 happyrobot-0.2.2/happyrobot/models/event.py
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     3217 2024-04-02 05:14:49.000000 happyrobot-0.2.2/happyrobot/models/message.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot/src/
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        0 2024-04-01 22:58:29.000000 happyrobot-0.2.2/happyrobot/src/__init__.py
+drwxrwxr-x   0 pablo     (1000) pablo     (1000)        0 2024-04-03 01:54:03.762966 happyrobot-0.2.2/happyrobot.egg-info/
+-rw-r--r--   0 pablo     (1000) pablo     (1000)      833 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/PKG-INFO
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)      441 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/SOURCES.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/dependency_links.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)        1 2024-04-01 22:38:17.000000 happyrobot-0.2.2/happyrobot.egg-info/not-zip-safe
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       13 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/requires.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       11 2024-04-03 01:54:03.000000 happyrobot-0.2.2/happyrobot.egg-info/top_level.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       12 2024-04-02 05:17:09.000000 happyrobot-0.2.2/requirements.txt
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)       79 2024-04-03 01:54:03.762966 happyrobot-0.2.2/setup.cfg
+-rw-rw-r--   0 pablo     (1000) pablo     (1000)     1228 2024-04-03 01:51:57.000000 happyrobot-0.2.2/setup.py
```

### Comparing `happyrobot-0.2.1/LICENSE` & `happyrobot-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.1/PKG-INFO` & `happyrobot-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.10
 License-File: LICENSE
+Requires-Dist: pytz==2024.1
 
 # Happyrobot Python SDK
 
+## Installation
+
+```bash
+pip install happyrobot
+```
+
+
 =======
 History
 =======
 
 0.1.0 (2024-03-11)
 ------------------
```

### Comparing `happyrobot-0.2.1/happyrobot/models/event.py` & `happyrobot-0.2.2/happyrobot/models/event.py`

 * *Files identical despite different names*

### Comparing `happyrobot-0.2.1/happyrobot.egg-info/PKG-INFO` & `happyrobot-0.2.2/happyrobot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: happyrobot
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package lets you interact with Happyrobot directly from Python.
 Author: Happyrobot
 Author-email: founders@happyrobot.ai
 Keywords: happyrobot
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.10
 License-File: LICENSE
+Requires-Dist: pytz==2024.1
 
 # Happyrobot Python SDK
 
+## Installation
+
+```bash
+pip install happyrobot
+```
+
+
 =======
 History
 =======
 
 0.1.0 (2024-03-11)
 ------------------
```

### Comparing `happyrobot-0.2.1/setup.py` & `happyrobot-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 def read_requirements(file):
     with open(file) as f:
         return f.read().splitlines()
 
 requirements = read_requirements('requirements.txt')
 
+VERSION = '0.2.2'
+
 setup(
     author="Happyrobot",
     author_email='founders@happyrobot.ai',
     name='happyrobot',
     python_requires='>=3.10',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
@@ -31,10 +33,10 @@
     ],
     description="This package lets you interact with Happyrobot directly from Python.",
     install_requires=requirements,
     long_description=readme + '\n\n' + history,
     include_package_data=True,
     keywords='happyrobot',
     packages=find_packages(include=['happyrobot', 'happyrobot.*']),
-    version='0.2.1',
+    version=VERSION,
     zip_safe=False,
 )
```

