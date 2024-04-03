# Comparing `tmp/qianlu-svr-plugin-0.0.6.tar.gz` & `tmp/qianlu-svr-plugin-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianlu-svr-plugin-0.0.6.tar", last modified: Wed Apr  3 08:45:35 2024, max compression
+gzip compressed data, was "qianlu-svr-plugin-0.0.7.tar", last modified: Wed Apr  3 08:49:41 2024, max compression
```

## Comparing `qianlu-svr-plugin-0.0.6.tar` & `qianlu-svr-plugin-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.484340 qianlu-svr-plugin-0.0.6/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:45:35.482835 qianlu-svr-plugin-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.462725 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/
--rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/__init__.py
--rw-rw-rw-   0        0        0     3468 2024-04-03 08:45:32.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/server.py
--rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:45:35.481675 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 08:45:35.000000 qianlu-svr-plugin-0.0.6/qianlu_svr_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:45:35.484340 qianlu-svr-plugin-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-03 08:45:32.000000 qianlu-svr-plugin-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.757513 qianlu-svr-plugin-0.0.7/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:49:41.756515 qianlu-svr-plugin-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.745544 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/
+-rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/__init__.py
+-rw-rw-rw-   0        0        0     3587 2024-04-03 08:49:30.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/server.py
+-rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:49:41.755518 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 08:49:41.000000 qianlu-svr-plugin-0.0.7/qianlu_svr_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:49:41.757513 qianlu-svr-plugin-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-03 08:49:38.000000 qianlu-svr-plugin-0.0.7/setup.py
```

### Comparing `qianlu-svr-plugin-0.0.6/qianlu_svr_plugin/server.py` & `qianlu-svr-plugin-0.0.7/qianlu_svr_plugin/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,16 +11,19 @@
         self.ws = None
         self.isRun = True
         self.parser = argparse.ArgumentParser(description="cv")
         self.parser.add_argument('-m', '--model', type=str, default='default', help='模型路径')
         self.parser.add_argument('-i', '--id', type=str, default='local_cv', help='id')
         self.services = {}
 
-    def register(self, key, service):
-        self.services[key] = service
+    def register(self, key, service, force=False):
+        if key not in self.services or force:
+            self.services[key] = service
+        else:
+            print("service has register")
 
     def unregister(self, key):
         if key in self.services.keys():
             del self.services[key]
 
     def on_message(self, client, message):
         msg = json.loads(message)
```

### Comparing `qianlu-svr-plugin-0.0.6/setup.py` & `qianlu-svr-plugin-0.0.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qianlu-svr-plugin",                     # This is the name of the package
-    version="0.0.6",                        # The initial release version
+    version="0.0.7",                        # The initial release version
     author="bxwx123",                     # Full name of the author
     description="this is service base plugin by websocket",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

