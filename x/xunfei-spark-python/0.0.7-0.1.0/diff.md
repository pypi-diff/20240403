# Comparing `tmp/xunfei-spark-python-0.0.7.tar.gz` & `tmp/xunfei-spark-python-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xunfei-spark-python-0.0.7.tar", last modified: Sat Mar 30 15:57:41 2024, max compression
+gzip compressed data, was "xunfei-spark-python-0.1.0.tar", last modified: Wed Apr  3 01:31:36 2024, max compression
```

## Comparing `xunfei-spark-python-0.0.7.tar` & `xunfei-spark-python-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-03-30 15:57:41.037317 xunfei-spark-python-0.0.7/
--rw-r--r--   0 sunminghui   (501) staff       (20)     3044 2024-03-30 15:57:41.036846 xunfei-spark-python-0.0.7/PKG-INFO
--rw-r--r--   0 sunminghui   (501) staff       (20)     2371 2024-03-30 15:57:26.000000 xunfei-spark-python-0.0.7/README.md
--rw-r--r--   0 sunminghui   (501) staff       (20)       38 2024-03-30 15:57:41.037425 xunfei-spark-python-0.0.7/setup.cfg
--rw-r--r--   0 sunminghui   (501) staff       (20)     3802 2024-03-30 15:57:26.000000 xunfei-spark-python-0.0.7/setup.py
-drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-03-30 15:57:41.031530 xunfei-spark-python-0.0.7/xunfei/
--rw-r--r--   0 sunminghui   (501) staff       (20)      122 2024-03-16 15:50:25.000000 xunfei-spark-python-0.0.7/xunfei/__init__.py
-drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-03-30 15:57:41.033514 xunfei-spark-python-0.0.7/xunfei/spark/
--rw-r--r--   0 sunminghui   (501) staff       (20)        0 2024-03-16 12:39:53.000000 xunfei-spark-python-0.0.7/xunfei/spark/__init__.py
--rw-r--r--   0 sunminghui   (501) staff       (20)     7140 2024-03-30 15:44:29.000000 xunfei-spark-python-0.0.7/xunfei/spark/client.py
--rw-r--r--   0 sunminghui   (501) staff       (20)      336 2024-03-16 12:57:49.000000 xunfei-spark-python-0.0.7/xunfei/spark/response.py
-drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-03-30 15:57:41.036268 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/
--rw-r--r--   0 sunminghui   (501) staff       (20)     3044 2024-03-30 15:57:40.000000 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/PKG-INFO
--rw-r--r--   0 sunminghui   (501) staff       (20)      324 2024-03-30 15:57:40.000000 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/SOURCES.txt
--rw-r--r--   0 sunminghui   (501) staff       (20)        1 2024-03-30 15:57:40.000000 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/dependency_links.txt
--rw-r--r--   0 sunminghui   (501) staff       (20)       24 2024-03-30 15:57:40.000000 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/requires.txt
--rw-r--r--   0 sunminghui   (501) staff       (20)        7 2024-03-30 15:57:40.000000 xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/top_level.txt
+drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-04-03 01:31:36.981806 xunfei-spark-python-0.1.0/
+-rw-r--r--   0 sunminghui   (501) staff       (20)     3102 2024-04-03 01:31:36.981290 xunfei-spark-python-0.1.0/PKG-INFO
+-rw-r--r--   0 sunminghui   (501) staff       (20)     2429 2024-04-03 01:29:21.000000 xunfei-spark-python-0.1.0/README.md
+-rw-r--r--   0 sunminghui   (501) staff       (20)       38 2024-04-03 01:31:36.981931 xunfei-spark-python-0.1.0/setup.cfg
+-rw-r--r--   0 sunminghui   (501) staff       (20)     3802 2024-04-03 01:29:21.000000 xunfei-spark-python-0.1.0/setup.py
+drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-04-03 01:31:36.974235 xunfei-spark-python-0.1.0/xunfei/
+-rw-r--r--   0 sunminghui   (501) staff       (20)      122 2024-03-16 15:50:25.000000 xunfei-spark-python-0.1.0/xunfei/__init__.py
+drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-04-03 01:31:36.975979 xunfei-spark-python-0.1.0/xunfei/spark/
+-rw-r--r--   0 sunminghui   (501) staff       (20)        0 2024-03-16 12:39:53.000000 xunfei-spark-python-0.1.0/xunfei/spark/__init__.py
+-rw-r--r--   0 sunminghui   (501) staff       (20)     7179 2024-04-03 01:27:31.000000 xunfei-spark-python-0.1.0/xunfei/spark/client.py
+-rw-r--r--   0 sunminghui   (501) staff       (20)      336 2024-03-16 12:57:49.000000 xunfei-spark-python-0.1.0/xunfei/spark/response.py
+drwxr-xr-x   0 sunminghui   (501) staff       (20)        0 2024-04-03 01:31:36.980383 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/
+-rw-r--r--   0 sunminghui   (501) staff       (20)     3102 2024-04-03 01:31:36.000000 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/PKG-INFO
+-rw-r--r--   0 sunminghui   (501) staff       (20)      324 2024-04-03 01:31:36.000000 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 sunminghui   (501) staff       (20)        1 2024-04-03 01:31:36.000000 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 sunminghui   (501) staff       (20)       24 2024-04-03 01:31:36.000000 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/requires.txt
+-rw-r--r--   0 sunminghui   (501) staff       (20)        7 2024-04-03 01:31:36.000000 xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/top_level.txt
```

### Comparing `xunfei-spark-python-0.0.7/PKG-INFO` & `xunfei-spark-python-0.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunfei-spark-python
-Version: 0.0.7
+Version: 0.1.0
 Summary: 科大讯飞星火大模型SDK
 Home-page: https://github.com/sunmh207/xunfei-spark-python
 Author: Stanley Sun
 Author-email: stanley.java@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,43 +16,44 @@
 Description-Content-Type: text/markdown
 Requires-Dist: websocket-client==1.7.0
 
 
 # 科大讯飞星火模型 Python SDK
 
 ## 介绍
