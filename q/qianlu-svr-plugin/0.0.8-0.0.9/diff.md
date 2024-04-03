# Comparing `tmp/qianlu-svr-plugin-0.0.8.tar.gz` & `tmp/qianlu-svr-plugin-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianlu-svr-plugin-0.0.8.tar", last modified: Wed Apr  3 09:20:23 2024, max compression
+gzip compressed data, was "qianlu-svr-plugin-0.0.9.tar", last modified: Wed Apr  3 09:27:58 2024, max compression
```

## Comparing `qianlu-svr-plugin-0.0.8.tar` & `qianlu-svr-plugin-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.986189 qianlu-svr-plugin-0.0.8/
--rw-rw-rw-   0        0        0      394 2024-04-03 09:20:23.984193 qianlu-svr-plugin-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.968236 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/
--rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/__init__.py
--rw-rw-rw-   0        0        0     4521 2024-04-03 09:16:57.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/server.py
--rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 09:20:23.983197 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 09:20:23.000000 qianlu-svr-plugin-0.0.8/qianlu_svr_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 09:20:23.986189 qianlu-svr-plugin-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-03 09:20:21.000000 qianlu-svr-plugin-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:27:58.755442 qianlu-svr-plugin-0.0.9/
+-rw-rw-rw-   0        0        0      391 2024-04-03 09:27:58.753448 qianlu-svr-plugin-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       41 2024-04-03 09:24:10.000000 qianlu-svr-plugin-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 09:27:58.742478 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin/
+-rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin/__init__.py
+-rw-rw-rw-   0        0        0     4521 2024-04-03 09:16:57.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin/server.py
+-rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 09:27:58.752450 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin.egg-info/
+-rw-rw-rw-   0        0        0      391 2024-04-03 09:27:58.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 09:27:58.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 09:27:58.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 09:27:58.000000 qianlu-svr-plugin-0.0.9/qianlu_svr_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 09:27:58.755442 qianlu-svr-plugin-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-03 09:27:55.000000 qianlu-svr-plugin-0.0.9/setup.py
```

### Comparing `qianlu-svr-plugin-0.0.8/qianlu_svr_plugin/server.py` & `qianlu-svr-plugin-0.0.9/qianlu_svr_plugin/server.py`

 * *Files identical despite different names*

### Comparing `qianlu-svr-plugin-0.0.8/setup.py` & `qianlu-svr-plugin-0.0.9/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qianlu-svr-plugin",                     # This is the name of the package
-    version="0.0.8",                        # The initial release version
+    version="0.0.9",                        # The initial release version
     author="bxwx123",                     # Full name of the author
     description="this is service base plugin by websocket",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

