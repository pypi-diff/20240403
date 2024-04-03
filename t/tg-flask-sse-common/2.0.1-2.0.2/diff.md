# Comparing `tmp/tg_flask_sse_common-2.0.1.tar.gz` & `tmp/tg_flask_sse_common-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-2.0.1.tar", last modified: Wed Apr  3 03:19:41 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.2.tar", last modified: Wed Apr  3 03:40:04 2024, max compression
```

## Comparing `tg_flask_sse_common-2.0.1.tar` & `tg_flask_sse_common-2.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.663114 tg_flask_sse_common-2.0.1/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:19:41.662879 tg_flask_sse_common-2.0.1/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.1/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:19:41.663160 tg_flask_sse_common-2.0.1/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:19:27.000000 tg_flask_sse_common-2.0.1/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.661876 tg_flask_sse_common-2.0.1/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:19:24.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    20591 2024-04-03 03:17:24.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:19:41.662611 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:19:41.000000 tg_flask_sse_common-2.0.1/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.066417 tg_flask_sse_common-2.0.2/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:40:04.066169 tg_flask_sse_common-2.0.2/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.2/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-03 03:40:04.066463 tg_flask_sse_common-2.0.2/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-03 03:40:01.000000 tg_flask_sse_common-2.0.2/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.065155 tg_flask_sse_common-2.0.2/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-03 03:39:58.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    20043 2024-04-03 03:39:47.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-03 03:40:04.065910 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-03 03:40:04.000000 tg_flask_sse_common-2.0.2/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,58 +103,51 @@
     def release_sse(self, channel):
         """
         移除待释放连接对象
         :param channel: 连接id
         """
         # 移除待释放连接对象
         release_connect_list = list()
-        release_channel_list = list()
 
         sse_connect_list = self.sse_global_clients.get(channel)
         if not sse_connect_list:
             sse_connect_list = []
 
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
                 release_connect_list.append(index)
 
         # 清理记录的待释放连接
         for index in release_connect_list:
             sse_connect_list.pop(index)
 
-        # 清理记录的频道
-        if len(sse_connect_list) == 0:
-            self.sse_global_clients.pop(channel)
-            release_channel_list.append(channel)
-
-        if len(release_connect_list) > 0 or len(release_channel_list) > 0:
+        if len(release_connect_list) > 0:
             print({
                 'title': 'sse-log',
-                'msg': '移除待释放连接/频道',
+                'msg': '移除待释放连接',
                 'ln_id': self.local_node_id,
                 'channel': channel,
                 'release_connect_list': release_connect_list,
-                'release_channel_list': release_channel_list,
                 'channel_connect_count': len(sse_connect_list),
                 'channel_count': self.count(),
                 'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
             })
 
     def release_timeout_sse(self):
         """
-        移除超时连接对象
+        移除超时连接对象/频道
         """
         release_channel_list = list()
 
         for _, channel in enumerate(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
-            if sse_connect_list is None:
-                continue
+            if not sse_connect_list:
+                sse_connect_list = []
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
                 connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
                 if (datetime.now() - connect_time).seconds > self.max_connect_time:
                     release_connect_list.append(index)
@@ -176,30 +169,36 @@
 
             if len(sse_connect_list) == 0:
                 release_channel_list.append(channel)
 
         # 清理记录的频道
         if len(release_channel_list) > 0:
             for channel in release_channel_list:
-                self.sse_global_clients.pop(channel)
+                # 清理时，需要重新获取频道下的连接对象，因为在清理过程中，可能有新的连接对象加入
+                sse_connect_list = self.sse_global_clients.get(channel)
+                if not sse_connect_list:
+                    sse_connect_list = []
+
+                # 清理时，确定没有连接对象后再清理
+                if len(sse_connect_list) == 0:
+                    self.sse_global_clients.pop(channel)
+
             print({
                 'title': 'sse-log',
                 'msg': '移除超时频道',
                 'ln_id': self.local_node_id,
                 'release_channel_list': release_channel_list,
                 'channel_count': self.count(),
                 'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
             })
 
     def release_message_accumulate_sse(self):
         """
         移除消息堆积过多的连接对象
         """
-        release_channel_list = list()
-
         for _, channel in enumerate(self.sse_global_clients.keys()):
             release_connect_list = list()
 
             sse_connect_list = self.sse_global_clients.get(channel)
             if not sse_connect_list:
                 sse_connect_list = []
 
@@ -222,30 +221,14 @@
                     'channel': channel,
                     'release_connect_list': release_connect_list,
                     'channel_connect_count': len(sse_connect_list),
                     'channel_count': self.count(),
                     'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
                 })
 
-            if len(sse_connect_list) == 0:
-                release_channel_list.append(channel)
-
-        # 清理记录的频道
-        if len(release_channel_list) > 0:
-            for channel in release_channel_list:
-                self.sse_global_clients.pop(channel)
-            print({
-                'title': 'sse-log',
-                'msg': '移除消息堆积过多频道',
-                'ln_id': self.local_node_id,
-                'release_channel_list': release_channel_list,
-                'channel_count': self.count(),
-                'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
-            })
-
     def disconnect_sse(self, channel, client_id):
         """
         监听到推送消息异常后，可以判断客户端是断开连接
         需注意 :
             这个事件的触发是非实时，所以在执行清理的时候，sse_connect_list中可能存在多个连接对象
         :param channel: 连接id
         :param client_id: 客户端id
@@ -312,23 +295,23 @@
         添加心跳消息到连接对象
         """
         # 问题:
         # 因为flask是无法主动监听到连接是否关闭的(或者说客户端关闭事件，flask是不会向上抛出异常)，所以需要定时发送心跳包
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
-        # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
-        # 3. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
+        # 2. 每次心跳包时，将检测消息堆积过多的对象 (额外兜底)
+        # 3. 每次心跳包时，将清理超时连接对象 (额外兜底)
         try:
             self.release_message_accumulate_sse()
 
-            self.release_timeout_sse()
-
             for channel in self.sse_global_clients.keys():
                 self.release_sse(channel=channel)
+
+            self.release_timeout_sse()
         except:
             pass
 
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
                 channel=channel,
```

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-2.0.1/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.2/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

