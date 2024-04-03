# Comparing `tmp/socketshark-0.4.0.tar.gz` & `tmp/socketshark-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketshark-0.4.0.tar", last modified: Wed Dec 13 09:42:54 2023, max compression
+gzip compressed data, was "socketshark-0.5.0.tar", last modified: Wed Apr  3 10:06:26 2024, max compression
```

## Comparing `socketshark-0.4.0.tar` & `socketshark-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.149656 socketshark-0.4.0/
--rw-r--r--   0 georgy     (501) staff       (20)     1089 2023-12-12 14:17:46.000000 socketshark-0.4.0/LICENSE
--rw-r--r--   0 georgy     (501) staff       (20)    23367 2023-12-13 09:42:54.149537 socketshark-0.4.0/PKG-INFO
--rw-r--r--   0 georgy     (501) staff       (20)    22649 2023-12-12 14:17:46.000000 socketshark-0.4.0/README.rst
--rw-r--r--   0 georgy     (501) staff       (20)      141 2023-12-12 14:17:46.000000 socketshark-0.4.0/pyproject.toml
--rw-r--r--   0 georgy     (501) staff       (20)     1242 2023-12-13 09:42:54.150070 socketshark-0.4.0/setup.cfg
--rw-r--r--   0 georgy     (501) staff       (20)     1312 2023-12-12 18:51:29.000000 socketshark-0.4.0/setup.py
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.146619 socketshark-0.4.0/socketshark/
--rw-r--r--   0 georgy     (501) staff       (20)     8776 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/__init__.py
--rw-r--r--   0 georgy     (501) staff       (20)       25 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/__main__.py
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.147600 socketshark-0.4.0/socketshark/backend/
--rw-r--r--   0 georgy     (501) staff       (20)        0 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/backend/__init__.py
--rw-r--r--   0 georgy     (501) staff       (20)     4958 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/backend/websockets.py
--rw-r--r--   0 georgy     (501) staff       (20)     2390 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/config_defaults.py
--rw-r--r--   0 georgy     (501) staff       (20)      888 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/constants.py
--rw-r--r--   0 georgy     (501) staff       (20)     5938 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/events.py
--rw-r--r--   0 georgy     (501) staff       (20)      297 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/exceptions.py
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.148234 socketshark-0.4.0/socketshark/metrics/
--rw-r--r--   0 georgy     (501) staff       (20)     1467 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/metrics/__init__.py
--rw-r--r--   0 georgy     (501) staff       (20)     1005 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/metrics/log.py
--rw-r--r--   0 georgy     (501) staff       (20)     1700 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/metrics/prometheus.py
--rw-r--r--   0 georgy     (501) staff       (20)     6908 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/receiver.py
--rw-r--r--   0 georgy     (501) staff       (20)     1473 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/redis_connection.py
--rw-r--r--   0 georgy     (501) staff       (20)     4591 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/session.py
--rw-r--r--   0 georgy     (501) staff       (20)    15320 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/subscription.py
--rw-r--r--   0 georgy     (501) staff       (20)     3571 2023-12-12 14:17:46.000000 socketshark-0.4.0/socketshark/utils.py
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.149264 socketshark-0.4.0/socketshark.egg-info/
--rw-r--r--   0 georgy     (501) staff       (20)    23367 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/PKG-INFO
--rw-r--r--   0 georgy     (501) staff       (20)      723 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/SOURCES.txt
--rw-r--r--   0 georgy     (501) staff       (20)        1 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/dependency_links.txt
--rw-r--r--   0 georgy     (501) staff       (20)       57 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/entry_points.txt
--rw-r--r--   0 georgy     (501) staff       (20)       49 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/requires.txt
--rw-r--r--   0 georgy     (501) staff       (20)       12 2023-12-13 09:42:54.000000 socketshark-0.4.0/socketshark.egg-info/top_level.txt
-drwxr-xr-x   0 georgy     (501) staff       (20)        0 2023-12-13 09:42:54.148409 socketshark-0.4.0/tests/
--rw-r--r--   0 georgy     (501) staff       (20)    81589 2023-12-12 14:17:46.000000 socketshark-0.4.0/tests/test_basic.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.572247 socketshark-0.5.0/
+-rw-r--r--   0 nsaje      (501) staff       (20)     1089 2024-04-03 07:05:31.000000 socketshark-0.5.0/LICENSE
+-rw-r--r--   0 nsaje      (501) staff       (20)    23270 2024-04-03 10:06:26.572343 socketshark-0.5.0/PKG-INFO
+-rw-r--r--   0 nsaje      (501) staff       (20)    22649 2024-04-03 07:05:31.000000 socketshark-0.5.0/README.rst
+-rw-r--r--   0 nsaje      (501) staff       (20)      141 2024-04-03 07:05:31.000000 socketshark-0.5.0/pyproject.toml
+-rw-r--r--   0 nsaje      (501) staff       (20)     1242 2024-04-03 10:06:26.572939 socketshark-0.5.0/setup.cfg
+-rw-r--r--   0 nsaje      (501) staff       (20)     1377 2024-04-03 10:05:03.000000 socketshark-0.5.0/setup.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.570328 socketshark-0.5.0/socketshark/
+-rw-r--r--   0 nsaje      (501) staff       (20)     8776 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/__init__.py
+-rw-r--r--   0 nsaje      (501) staff       (20)       25 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/__main__.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.571322 socketshark-0.5.0/socketshark/backend/
+-rw-r--r--   0 nsaje      (501) staff       (20)        0 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/backend/__init__.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     4958 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/backend/websockets.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     2390 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/config_defaults.py
+-rw-r--r--   0 nsaje      (501) staff       (20)      888 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/constants.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     5938 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/events.py
+-rw-r--r--   0 nsaje      (501) staff       (20)      297 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/exceptions.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.571739 socketshark-0.5.0/socketshark/metrics/
+-rw-r--r--   0 nsaje      (501) staff       (20)     1467 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/metrics/__init__.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     1005 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/metrics/log.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     1700 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/metrics/prometheus.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     6908 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/receiver.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     1473 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/redis_connection.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     4591 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/session.py
+-rw-r--r--   0 nsaje      (501) staff       (20)    15320 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/subscription.py
+-rw-r--r--   0 nsaje      (501) staff       (20)     3571 2024-04-03 07:05:31.000000 socketshark-0.5.0/socketshark/utils.py
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.571109 socketshark-0.5.0/socketshark.egg-info/
+-rw-r--r--   0 nsaje      (501) staff       (20)    23270 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/PKG-INFO
+-rw-r--r--   0 nsaje      (501) staff       (20)      723 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/SOURCES.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)        1 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/dependency_links.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       57 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/entry_points.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       75 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/requires.txt
+-rw-r--r--   0 nsaje      (501) staff       (20)       12 2024-04-03 10:06:26.000000 socketshark-0.5.0/socketshark.egg-info/top_level.txt
+drwxr-xr-x   0 nsaje      (501) staff       (20)        0 2024-04-03 10:06:26.571999 socketshark-0.5.0/tests/
+-rw-r--r--   0 nsaje      (501) staff       (20)    81589 2024-04-03 07:05:31.000000 socketshark-0.5.0/tests/test_basic.py
```

### Comparing `socketshark-0.4.0/LICENSE` & `socketshark-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/PKG-INFO` & `socketshark-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: socketshark
-Version: 0.4.0
+Version: 0.5.0
 Summary: WebSocket message router
 Home-page: http://github.com/closeio/socketshark
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: prometheus
 License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: aioredis
