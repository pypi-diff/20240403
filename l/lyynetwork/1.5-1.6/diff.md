# Comparing `tmp/lyynetwork-1.5.tar.gz` & `tmp/lyynetwork-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyynetwork-1.5.tar", last modified: Wed Apr  3 15:09:21 2024, max compression
+gzip compressed data, was "lyynetwork-1.6.tar", last modified: Wed Apr  3 15:10:52 2024, max compression
```

## Comparing `lyynetwork-1.5.tar` & `lyynetwork-1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 15:09:21.719505 lyynetwork-1.5/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynetwork-1.5/LICENSE
--rw-rw-rw-   0        0        0      160 2024-04-03 15:09:21.718505 lyynetwork-1.5/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynetwork-1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 15:09:21.717505 lyynetwork-1.5/lyynetwork.egg-info/
--rw-rw-rw-   0        0        0      160 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 15:09:21.000000 lyynetwork-1.5/lyynetwork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7275 2024-04-03 15:09:05.000000 lyynetwork-1.5/lyynetwork.py
--rw-rw-rw-   0        0        0       42 2024-04-03 15:09:21.719505 lyynetwork-1.5/setup.cfg
--rw-rw-rw-   0        0        0      265 2024-04-03 15:09:16.000000 lyynetwork-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:10:52.649429 lyynetwork-1.6/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyynetwork-1.6/LICENSE
+-rw-rw-rw-   0        0        0      160 2024-04-03 15:10:52.648429 lyynetwork-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyynetwork-1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 15:10:52.647429 lyynetwork-1.6/lyynetwork.egg-info/
+-rw-rw-rw-   0        0        0      160 2024-04-03 15:10:52.000000 lyynetwork-1.6/lyynetwork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-04-03 15:10:52.000000 lyynetwork-1.6/lyynetwork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:10:52.000000 lyynetwork-1.6/lyynetwork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 15:10:52.000000 lyynetwork-1.6/lyynetwork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7976 2024-04-03 15:10:38.000000 lyynetwork-1.6/lyynetwork.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 15:10:52.649429 lyynetwork-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      265 2024-04-03 15:10:51.000000 lyynetwork-1.6/setup.py
```

### Comparing `lyynetwork-1.5/LICENSE` & `lyynetwork-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lyynetwork-1.5/lyynetwork.py` & `lyynetwork-1.6/lyynetwork.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 import socket
 import json
 import time
 import threading
+import requests
+
+def ocr_panddle_jd_server(img_link, ocr_red_text=False, debug=False):
+    # 目标URL
+    url = "http://117.72.45.252:10028/ocr"
+
+    # 要发送的数据
+    post_data = {"img_url": img_link}
+
+    # 发送POST请求
+    response = requests.post(url, json=post_data)
+
+    # 检查响应是否成功
+    if response.status_code == 200:
+        if debug:
+            print(response.text)
+        # 解析JSON响应
+        result = response.json()
+        if debug:
+            print(result)
+        return result.get("ocr_text")
+    else:
+        # 如果响应不成功，打印错误信息
+        print(f"Error: {response.status_code}")
+        return None
 
 
 def is_port_open(host, port):
     # 创建一个socket对象
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     sock.settimeout(1)  # 设置超时时间
     try:
```

