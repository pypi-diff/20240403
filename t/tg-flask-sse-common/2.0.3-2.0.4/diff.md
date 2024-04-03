# Comparing `tmp/tg_flask_sse_common-2.0.3.tar.gz` & `tmp/tg_flask_sse_common-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.3.tar", last modified: Wed Apr  3 03:47:45 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.4.tar", last modified: Wed Apr  3 03:50:34 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.3.tar` & `tg_flask_sse_common-2.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.863124 tg_flask_sse_common-2.0.3/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:47:45.862879 tg_flask_sse_common-2.0.3/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.3/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:47:45.863179 tg_flask_sse_common-2.0.3/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:47:28.000000 tg_flask_sse_common-2.0.3/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.861870 tg_flask_sse_common-2.0.3/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:47:26.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    19983 2024-04-03 03:47:19.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.862634 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.920803 tg_flask_sse_common-2.0.4/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:50:34.920562 tg_flask_sse_common-2.0.4/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.4/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:50:34.920848 tg_flask_sse_common-2.0.4/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:50:24.000000 tg_flask_sse_common-2.0.4/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.919577 tg_flask_sse_common-2.0.4/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:50:21.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    20008 2024-04-03 03:50:02.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.920323 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,22 +169,22 @@
 
             if len(sse_connect_list) == 0:
                 release_channel_list.append(channel)
 
         # 清理记录的频道
         if len(release_channel_list) > 0:
             for channel in release_channel_list:
-                # 清理时，需要重新获取频道下的连接对象，因为在清理过程中，可能有新的连接对象加入
-                sse_connect_list = self.sse_global_clients.get(channel)
-                if not sse_connect_list:
-                    sse_connect_list = []
-
-                # 清理时，确定没有连接对象后再清理
-                if len(sse_connect_list) == 0:
-                    self.sse_global_clients.pop(channel)
+                # # 清理时，需要重新获取频道下的连接对象，因为在清理过程中，可能有新的连接对象加入
+                # sse_connect_list = self.sse_global_clients.get(channel)
+                # if not sse_connect_list:
+                #     sse_connect_list = []
+                #
+                # # 清理时，确定没有连接对象后再清理
+                # if len(sse_connect_list) == 0:
+                self.sse_global_clients.pop(channel)
 
             print({
                 'title': 'sse-log',
                 'msg': '移除超时频道',
                 'ln_id': self.local_node_id,
                 'release_channel_list': release_channel_list,
                 'channel_count': self.count(),
```

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

