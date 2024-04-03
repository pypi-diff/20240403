# Comparing `tmp/yandex_tracker_client-2.6.tar.gz` & `tmp/yandex_tracker_client-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yandex_tracker_client-2.6.tar", last modified: Tue Aug  1 20:35:08 2023, max compression
+gzip compressed data, was "dist/yandex_tracker_client-2.7.tar", last modified: Wed Apr  3 20:19:36 2024, max compression
```

## Comparing `yandex_tracker_client-2.6.tar` & `yandex_tracker_client-2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client/
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/__init__.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/client.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    37008 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/collections.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8175 2023-08-01 05:36:59.000000 yandex_tracker_client-2.6/yandex_tracker_client/connection.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/exceptions.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7480 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/objects.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/settings.py
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2023-04-28 20:02:24.000000 yandex_tracker_client-2.6/yandex_tracker_client/uriutils.py
-drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      519 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/SOURCES.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/dependency_links.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       52 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/requires.txt
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/yandex_tracker_client.egg-info/top_level.txt
--rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     9249 2023-08-01 05:36:59.000000 yandex_tracker_client-2.6/README.rst
--rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1520 2023-08-01 20:35:02.000000 yandex_tracker_client-2.6/setup.py
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/PKG-INFO
--rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2023-08-01 20:35:08.000000 yandex_tracker_client-2.6/setup.cfg
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       80 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/__init__.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     2394 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/client.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)    37008 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/collections.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     8907 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/connection.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     3337 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/exceptions.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     7480 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/objects.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)       93 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/settings.py
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     1096 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client/uriutils.py
+drwxr-xr-x   0 smosker  (346405873) LD\Domain Users (593637566)        0 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      519 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/SOURCES.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)        1 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/dependency_links.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      119 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/requires.txt
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       22 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/yandex_tracker_client.egg-info/top_level.txt
+-rw-rw-r--   0 smosker  (346405873) LD\Domain Users (593637566)     9249 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/README.rst
+-rwxrwxr-x   0 smosker  (346405873) LD\Domain Users (593637566)     1508 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/setup.py
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)      746 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/PKG-INFO
+-rw-r--r--   0 smosker  (346405873) LD\Domain Users (593637566)       38 2024-04-03 20:19:36.000000 yandex_tracker_client-2.7/setup.cfg
```

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/client.py` & `yandex_tracker_client-2.7/yandex_tracker_client/client.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/collections.py` & `yandex_tracker_client-2.7/yandex_tracker_client/collections.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/connection.py` & `yandex_tracker_client-2.7/yandex_tracker_client/connection.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # coding: utf-8
 
 import logging
 import requests
 import json
+import time
 
 try:
     from requests.utils import check_header_validity
 except:
     # For compatibility with requests version < 2.11
     check_header_validity = lambda header: True
 
@@ -33,14 +34,17 @@
 
     def __init__(self,
                  token=None,
                  org_id=None,
                  base_url="https://api.tracker.yandex.net",
                  timeout=10,
                  retries=10,
+                 retries_initial_delay=0,
+                 retries_delay_multiplier=1,
+                 retries_delay_upper_limit=0,
                  headers=None,
                  api_version=VERSION_V2,
                  verify=True,
                  cloud_org_id=None,
                  iam_token=None,
                  ):
 
@@ -71,14 +75,17 @@
         for header in self.session.headers.items():
             check_header_validity(header)
 
         self.base_url = base_url
         self.api_version = api_version
         self.timeout = timeout
         self.retries = retries
+        self.retries_initial_delay = retries_initial_delay
+        self.retries_delay_multiplier = retries_delay_multiplier
+        self.retries_delay_upper_limit = retries_delay_upper_limit
 
     get = bind_method('GET')
     put = bind_method('PUT')
     post = bind_method('POST')
     patch = bind_method('PATCH')
     delete = bind_method('DELETE')
 
@@ -145,30 +152,41 @@
         )
 
     def _try_request(self, **kwargs):
         response = None
         exception = None
         iterations = max(self.retries + 1, 1)
 
+        retry_delay = self.retries_initial_delay
+        multiplier = self.retries_delay_multiplier
+        limit = self.retries_delay_upper_limit
+
         for retry in range(iterations):
             try:
                 response = self.session.request(**kwargs)
             except Exception as e:
                 exception = e
             else:
                 exception = None
-                if 500 <= response.status_code < 600:
+                if 500 <= response.status_code < 600 or response.status_code == 429 and retry_delay > 0:
                     logger.warning(
                         "Request failed with status %d, retrying (%d)...",
                         response.status_code, retry
                     )
                     self._log_error(logging.WARNING, response)
                 else:
                     break
-            # XXX: sleep?
+
+            if retry_delay > 0:
+                time.sleep(retry_delay)
+
+            if multiplier > 1:
+                retry_delay *= multiplier
+            if 0 < limit < retry_delay:
+                retry_delay = limit
 
         if exception is not None:
             raise exceptions.TrackerRequestError(exception)
         elif 500 <= response.status_code < 600:
             raise exceptions.OutOfRetries(response)
         elif 400 <= response.status_code < 500:
             self._log_error(logging.ERROR, response)
```

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/exceptions.py` & `yandex_tracker_client-2.7/yandex_tracker_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/objects.py` & `yandex_tracker_client-2.7/yandex_tracker_client/objects.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client/uriutils.py` & `yandex_tracker_client-2.7/yandex_tracker_client/uriutils.py`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client.egg-info/PKG-INFO` & `yandex_tracker_client-2.7/yandex_tracker_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex-tracker-client
-Version: 2.6
+Version: 2.7
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

### Comparing `yandex_tracker_client-2.6/yandex_tracker_client.egg-info/SOURCES.txt` & `yandex_tracker_client-2.7/yandex_tracker_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/README.rst` & `yandex_tracker_client-2.7/README.rst`

 * *Files identical despite different names*

### Comparing `yandex_tracker_client-2.6/setup.py` & `yandex_tracker_client-2.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,33 +2,28 @@
 
 import codecs
 import os
 import sys
 
 from setuptools import setup
 
-if sys.version_info.major < 3:
-    stools = 'setuptools<=42.0.2'
-else:
-    stools = 'setuptools'
-
 # Utility function to read the README file.
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='yandex_tracker_client',
-    version='2.6',
+    version='2.7',
     description='Client for Yandex.Tracker',
     author='Yandex Team',
     author_email='smosker@yandex-team.ru',
     url='https://github.com/yandex/yandex_tracker_client',
     long_description='',
     packages=['yandex_tracker_client'],
     classifiers=['Development Status :: 5 - Production/Stable',
@@ -40,11 +35,12 @@
                  'Programming Language :: Python :: 3',
                  'Programming Language :: Python :: 2',
                  ],
     keywords='python yandex.tracker api-client',
     python_requires='>=2.7',
     install_requires=[
         'requests[security]>=2.0',
-        stools,
+        'setuptools<=42.0.2; python_version <= "2.7"',
+        'setuptools; python_version >= "3.4"',
         'six>=1.9',
     ]
 )
```

### Comparing `yandex_tracker_client-2.6/PKG-INFO` & `yandex_tracker_client-2.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: yandex_tracker_client
-Version: 2.6
+Version: 2.7
 Summary: Client for Yandex.Tracker
 Home-page: https://github.com/yandex/yandex_tracker_client
 Author: Yandex Team
 Author-email: smosker@yandex-team.ru
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python yandex.tracker api-client
```

