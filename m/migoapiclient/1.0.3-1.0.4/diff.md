# Comparing `tmp/migoapiclient-1.0.3.tar.gz` & `tmp/migoapiclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "migoapiclient-1.0.3.tar", last modified: Wed Apr  3 08:25:31 2024, max compression
+gzip compressed data, was "migoapiclient-1.0.4.tar", last modified: Wed Apr  3 08:50:10 2024, max compression
```

## Comparing `migoapiclient-1.0.3.tar` & `migoapiclient-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:25:31.772910 migoapiclient-1.0.3/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:25:31.771910 migoapiclient-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:25:31.768910 migoapiclient-1.0.3/migoapiclient/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:07:00.000000 migoapiclient-1.0.3/migoapiclient/__init__.py
--rw-rw-rw-   0        0        0     8452 2024-04-03 07:02:36.000000 migoapiclient-1.0.3/migoapiclient/api_client.py
--rw-rw-rw-   0        0        0      986 2024-04-03 04:05:29.000000 migoapiclient-1.0.3/migoapiclient/file_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:25:31.771910 migoapiclient-1.0.3/migoapiclient.egg-info/
--rw-rw-rw-   0        0        0     3900 2024-04-03 08:25:31.000000 migoapiclient-1.0.3/migoapiclient.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:25:31.000000 migoapiclient-1.0.3/migoapiclient.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:25:31.000000 migoapiclient-1.0.3/migoapiclient.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-03 08:25:31.000000 migoapiclient-1.0.3/migoapiclient.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:25:31.772910 migoapiclient-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     3898 2024-04-03 08:24:43.000000 migoapiclient-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:25:31.770910 migoapiclient-1.0.3/src/
--rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.3/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3288 2024-04-03 07:12:56.000000 migoapiclient-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.753846 migoapiclient-1.0.4/migoapiclient/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:07:00.000000 migoapiclient-1.0.4/migoapiclient/__init__.py
+-rw-rw-rw-   0        0        0     9834 2024-04-03 08:48:29.000000 migoapiclient-1.0.4/migoapiclient/api_client.py
+-rw-rw-rw-   0        0        0      986 2024-04-03 04:05:29.000000 migoapiclient-1.0.4/migoapiclient/file_manager.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.757395 migoapiclient-1.0.4/migoapiclient.egg-info/
+-rw-rw-rw-   0        0        0     3900 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-03 08:50:10.000000 migoapiclient-1.0.4/migoapiclient.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:50:10.758402 migoapiclient-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     3940 2024-04-03 08:50:05.000000 migoapiclient-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:10.756891 migoapiclient-1.0.4/src/
+-rw-rw-rw-   0        0        0        0 2024-04-03 08:01:08.000000 migoapiclient-1.0.4/src/__init__.py
```

### Comparing `migoapiclient-1.0.3/PKG-INFO` & `migoapiclient-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.3/README.md` & `migoapiclient-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.3/migoapiclient/api_client.py` & `migoapiclient-1.0.4/migoapiclient/api_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime
 
 from dateutil.tz import tz
 
 from file_manager import LogFileManager
 import time
 import requests
+
 ERROR_MSG = """
 ---------------------------------- {0} begin ----------------------------------
 请求URL是：{1}
 请求headers是：{2}
 请求params是：{3}
 请求post是：{4}
 错误信息是：{5}
@@ -152,30 +153,30 @@
 
     def get_node_info_list(self, migo_shop_id: int):
         """
         获取节点信息列表
         :param migo_shop_id 米果店铺ID
         """
         post_data = {
-          "nodeConfigId": self.node_id,
-          "shopId": migo_shop_id
+            "nodeConfigId": self.node_id,
+            "shopId": migo_shop_id
         }
         uri = f'/data-collection-service/node/search'
         return self.try_post(self.host + uri, json=post_data)
 
     def post_auth_data(self, migo_shop_id, **kwargs):
         """
         刷新认证数据
         :param migo_shop_id 米果店铺ID
         :param kwargs 所需的认证参数
         """
         post_data = {
-          "crawlData": json.dumps(kwargs),
-          "nodeConfigId": self.node_id,
-          "shopId": migo_shop_id
+            "crawlData": json.dumps(kwargs),
+            "nodeConfigId": self.node_id,
+            "shopId": migo_shop_id
         }
         uri = '/data-collection-service/node/refresh'
         return self.try_post(self.host + uri, json=post_data)
 
     def post_crawl_data(self, crawl_data: dict):
         """
         推送采集数据
@@ -214,17 +215,51 @@
                     "id": str(time.time()).replace('.', ''),
                     "shopId": shop_id,
                     "nodeId": node_id,
                     "dataType": data_type,
                     "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
                     "logData": json.dumps(log_data),
                     "logParams": json.dumps(log_params),
-                    "logStack": "",
+                    "logStack": log_stack,
                     "logMsg": error_msg
                 }
             ],
             "primaryKey": "id",
             "refreshNow": 0,
             "tableName": "log_node_spider_error"
         }
         response_data = self.try_post(self.host + uri, 0, json=post_data)
         return response_data
+
+    def post_info_log(self, msg: str, data_type: str, node_id: str, shop_id: str, log_data: dict = None,
+                      log_params: dict = None, log_stack: str = None):
+        """
+        上传日志
+        :param msg 错误信息
+        :param data_type 数据类型
+        :param node_id 节点ID
+        :param shop_id 店铺ID
+        :param log_data 请求的post参数
+        :param log_params 请求的get参数
+        :param log_stack 日志其他信息
+        """
+        uri = '/data-collection-service/node/logsave'
+        post_data = {
+            "data": [
+                {
+                    "id": str(time.time()).replace('.', ''),
+                    "shopId": shop_id,
+                    "nodeId": node_id,
+                    "dataType": data_type,
+                    "logTime": str(datetime.fromtimestamp(int(time.time()), tz.gettz('Asia/Shanghai'))),
+                    "logData": json.dumps(log_data),
+                    "logParams": json.dumps(log_params),
+                    "logStack": log_stack,
+                    "logMsg": msg
+                }
+            ],
+            "primaryKey": "id",
+            "refreshNow": 0,
+            "tableName": "log_node_spider"
+        }
+        response_data = self.try_post(self.host + uri, 0, json=post_data)
+        return response_data
```

### Comparing `migoapiclient-1.0.3/migoapiclient/file_manager.py` & `migoapiclient-1.0.4/migoapiclient/file_manager.py`

 * *Files identical despite different names*

### Comparing `migoapiclient-1.0.3/migoapiclient.egg-info/PKG-INFO` & `migoapiclient-1.0.4/migoapiclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: migoapiclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: 米果请求API客户端
 Home-page: https://github.com/me/myproject
 Author: pykira
 Author-email: 2920167524@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `migoapiclient-1.0.3/setup.py` & `migoapiclient-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'migoapiclient'
 DESCRIPTION = '米果请求API客户端'
 URL = 'https://github.com/me/myproject'
 EMAIL = '2920167524@qq.com'
 AUTHOR = 'pykira'
 REQUIRES_PYTHON = '>=3.5.0'
-VERSION = '1.0.3'
+VERSION = input('请输入程序版本，例如：1.0.3\n')
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

