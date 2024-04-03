# Comparing `tmp/qianlu-svr-plugin-0.0.4.tar.gz` & `tmp/qianlu-svr-plugin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qianlu-svr-plugin-0.0.4.tar", last modified: Wed Apr  3 08:24:01 2024, max compression
+gzip compressed data, was "qianlu-svr-plugin-0.0.5.tar", last modified: Wed Apr  3 08:27:20 2024, max compression
```

## Comparing `qianlu-svr-plugin-0.0.4.tar` & `qianlu-svr-plugin-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:24:01.461503 qianlu-svr-plugin-0.0.4/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:24:01.459509 qianlu-svr-plugin-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:24:01.439562 qianlu-svr-plugin-0.0.4/qianlu-svr-plugin/
--rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.4/qianlu-svr-plugin/__init__.py
--rw-rw-rw-   0        0        0     3274 2024-04-03 06:59:16.000000 qianlu-svr-plugin-0.0.4/qianlu-svr-plugin/server.py
--rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.4/qianlu-svr-plugin/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:24:01.457514 qianlu-svr-plugin-0.0.4/qianlu_svr_plugin.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-03 08:24:01.000000 qianlu-svr-plugin-0.0.4/qianlu_svr_plugin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-04-03 08:24:01.000000 qianlu-svr-plugin-0.0.4/qianlu_svr_plugin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:24:01.000000 qianlu-svr-plugin-0.0.4/qianlu_svr_plugin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-04-03 08:24:01.000000 qianlu-svr-plugin-0.0.4/qianlu_svr_plugin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 08:24:01.461503 qianlu-svr-plugin-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1138 2024-04-03 08:23:58.000000 qianlu-svr-plugin-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.689736 qianlu-svr-plugin-0.0.5/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:27:20.688738 qianlu-svr-plugin-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-04-03 07:07:23.000000 qianlu-svr-plugin-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.673778 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/
+-rw-rw-rw-   0        0        0       33 2024-04-03 07:55:08.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/__init__.py
+-rw-rw-rw-   0        0        0     3274 2024-04-03 06:59:16.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/server.py
+-rw-rw-rw-   0        0        0      454 2024-04-03 06:48:41.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:27:20.687769 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-03 08:27:20.000000 qianlu-svr-plugin-0.0.5/qianlu_svr_plugin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:27:20.689736 qianlu-svr-plugin-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1138 2024-04-03 08:27:18.000000 qianlu-svr-plugin-0.0.5/setup.py
```

### Comparing `qianlu-svr-plugin-0.0.4/qianlu-svr-plugin/server.py` & `qianlu-svr-plugin-0.0.5/qianlu_svr_plugin/server.py`

 * *Files identical despite different names*

### Comparing `qianlu-svr-plugin-0.0.4/setup.py` & `qianlu-svr-plugin-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qianlu-svr-plugin",                     # This is the name of the package
-    version="0.0.4",                        # The initial release version
+    version="0.0.5",                        # The initial release version
     author="bxwx123",                     # Full name of the author
     description="this is service base plugin by websocket",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

