# Comparing `tmp/tg_flask_sse_common-2.0.2.tar.gz` & `tmp/tg_flask_sse_common-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.2.tar", last modified: Wed Apr  3 03:40:04 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.3.tar", last modified: Wed Apr  3 03:47:45 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.2.tar` & `tg_flask_sse_common-2.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.066417 tg_flask_sse_common-2.0.2/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:40:04.066169 tg_flask_sse_common-2.0.2/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.2/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:40:04.066463 tg_flask_sse_common-2.0.2/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:40:01.000000 tg_flask_sse_common-2.0.2/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.065155 tg_flask_sse_common-2.0.2/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:39:58.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    20043 2024-04-03 03:39:47.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.065910 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.863124 tg_flask_sse_common-2.0.3/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:47:45.862879 tg_flask_sse_common-2.0.3/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.3/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:47:45.863179 tg_flask_sse_common-2.0.3/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:47:28.000000 tg_flask_sse_common-2.0.3/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.861870 tg_flask_sse_common-2.0.3/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:47:26.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19983 2024-04-03 03:47:19.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:47:45.862634 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:47:45.000000 tg_flask_sse_common-2.0.3/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,14 +210,15 @@
                 if len(message_list) > 200:
                     release_connect_list.append(index)
 
             # 清理记录的消息堆积过多连接
             if len(release_connect_list) > 0:
                 for index in release_connect_list:
                     sse_connect_list.pop(index)
+
                 print({
                     'title': 'sse-log',
                     'msg': '移除消息堆积过多连接',
                     'ln_id': self.local_node_id,
                     'channel': channel,
                     'release_connect_list': release_connect_list,
                     'channel_connect_count': len(sse_connect_list),
@@ -297,23 +298,21 @@
         # 问题:
         # 因为flask是无法主动监听到连接是否关闭的(或者说客户端关闭事件，flask是不会向上抛出异常)，所以需要定时发送心跳包
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
         # 2. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
         # 3. 每次心跳包时，将清理超时连接对象 (额外兜底)
-        try:
-            self.release_message_accumulate_sse()
 
-            for channel in self.sse_global_clients.keys():
-                self.release_sse(channel=channel)
+        self.release_message_accumulate_sse()
+
+        for channel in self.sse_global_clients.keys():
+            self.release_sse(channel=channel)
 
-            self.release_timeout_sse()
-        except:
-            pass
+        self.release_timeout_sse()
 
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
                 channel=channel,
                 message=SseMessage(
                     channel=channel,
```

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.3/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

