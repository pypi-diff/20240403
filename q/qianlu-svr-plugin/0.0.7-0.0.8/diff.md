# Comparing `tmp/qianlu-svr-plugin-0.0.7.tar.gz` & `tmp/qianlu-svr-plugin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianlu-svr-plugin-0.0.7.tar", last modified: Wed Apr  3 08:49:41 2024, max compression
+gzip compressed data, was "qianlu-svr-plugin-0.0.8.tar", last modified: Wed Apr  3 09:20:23 2024, max compression
```

## Comparing `qianlu-svr-plugin-0.0.7.tar` & `qianlu-svr-plugin-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.757513 qianlu-svr-plugin-0.0.7/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:49:41.756515 qianlu-svr-plugin-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.745544 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/
--rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/__init__.py
--rw-rw-rw-   0        0        0     3587 2024-04-03 08:49:30.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/server.py
--rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.755518 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:49:41.757513 qianlu-svr-plugin-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-03 08:49:38.000000 qianlu-svr-plugin-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.986189 qianlu-svr-plugin-0.0.8/
+-rw-rw-rw-   0        0        0      394 2024-04-03 09:20:23.984193 qianlu-svr-plugin-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.968236 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/
+-rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/__init__.py
+-rw-rw-rw-   0        0        0     4521 2024-04-03 09:16:57.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/server.py
+-rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.983197 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:20:23.986189 qianlu-svr-plugin-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-03 09:20:21.000000 qianlu-svr-plugin-0.0.8/setup.py
```

### Comparing `qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/server.py` & `qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,57 +10,80 @@
         super(QianluService, self).__init__()
         self.ws = None
         self.isRun = True
         self.parser = argparse.ArgumentParser(description="cv")
         self.parser.add_argument('-m', '--model', type=str, default='default', help='模型路径')
         self.parser.add_argument('-i', '--id', type=str, default='local_cv', help='id')
         self.services = {}
+        self.onMessageFunction = []
 
     def register(self, key, service, force=False):
         if key not in self.services or force:
             self.services[key] = service
         else:
             print("service has register")
 
     def unregister(self, key):
         if key in self.services.keys():
             del self.services[key]
 
+    def onMessage(self, func):
+        self.onMessageFunction.append(func)
+
+    def clearMessage(self):
+        self.onMessageFunction = []
+
     def on_message(self, client, message):
         msg = json.loads(message)
         dataObj = {}
         try:
             dataObj = json.loads(msg["data"])
         except ValueError as e:
             pass
+
+        print("on_message：%s" % msg)
         to = msg['to']
         msg['to'] = msg['from']
         msg['from'] = to
         if len(dataObj) > 0:
+            if "serviceID" in dataObj and 'functionName' in dataObj and dataObj['serviceID'] == "onMessage" and dataObj['functionName'] == "onMessage":
+                try:
+                    for func in self.onMessageFunction:
+                        result = func(dataObj['args'])
+                        msg['data'] = json.dumps(result)
+                        client.send(json.dumps(msg))
+                        return
+                except ValueError as e:
+                    msg['data'] = json.dumps({"code": -3005, "msg": "执行功能异常", "data": ""})
+                    client.send(json.dumps(msg))
+                    return
             if "serviceID" in dataObj and dataObj['serviceID'] in self.services:
                 try:
                     method = getattr(self.services[dataObj["serviceID"]], dataObj["functionName"])
                     init = getattr(self.services[dataObj["serviceID"]], "init")
                     if init is not None and "config" in dataObj:
                         init(dataObj['config'])
 
                     if method is not None:
                         result = method(dataObj['args'])
                         msg['data'] = json.dumps(result)
                         client.send(json.dumps(msg))
+                        return
                     else:
                         msg['data'] = json.dumps({"code": -3002, "msg": "功能未发现", "data": ""})
                         client.send(json.dumps(msg))
+                        return
                 except ValueError as e:
                     msg['data'] = json.dumps({"code": -3003, "msg": "执行异常", "data": ""})
                     client.send(json.dumps(msg))
+                    return
             else:
                 msg['data'] = json.dumps({"code": -3001, "msg": "服务未发现", "data": ""})
                 client.send(json.dumps(msg))
-        print("on_message：%s" % msg)
+                return
 
     def on_error(self, ws, error):
         print("####### on_error #######")
         print("error：%s" % error)
 
     def on_close(self, ws, close_status_code, close_msg):
         print("####### on_close #######")
```

### Comparing `qianlu-svr-plugin-0.0.7/setup.py` & `qianlu-svr-plugin-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qianlu-svr-plugin",                     # This is the name of the package
-    version="0.0.7",                        # The initial release version
+    version="0.0.8",                        # The initial release version
     author="bxwx123",                     # Full name of the author
     description="this is service base plugin by websocket",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

