# Comparing `tmp/tg_flask_sse_common-2.0.4.tar.gz` & `tmp/tg_flask_sse_common-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.4.tar", last modified: Wed Apr  3 03:50:34 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.5.tar", last modified: Wed Apr  3 04:53:01 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.4.tar` & `tg_flask_sse_common-2.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.920803 tg_flask_sse_common-2.0.4/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:50:34.920562 tg_flask_sse_common-2.0.4/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.4/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:50:34.920848 tg_flask_sse_common-2.0.4/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:50:24.000000 tg_flask_sse_common-2.0.4/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.919577 tg_flask_sse_common-2.0.4/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:50:21.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    20008 2024-04-03 03:50:02.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:50:34.920323 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:50:34.000000 tg_flask_sse_common-2.0.4/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 04:53:01.274782 tg_flask_sse_common-2.0.5/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 04:53:01.274534 tg_flask_sse_common-2.0.5/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.5/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 04:53:01.274829 tg_flask_sse_common-2.0.5/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 04:52:50.000000 tg_flask_sse_common-2.0.5/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 04:53:01.273192 tg_flask_sse_common-2.0.5/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 04:52:47.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19865 2024-04-03 04:52:32.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 04:53:01.274212 tg_flask_sse_common-2.0.5/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 04:53:01.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 04:53:01.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 04:53:01.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 04:53:01.000000 tg_flask_sse_common-2.0.5/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         :param channel: 连接id
         """
         # 移除待释放连接对象
         release_connect_list = list()
 
         sse_connect_list = self.sse_global_clients.get(channel)
         if not sse_connect_list:
-            sse_connect_list = []
+            return
 
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
                 release_connect_list.append(index)
 
         # 清理记录的待释放连接
         for index in release_connect_list:
@@ -139,19 +139,20 @@
         release_channel_list = list()
 
         for _, channel in enumerate(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
-                sse_connect_list = []
+                continue
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
+
                 connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
                 if (datetime.now() - connect_time).seconds > self.max_connect_time:
                     release_connect_list.append(index)
 
             # 清理记录的超时连接
             if len(release_connect_list) > 0:
                 for index in release_connect_list:
@@ -169,22 +170,21 @@
 
             if len(sse_connect_list) == 0:
                 release_channel_list.append(channel)
 
         # 清理记录的频道
         if len(release_channel_list) > 0:
             for channel in release_channel_list:
-                # # 清理时，需要重新获取频道下的连接对象，因为在清理过程中，可能有新的连接对象加入
-                # sse_connect_list = self.sse_global_clients.get(channel)
-                # if not sse_connect_list:
-                #     sse_connect_list = []
-                #
-                # # 清理时，确定没有连接对象后再清理
-                # if len(sse_connect_list) == 0:
-                self.sse_global_clients.pop(channel)
+                # 清理时，需要重新获取频道下的连接对象，因为在清理过程中，可能有新的连接对象加入
+                sse_connect_list = self.sse_global_clients.get(channel)
+                if not sse_connect_list:
+                    sse_connect_list = []
+
+                if len(sse_connect_list) == 0:
+                    self.sse_global_clients.pop(channel)
 
             print({
                 'title': 'sse-log',
                 'msg': '移除超时频道',
                 'ln_id': self.local_node_id,
                 'release_channel_list': release_channel_list,
                 'channel_count': self.count(),
@@ -196,15 +196,15 @@
         移除消息堆积过多的连接对象
         """
         for _, channel in enumerate(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
-                sse_connect_list = []
+                continue
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
 
                 message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
                 if len(message_list) > 200:
@@ -290,29 +290,28 @@
             })
 
         self.sse_global_clients[channel] = sse_connect_list
 
     def add_heartbeat(self):
         """
         添加心跳消息到连接对象
-        """
         # 问题:
         # 因为flask是无法主动监听到连接是否关闭的(或者说客户端关闭事件，flask是不会向上抛出异常)，所以需要定时发送心跳包
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
-        #
-        # 1. 每次心跳包时，将清理已经关闭的连接对象
-        # 2. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
-        # 3. 每次心跳包时，将清理超时连接对象 (额外兜底)
+        """
 
-        self.release_message_accumulate_sse()
+        # 1. 每次心跳包时，将清理已经关闭的连接对象
+        self.release_timeout_sse()
 
+        # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
         for channel in self.sse_global_clients.keys():
             self.release_sse(channel=channel)
 
-        self.release_timeout_sse()
+        # 3. 每次心跳包时，将检测消息堆积过多的对象(额外兜底)
+        self.release_message_accumulate_sse()
 
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
                 channel=channel,
                 message=SseMessage(
                     channel=channel,
```

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.4/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.5/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