-
-关于科大讯飞星火大模型，官网仅给出了[Web API文档](https://www.xfyun.cn/doc/spark/Web.html)，没有提供Python版SDK，使用起来不方便，尤其是在Stream交互的场景中。本项目封装了星火大模型的Web API，提供了类似OpenAI格式的SDK。
+科大讯飞星火大模型的Python版SDK，目前支持3.5版本的API。 详细参数说明可参考官网[WebAPI接口文档](https://www.xfyun.cn/doc/spark/Web.html)。
 
 ## 快速体验
 
 1. 下载本项目代码，并安装依赖
 ```
-pip install -r  requirements.txt
+git clone https://github.com/sunmh207/xunfei-spark-python.git
+cd xunfei-spark-python
+pip install -r requirements.txt
 ```
 
 2. 复制文件.env.dist 为.env，并将.env文件中的`{your_app_id}`, `{your_api_secret}`, `{your_api_key}`替换为自己的应用信息
 ```
 cp .env.dist .env
 ```
 
 3. 运行demo
 ```
 python demo.py
 ```
 ![demo](docs/imgs/demo.png)
 
-备注: 使用前请确保已经在科大讯飞官网注册账号，并且已经创建了应用，获取到了`app_id`, `api_secret`, `api_key`
+备注: 使用前请确保已经在科大讯飞官网注册账号、创建应用，且获得了`app_id`, `api_secret`, `api_key`，获取key的地址：[https://console.xfyun.cn/services/bm35](https://console.xfyun.cn/services/bm35)
 
 
 ## 项目中使用
 
 ### 1.安装
 ```
-pip install xunfei-spark-python==0.0.7
+pip install xunfei-spark-python==0.1.0
 ```
 
 ### 2.使用说明
 
 #### 问答接口
 
 ```python
@@ -76,26 +77,29 @@
 ```
 
 #### Stream模式问答接口
     
 ```python
 from xunfei.spark.client import Spark
 
-if __name__ == '__main__':
+def main():
     config = {
         "app_id": "{your_app_id}",
         "api_secret": "{your_api_secret}",
         "api_key": "{your_api_key}",
         "gpt_url": "wss://spark-api.xf-yun.com/v3.5/chat",
         "domain": "generalv3.5",
     }
     spark = Spark(**config)
     messages = [{"role": "user", "content": "你是谁开发的？"}]
 
     for message in spark.chat_stream(messages=messages, temperature=0.5, max_tokens=1024):
         if message:
-            if 'type' in message and message['type'] == 'chunk':
-                print(f"客户端接受到的消息: {message}")
-            elif 'type' in message and message['type'] == 'stop':
-                print(f"结束")
+            if message.get('type') == 'chunk':
+                print(f"客户端接受到的消息: {message['content']}")
+            elif message.get('type') == 'stop':
+                print("结束")
                 break
+
+if __name__ == '__main__':
+    main()
 ```
```

### Comparing `xunfei-spark-python-0.0.7/README.md` & `xunfei-spark-python-0.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 # 科大讯飞星火模型 Python SDK
 
 ## 介绍
-
-关于科大讯飞星火大模型，官网仅给出了[Web API文档](https://www.xfyun.cn/doc/spark/Web.html)，没有提供Python版SDK，使用起来不方便，尤其是在Stream交互的场景中。本项目封装了星火大模型的Web API，提供了类似OpenAI格式的SDK。
+科大讯飞星火大模型的Python版SDK，目前支持3.5版本的API。 详细参数说明可参考官网[WebAPI接口文档](https://www.xfyun.cn/doc/spark/Web.html)。
 
 ## 快速体验
 
 1. 下载本项目代码，并安装依赖
 ```
-pip install -r  requirements.txt
+git clone https://github.com/sunmh207/xunfei-spark-python.git
+cd xunfei-spark-python
+pip install -r requirements.txt
 ```
 
 2. 复制文件.env.dist 为.env，并将.env文件中的`{your_app_id}`, `{your_api_secret}`, `{your_api_key}`替换为自己的应用信息
 ```
 cp .env.dist .env
 ```
 
 3. 运行demo
 ```
 python demo.py
 ```
 ![demo](docs/imgs/demo.png)
 
-备注: 使用前请确保已经在科大讯飞官网注册账号，并且已经创建了应用，获取到了`app_id`, `api_secret`, `api_key`
+备注: 使用前请确保已经在科大讯飞官网注册账号、创建应用，且获得了`app_id`, `api_secret`, `api_key`，获取key的地址：[https://console.xfyun.cn/services/bm35](https://console.xfyun.cn/services/bm35)
 
 
 ## 项目中使用
 
 ### 1.安装
 ```
-pip install xunfei-spark-python==0.0.7
+pip install xunfei-spark-python==0.1.0
 ```
 
 ### 2.使用说明
 
 #### 问答接口
 
 ```python
@@ -57,26 +58,29 @@
 ```
 
 #### Stream模式问答接口
     
 ```python
 from xunfei.spark.client import Spark
 
-if __name__ == '__main__':
+def main():
     config = {
         "app_id": "{your_app_id}",
         "api_secret": "{your_api_secret}",
         "api_key": "{your_api_key}",
         "gpt_url": "wss://spark-api.xf-yun.com/v3.5/chat",
         "domain": "generalv3.5",
     }
     spark = Spark(**config)
     messages = [{"role": "user", "content": "你是谁开发的？"}]
 
     for message in spark.chat_stream(messages=messages, temperature=0.5, max_tokens=1024):
         if message:
-            if 'type' in message and message['type'] == 'chunk':
-                print(f"客户端接受到的消息: {message}")
-            elif 'type' in message and message['type'] == 'stop':
-                print(f"结束")
+            if message.get('type') == 'chunk':
+                print(f"客户端接受到的消息: {message['content']}")
+            elif message.get('type') == 'stop':
+                print("结束")
                 break
+
+if __name__ == '__main__':
+    main()
 ```
```

### Comparing `xunfei-spark-python-0.0.7/setup.py` & `xunfei-spark-python-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'xunfei-spark-python'
 DESCRIPTION = u'科大讯飞星火大模型SDK'
 URL = 'https://github.com/sunmh207/xunfei-spark-python'
 EMAIL = 'stanley.java@gmail.com'
 AUTHOR = 'Stanley Sun'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '0.0.7'
+VERSION = '0.1.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'websocket-client==1.7.0',
 ]
 
 # What packages are optional?
```

### Comparing `xunfei-spark-python-0.0.7/xunfei/spark/client.py` & `xunfei-spark-python-0.1.0/xunfei/spark/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
             self.wss_status = 'error'
 
         def on_close(*args):
             self.wss_status = 'closed'
 
         def on_open(ws):
             self.wss_status = 'open'
+            self.response_content = ''
             thread.start_new_thread(run, (ws,))
 
         websocket.enableTrace(False)
         ws_url = self.create_url()
 
         ws = websocket.WebSocketApp(ws_url, on_message=on_message, on_error=on_error, on_close=on_close,
                                     on_open=on_open)
```

### Comparing `xunfei-spark-python-0.0.7/xunfei_spark_python.egg-info/PKG-INFO` & `xunfei-spark-python-0.1.0/xunfei_spark_python.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xunfei-spark-python
-Version: 0.0.7
+Version: 0.1.0
 Summary: 科大讯飞星火大模型SDK
 Home-page: https://github.com/sunmh207/xunfei-spark-python
 Author: Stanley Sun
 Author-email: stanley.java@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,43 +16,44 @@
 Description-Content-Type: text/markdown
 Requires-Dist: websocket-client==1.7.0
 
 
 # 科大讯飞星火模型 Python SDK
 
 ## 介绍
-
-关于科大讯飞星火大模型，官网仅给出了[Web API文档](https://www.xfyun.cn/doc/spark/Web.html)，没有提供Python版SDK，使用起来不方便，尤其是在Stream交互的场景中。本项目封装了星火大模型的Web API，提供了类似OpenAI格式的SDK。
+科大讯飞星火大模型的Python版SDK，目前支持3.5版本的API。 详细参数说明可参考官网[WebAPI接口文档](https://www.xfyun.cn/doc/spark/Web.html)。
 
 ## 快速体验
 
 1. 下载本项目代码，并安装依赖
 ```
-pip install -r  requirements.txt
+git clone https://github.com/sunmh207/xunfei-spark-python.git
+cd xunfei-spark-python
+pip install -r requirements.txt
 ```
 
 2. 复制文件.env.dist 为.env，并将.env文件中的`{your_app_id}`, `{your_api_secret}`, `{your_api_key}`替换为自己的应用信息
 ```
 cp .env.dist .env
 ```
 
 3. 运行demo
 ```
 python demo.py
 ```
 ![demo](docs/imgs/demo.png)
 
-备注: 使用前请确保已经在科大讯飞官网注册账号，并且已经创建了应用，获取到了`app_id`, `api_secret`, `api_key`
+备注: 使用前请确保已经在科大讯飞官网注册账号、创建应用，且获得了`app_id`, `api_secret`, `api_key`，获取key的地址：[https://console.xfyun.cn/services/bm35](https://console.xfyun.cn/services/bm35)
 
 
 ## 项目中使用
 
 ### 1.安装
 ```
-pip install xunfei-spark-python==0.0.7
+pip install xunfei-spark-python==0.1.0
 ```
 
 ### 2.使用说明
 
 #### 问答接口
 
 ```python
@@ -76,26 +77,29 @@
 ```
 
 #### Stream模式问答接口
     
 ```python
 from xunfei.spark.client import Spark
 
-if __name__ == '__main__':
+def main():
     config = {
         "app_id": "{your_app_id}",
         "api_secret": "{your_api_secret}",
         "api_key": "{your_api_key}",
         "gpt_url": "wss://spark-api.xf-yun.com/v3.5/chat",
         "domain": "generalv3.5",
     }
     spark = Spark(**config)
     messages = [{"role": "user", "content": "你是谁开发的？"}]
 
     for message in spark.chat_stream(messages=messages, temperature=0.5, max_tokens=1024):
         if message:
-            if 'type' in message and message['type'] == 'chunk':
-                print(f"客户端接受到的消息: {message}")
-            elif 'type' in message and message['type'] == 'stop':
-                print(f"结束")
+            if message.get('type') == 'chunk':
+                print(f"客户端接受到的消息: {message['content']}")
+            elif message.get('type') == 'stop':
+                print("结束")
                 break
+
+if __name__ == '__main__':
+    main()
 ```
```