-Requires-Dist: click
-Requires-Dist: structlog[dev]
-Requires-Dist: websockets
 
 ===========
 SocketShark
 ===========
 .. image:: https://circleci.com/gh/closeio/socketshark/tree/master.svg?style=svg
     :target: https://circleci.com/gh/closeio/socketshark/tree/master
```

### Comparing `socketshark-0.4.0/README.rst` & `socketshark-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/setup.cfg` & `socketshark-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/setup.py` & `socketshark-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,36 +4,39 @@
     long_description = file.read()
 
 
 install_requires = [
     'aiohttp',
     'aioredis',
     'click',
-    'structlog[dev]',
+    'structlog',
     'websockets',
 ]
 
 tests_require = install_requires + [
     'aioresponses',
     'pytest',
     'pytest-asyncio',
     'lintlizard',
 ]
 
 setup(
     name='socketshark',
-    version='0.4.0',
+    version='0.5.0',
     url='http://github.com/closeio/socketshark',
     license='MIT',
     description='WebSocket message router',
     long_description=long_description,
     test_suite='tests',
     tests_require=tests_require,
     platforms='any',
     install_requires=install_requires,
+    extras_require={
+        'prometheus': 'prometheus-async',
+    },
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

### Comparing `socketshark-0.4.0/socketshark/__init__.py` & `socketshark-0.5.0/socketshark/__init__.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/backend/websockets.py` & `socketshark-0.5.0/socketshark/backend/websockets.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/config_defaults.py` & `socketshark-0.5.0/socketshark/config_defaults.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/constants.py` & `socketshark-0.5.0/socketshark/constants.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/events.py` & `socketshark-0.5.0/socketshark/events.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/metrics/__init__.py` & `socketshark-0.5.0/socketshark/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/metrics/log.py` & `socketshark-0.5.0/socketshark/metrics/log.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/metrics/prometheus.py` & `socketshark-0.5.0/socketshark/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/receiver.py` & `socketshark-0.5.0/socketshark/receiver.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/redis_connection.py` & `socketshark-0.5.0/socketshark/redis_connection.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/session.py` & `socketshark-0.5.0/socketshark/session.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/subscription.py` & `socketshark-0.5.0/socketshark/subscription.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark/utils.py` & `socketshark-0.5.0/socketshark/utils.py`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/socketshark.egg-info/PKG-INFO` & `socketshark-0.5.0/socketshark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 2.1
 Name: socketshark
-Version: 0.4.0
+Version: 0.5.0
 Summary: WebSocket message router
 Home-page: http://github.com/closeio/socketshark
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: prometheus
 License-File: LICENSE
-Requires-Dist: aiohttp
-Requires-Dist: aioredis
-Requires-Dist: click
-Requires-Dist: structlog[dev]
-Requires-Dist: websockets
 
 ===========
 SocketShark
 ===========
 .. image:: https://circleci.com/gh/closeio/socketshark/tree/master.svg?style=svg
     :target: https://circleci.com/gh/closeio/socketshark/tree/master
```

### Comparing `socketshark-0.4.0/socketshark.egg-info/SOURCES.txt` & `socketshark-0.5.0/socketshark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socketshark-0.4.0/tests/test_basic.py` & `socketshark-0.5.0/tests/test_basic.py`

 * *Files identical despite different names*

