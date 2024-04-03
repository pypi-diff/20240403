# Comparing `tmp/dripfeed-client-0.0.2.tar.gz` & `tmp/dripfeed-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dripfeed-client-0.0.2.tar", last modified: Sat Mar 30 08:17:50 2024, max compression
+gzip compressed data, was "dripfeed-client-0.1.0.tar", last modified: Wed Apr  3 18:09:57 2024, max compression
```

## Comparing `dripfeed-client-0.0.2.tar` & `dripfeed-client-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-03-30 08:17:50.586723 dripfeed-client-0.0.2/
--rw-r--r--   0 g          (501) staff       (20)     1071 2024-03-30 08:09:04.000000 dripfeed-client-0.0.2/LICENSE
--rw-r--r--   0 g          (501) staff       (20)      596 2024-03-30 08:17:50.586464 dripfeed-client-0.0.2/PKG-INFO
-drwxr-xr-x   0 g          (501) staff       (20)        0 2024-03-30 08:17:50.586271 dripfeed-client-0.0.2/dripfeed_client.egg-info/
--rw-r--r--   0 g          (501) staff       (20)      596 2024-03-30 08:17:50.000000 dripfeed-client-0.0.2/dripfeed_client.egg-info/PKG-INFO
--rw-r--r--   0 g          (501) staff       (20)      210 2024-03-30 08:17:50.000000 dripfeed-client-0.0.2/dripfeed_client.egg-info/SOURCES.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-03-30 08:17:50.000000 dripfeed-client-0.0.2/dripfeed_client.egg-info/dependency_links.txt
--rw-r--r--   0 g          (501) staff       (20)        9 2024-03-30 08:17:50.000000 dripfeed-client-0.0.2/dripfeed_client.egg-info/requires.txt
--rw-r--r--   0 g          (501) staff       (20)        1 2024-03-30 08:17:50.000000 dripfeed-client-0.0.2/dripfeed_client.egg-info/top_level.txt
--rw-r--r--   0 g          (501) staff       (20)       38 2024-03-30 08:17:50.586763 dripfeed-client-0.0.2/setup.cfg
--rw-r--r--   0 g          (501) staff       (20)      755 2024-03-30 08:11:13.000000 dripfeed-client-0.0.2/setup.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-03 18:09:57.734249 dripfeed-client-0.1.0/
+-rw-r--r--   0 g          (501) staff       (20)     1071 2024-03-30 08:09:04.000000 dripfeed-client-0.1.0/LICENSE
+-rw-r--r--   0 g          (501) staff       (20)      755 2024-04-03 18:09:57.734068 dripfeed-client-0.1.0/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)     1923 2024-03-30 08:36:20.000000 dripfeed-client-0.1.0/dripfeed.py
+drwxr-xr-x   0 g          (501) staff       (20)        0 2024-04-03 18:09:57.733885 dripfeed-client-0.1.0/dripfeed_client.egg-info/
+-rw-r--r--   0 g          (501) staff       (20)      755 2024-04-03 18:09:57.000000 dripfeed-client-0.1.0/dripfeed_client.egg-info/PKG-INFO
+-rw-r--r--   0 g          (501) staff       (20)      222 2024-04-03 18:09:57.000000 dripfeed-client-0.1.0/dripfeed_client.egg-info/SOURCES.txt
+-rw-r--r--   0 g          (501) staff       (20)        1 2024-04-03 18:09:57.000000 dripfeed-client-0.1.0/dripfeed_client.egg-info/dependency_links.txt
+-rw-r--r--   0 g          (501) staff       (20)        9 2024-04-03 18:09:57.000000 dripfeed-client-0.1.0/dripfeed_client.egg-info/requires.txt
+-rw-r--r--   0 g          (501) staff       (20)        9 2024-04-03 18:09:57.000000 dripfeed-client-0.1.0/dripfeed_client.egg-info/top_level.txt
+-rw-r--r--   0 g          (501) staff       (20)       38 2024-04-03 18:09:57.734285 dripfeed-client-0.1.0/setup.cfg
+-rw-r--r--   0 g          (501) staff       (20)      992 2024-04-03 18:07:35.000000 dripfeed-client-0.1.0/setup.py
```

### Comparing `dripfeed-client-0.0.2/LICENSE` & `dripfeed-client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dripfeed-client-0.0.2/PKG-INFO` & `dripfeed-client-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: dripfeed-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: A client for the dripfeed RSS proxy service.
 Home-page: https://github.com/xurble/python-dripfeed-client
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Dripfeed Client
 
 This is a simple python wrapper around the [DripFeed API](https://dripfeed.app/)
```

### Comparing `dripfeed-client-0.0.2/dripfeed_client.egg-info/PKG-INFO` & `dripfeed-client-0.1.0/dripfeed_client.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: dripfeed-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: A client for the dripfeed RSS proxy service.
 Home-page: https://github.com/xurble/python-dripfeed-client
 Author: Gareth Simpson
 Author-email: g@xurble.org
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Dripfeed Client
 
 This is a simple python wrapper around the [DripFeed API](https://dripfeed.app/)
```

