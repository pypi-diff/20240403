# Comparing `tmp/tg_flask_sse_common-2.0.0.tar.gz` & `tmp/tg_flask_sse_common-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.0.tar", last modified: Tue Apr  2 13:19:30 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.1.tar", last modified: Wed Apr  3 03:19:41 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.0.tar` & `tg_flask_sse_common-2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.532188 tg_flask_sse_common-2.0.0/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:19:30.531958 tg_flask_sse_common-2.0.0/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.0/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 13:19:30.532242 tg_flask_sse_common-2.0.0/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 13:19:14.000000 tg_flask_sse_common-2.0.0/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.531022 tg_flask_sse_common-2.0.0/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 13:19:10.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    19958 2024-04-02 13:18:29.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.531725 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.663114 tg_flask_sse_common-2.0.1/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:19:41.662879 tg_flask_sse_common-2.0.1/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.1/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:19:41.663160 tg_flask_sse_common-2.0.1/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:19:27.000000 tg_flask_sse_common-2.0.1/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.661876 tg_flask_sse_common-2.0.1/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:19:24.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    20591 2024-04-03 03:17:24.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.662611 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,82 +102,89 @@
 
     def release_sse(self, channel):
         """
         移除待释放连接对象
         :param channel: 连接id
         """
         # 移除待释放连接对象
-        release_connect_count = 0
+        release_connect_list = list()
         release_channel_list = list()
 
         sse_connect_list = self.sse_global_clients.get(channel)
         if not sse_connect_list:
             sse_connect_list = []
 
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
-                sse_connect_list.pop(index)
-                release_connect_count += 1
+                release_connect_list.append(index)
 
+        # 清理记录的待释放连接
+        for index in release_connect_list:
+            sse_connect_list.pop(index)
+
+        # 清理记录的频道
         if len(sse_connect_list) == 0:
             self.sse_global_clients.pop(channel)
             release_channel_list.append(channel)
 
-        if release_connect_count > 0 or len(release_channel_list) > 0:
+        if len(release_connect_list) > 0 or len(release_channel_list) > 0:
             print({
                 'title': 'sse-log',
                 'msg': '移除待释放连接/频道',
                 'ln_id': self.local_node_id,
                 'channel': channel,
-                'release_connect_count': release_connect_count,
+                'release_connect_list': release_connect_list,
                 'release_channel_list': release_channel_list,
                 'channel_connect_count': len(sse_connect_list),
                 'channel_count': self.count(),
                 'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
             })
 
     def release_timeout_sse(self):
         """
         移除超时连接对象
         """
         release_channel_list = list()
 
         for _, channel in enumerate(self.sse_global_clients.keys()):
-            release_connect_count = 0
+            release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if sse_connect_list is None:
                 continue
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
-
                 connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
                 if (datetime.now() - connect_time).seconds > self.max_connect_time:
-                    sse_connect_list.pop(index)
-                    release_connect_count += 1
-
-            if len(sse_connect_list) == 0:
-                self.sse_global_clients.pop(channel)
-                release_channel_list.append(channel)
+                    release_connect_list.append(index)
 
-            if release_connect_count > 0:
+            # 清理记录的超时连接
+            if len(release_connect_list) > 0:
+                for index in release_connect_list:
+                    sse_connect_list.pop(index)
                 print({
                     'title': 'sse-log',
                     'msg': '移除超时连接',
                     'ln_id': self.local_node_id,
                     'channel': channel,
-                    'release_connect_count': release_connect_count,
+                    'release_connect_list': release_connect_list,
                     'channel_connect_count': len(sse_connect_list),
                     'channel_count': self.count(),
                     'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
                 })
 
+            if len(sse_connect_list) == 0:
+                release_channel_list.append(channel)
+
+        # 清理记录的频道
         if len(release_channel_list) > 0:
+            for channel in release_channel_list:
+                self.sse_global_clients.pop(channel)
             print({
                 'title': 'sse-log',
                 'msg': '移除超时频道',
                 'ln_id': self.local_node_id,
                 'release_channel_list': release_channel_list,
                 'channel_count': self.count(),
                 'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
@@ -186,45 +193,50 @@
     def release_message_accumulate_sse(self):
         """
         移除消息堆积过多的连接对象
         """
         release_channel_list = list()
 
         for _, channel in enumerate(self.sse_global_clients.keys()):
-            release_connect_count = 0
+            release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
-            if sse_connect_list is None:
-                continue
+            if not sse_connect_list:
+                sse_connect_list = []
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
 
                 message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
                 if len(message_list) > 200:
-                    sse_connect_list.pop(index)
+                    release_connect_list.append(index)
 
-            if len(sse_connect_list) == 0:
-                self.sse_global_clients.pop(channel)
-                release_channel_list.append(channel)
-
-            if release_connect_count > 0:
+            # 清理记录的消息堆积过多连接
+            if len(release_connect_list) > 0:
+                for index in release_connect_list:
+                    sse_connect_list.pop(index)
                 print({
                     'title': 'sse-log',
                     'msg': '移除消息堆积过多连接',
                     'ln_id': self.local_node_id,
                     'channel': channel,
-                    'release_connect_count': release_connect_count,
+                    'release_connect_list': release_connect_list,
                     'channel_connect_count': len(sse_connect_list),
                     'channel_count': self.count(),
                     'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
                 })
 
+            if len(sse_connect_list) == 0:
+                release_channel_list.append(channel)
+
+        # 清理记录的频道
         if len(release_channel_list) > 0:
+            for channel in release_channel_list:
+                self.sse_global_clients.pop(channel)
             print({
                 'title': 'sse-log',
                 'msg': '移除消息堆积过多频道',
                 'ln_id': self.local_node_id,
                 'release_channel_list': release_channel_list,
                 'channel_count': self.count(),
                 'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
@@ -301,21 +313,24 @@
         """
         # 问题:
         # 因为flask是无法主动监听到连接是否关闭的(或者说客户端关闭事件，flask是不会向上抛出异常)，所以需要定时发送心跳包
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
         # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
-        # 3. 每次心跳包时，将检测消息堆积过多的对象
-        self.release_timeout_sse()
-
-        for _, channel in enumerate(self.sse_global_clients.keys()):
-            self.release_sse(channel=channel)
-
-        self.release_message_accumulate_sse()
+        # 3. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
+        try:
+            self.release_message_accumulate_sse()
+
+            self.release_timeout_sse()
+
+            for channel in self.sse_global_clients.keys():
+                self.release_sse(channel=channel)
+        except:
+            pass
 
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
                 channel=channel,
                 message=SseMessage(
                     channel=channel,
```

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

