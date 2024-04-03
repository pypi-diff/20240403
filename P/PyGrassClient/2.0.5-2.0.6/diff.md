# Comparing `tmp/PyGrassClient-2.0.5.tar.gz` & `tmp/PyGrassClient-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGrassClient-2.0.5.tar", last modified: Fri Mar 29 19:12:00 2024, max compression
+gzip compressed data, was "PyGrassClient-2.0.6.tar", last modified: Wed Apr  3 03:27:46 2024, max compression
```

## Comparing `PyGrassClient-2.0.5.tar` & `PyGrassClient-2.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:12:00.918540 PyGrassClient-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-29 19:12:00.918540 PyGrassClient-2.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:12:00.918540 PyGrassClient-2.0.5/PyGrassClient/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/PyGrassClient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/PyGrassClient/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/PyGrassClient/_async_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/PyGrassClient/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/PyGrassClient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:12:00.918540 PyGrassClient-2.0.5/PyGrassClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-29 19:12:00.000000 PyGrassClient-2.0.5/PyGrassClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-29 19:12:00.000000 PyGrassClient-2.0.5/PyGrassClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:12:00.000000 PyGrassClient-2.0.5/PyGrassClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-29 19:12:00.000000 PyGrassClient-2.0.5/PyGrassClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-29 19:12:00.000000 PyGrassClient-2.0.5/PyGrassClient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:12:00.918540 PyGrassClient-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-29 19:11:57.000000 PyGrassClient-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:27:46.822469 PyGrassClient-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-03 03:27:46.822469 PyGrassClient-2.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:27:46.822469 PyGrassClient-2.0.6/PyGrassClient/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/PyGrassClient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/PyGrassClient/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/PyGrassClient/_async_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6403 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/PyGrassClient/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/PyGrassClient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:27:46.822469 PyGrassClient-2.0.6/PyGrassClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-03 03:27:46.000000 PyGrassClient-2.0.6/PyGrassClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 03:27:46.000000 PyGrassClient-2.0.6/PyGrassClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:27:46.000000 PyGrassClient-2.0.6/PyGrassClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 03:27:46.000000 PyGrassClient-2.0.6/PyGrassClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 03:27:46.000000 PyGrassClient-2.0.6/PyGrassClient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:27:46.822469 PyGrassClient-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-03 03:27:40.000000 PyGrassClient-2.0.6/setup.py
```

### Comparing `PyGrassClient-2.0.5/LICENSE` & `PyGrassClient-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGrassClient-2.0.5/PKG-INFO` & `PyGrassClient-2.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGrassClient
-Version: 2.0.5
+Version: 2.0.6
 Summary: Get Grass Python Package
 Home-page: https://github.com/Confusion-ymc/PyGrassClient
 Author: confusion
 Author-email: 1107238486@qq.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Confusion-ymc/PyGrassClient
 Project-URL: Source, https://github.com/Confusion-ymc/PyGrassClient
@@ -64,15 +64,21 @@
 - 不配置代理
   - **每一行是一个账号配置** 
   - **没有代理则直接是`user_id`为一行，----- 格式为`5242367b-d366-1234-987a-9ebd303fa8f5`**
   - **如果不知道`user_id`, 就用账号和密码----格式为`test@qq.com---Aa@password`**
 - 配置代理
   - **如果使用代理则在后面加上`==代理连接`----格式为`5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080`**
 
-
 - 例如：
  ```text
 5242367b-d366-1234-987a-9ebd303fa8f5==http://proxy.com:8080
 5242367b-d366-1234-987a-9ebd303fa8f5
 test@qq.com---Aa@password 
 5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080
  ```
+
+### 5.获取 UserID
+ ```python
+from PyGrassClient import PyGrassClient
+
+PyGrassClient(user_name="example@gmail.com", password='your—password').get_user_id()
+```
```

### Comparing `PyGrassClient-2.0.5/PyGrassClient/_async_core.py` & `PyGrassClient-2.0.6/PyGrassClient/_async_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,18 @@
                 send_message = json.dumps(
                     {"id": str(uuid.uuid4()), "version": "1.0.0", "action": "PING", "data": {}})
                 if self.ws:
                     self.log(DEBUG, f'[发送消息] [{self.user_id}] [{self.proxy_url}] [{send_message}]')
                     await self.ws.send(send_message)
             except Exception as e:
                 self.log(DEBUG, f'[PING Error] {e}')
-            await asyncio.sleep(20)
+            for i in range(20):
+                if self._stop:
+                    break
+                await asyncio.sleep(1)
         self._ping_stopped = True
 
     def auth_response(self, message):
         return {
             "id": message["id"],
             "origin_action": "AUTH",
             "result": {
```

### Comparing `PyGrassClient-2.0.5/PyGrassClient/utils.py` & `PyGrassClient-2.0.6/PyGrassClient/utils.py`

 * *Files identical despite different names*

### Comparing `PyGrassClient-2.0.5/PyGrassClient.egg-info/PKG-INFO` & `PyGrassClient-2.0.6/PyGrassClient.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGrassClient
-Version: 2.0.5
+Version: 2.0.6
 Summary: Get Grass Python Package
 Home-page: https://github.com/Confusion-ymc/PyGrassClient
 Author: confusion
 Author-email: 1107238486@qq.com
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/Confusion-ymc/PyGrassClient
 Project-URL: Source, https://github.com/Confusion-ymc/PyGrassClient
@@ -64,15 +64,21 @@
 - 不配置代理
   - **每一行是一个账号配置** 
   - **没有代理则直接是`user_id`为一行，----- 格式为`5242367b-d366-1234-987a-9ebd303fa8f5`**
   - **如果不知道`user_id`, 就用账号和密码----格式为`test@qq.com---Aa@password`**
 - 配置代理
   - **如果使用代理则在后面加上`==代理连接`----格式为`5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080`**
 
-
 - 例如：
  ```text
 5242367b-d366-1234-987a-9ebd303fa8f5==http://proxy.com:8080
 5242367b-d366-1234-987a-9ebd303fa8f5
 test@qq.com---Aa@password 
 5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080
  ```
+
+### 5.获取 UserID
+ ```python
+from PyGrassClient import PyGrassClient
+
+PyGrassClient(user_name="example@gmail.com", password='your—password').get_user_id()
+```
```

### Comparing `PyGrassClient-2.0.5/README.md` & `PyGrassClient-2.0.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -36,15 +36,21 @@
 - 不配置代理
   - **每一行是一个账号配置** 
   - **没有代理则直接是`user_id`为一行，----- 格式为`5242367b-d366-1234-987a-9ebd303fa8f5`**
   - **如果不知道`user_id`, 就用账号和密码----格式为`test@qq.com---Aa@password`**
 - 配置代理
   - **如果使用代理则在后面加上`==代理连接`----格式为`5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080`**
 
-
 - 例如：
  ```text
 5242367b-d366-1234-987a-9ebd303fa8f5==http://proxy.com:8080
 5242367b-d366-1234-987a-9ebd303fa8f5
 test@qq.com---Aa@password 
 5242367b-d366-1258-987a-9ebd303fa8f5==socks5://proxy.com:1080
- ```
+ ```
+
+### 5.获取 UserID
+ ```python
+from PyGrassClient import PyGrassClient
+
+PyGrassClient(user_name="example@gmail.com", password='your—password').get_user_id()
+```
```

### Comparing `PyGrassClient-2.0.5/setup.py` & `PyGrassClient-2.0.6/setup.py`

 * *Files identical despite different names*

