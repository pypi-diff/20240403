# Comparing `tmp/qianlu-svr-plugin-0.0.5.tar.gz` & `tmp/qianlu-svr-plugin-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianlu-svr-plugin-0.0.5.tar", last modified: Wed Apr  3 08:27:20 2024, max compression
+gzip compressed data, was "qianlu-svr-plugin-0.0.6.tar", last modified: Wed Apr  3 08:45:35 2024, max compression
```

## Comparing `qianlu-svr-plugin-0.0.5.tar` & `qianlu-svr-plugin-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.689736 qianlu-svr-plugin-0.0.5/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:27:20.688738 qianlu-svr-plugin-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.673778 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/
--rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/__init__.py
--rw-rw-rw-   0        0        0     3274 2024-04-03 06:59:16.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/server.py
--rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.687769 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:27:20.689736 qianlu-svr-plugin-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-03 08:27:18.000000 qianlu-svr-plugin-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.484340 qianlu-svr-plugin-0.0.6/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:45:35.482835 qianlu-svr-plugin-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.462725 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/
+-rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/__init__.py
+-rw-rw-rw-   0        0        0     3468 2024-04-03 08:45:32.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/server.py
+-rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.481675 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:45:35.484340 qianlu-svr-plugin-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-03 08:45:32.000000 qianlu-svr-plugin-0.0.6/setup.py
```

### Comparing `qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/server.py` & `qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/server.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,18 @@
         to = msg['to']
         msg['to'] = msg['from']
         msg['from'] = to
         if len(dataObj) > 0:
             if "serviceID" in dataObj and dataObj['serviceID'] in self.services:
                 try:
                     method = getattr(self.services[dataObj["serviceID"]], dataObj["functionName"])
+                    init = getattr(self.services[dataObj["serviceID"]], "init")
+                    if init is not None and "config" in dataObj:
+                        init(dataObj['config'])
+
                     if method is not None:
                         result = method(dataObj['args'])
                         msg['data'] = json.dumps(result)
                         client.send(json.dumps(msg))
                     else:
                         msg['data'] = json.dumps({"code": -3002, "msg": "功能未发现", "data": ""})
                         client.send(json.dumps(msg))
```

### Comparing `qianlu-svr-plugin-0.0.5/setup.py` & `qianlu-svr-plugin-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qianlu-svr-plugin",                     # This is the name of the package
-    version="0.0.5",                        # The initial release version
+    version="0.0.6",                        # The initial release version
     author="bxwx123",                     # Full name of the author
     description="this is service base plugin by websocket",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

