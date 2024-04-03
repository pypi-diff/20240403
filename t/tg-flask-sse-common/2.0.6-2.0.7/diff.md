# Comparing `tmp/tg_flask_sse_common-2.0.6.tar.gz` & `tmp/tg_flask_sse_common-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.6.tar", last modified: Wed Apr  3 05:09:20 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.7.tar", last modified: Wed Apr  3 05:16:54 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.6.tar` & `tg_flask_sse_common-2.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:09:20.935195 tg_flask_sse_common-2.0.6/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 05:09:20.934970 tg_flask_sse_common-2.0.6/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.6/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 05:09:20.935239 tg_flask_sse_common-2.0.6/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 05:09:12.000000 tg_flask_sse_common-2.0.6/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:09:20.934051 tg_flask_sse_common-2.0.6/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 05:09:09.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    20572 2024-04-03 05:07:47.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:09:20.934742 tg_flask_sse_common-2.0.6/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 05:09:20.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 05:09:20.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 05:09:20.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 05:09:20.000000 tg_flask_sse_common-2.0.6/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:16:54.224401 tg_flask_sse_common-2.0.7/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 05:16:54.224165 tg_flask_sse_common-2.0.7/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.7/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 05:16:54.224445 tg_flask_sse_common-2.0.7/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 05:16:48.000000 tg_flask_sse_common-2.0.7/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:16:54.223095 tg_flask_sse_common-2.0.7/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 05:16:44.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    20574 2024-04-03 05:16:34.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 05:16:54.223927 tg_flask_sse_common-2.0.7/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 05:16:54.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 05:16:54.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 05:16:54.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 05:16:54.000000 tg_flask_sse_common-2.0.7/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         release_channel_list = list()
 
         for _, channel in enumerate(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
-                return
+                continue
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
 
                 message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
                 if len(message_list) > 200:
```

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.6/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.7/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

