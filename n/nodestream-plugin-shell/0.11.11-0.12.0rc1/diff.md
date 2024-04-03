# Comparing `tmp/nodestream_plugin_shell-0.11.11.tar.gz` & `tmp/nodestream_plugin_shell-0.12.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_shell-0.11.11.tar", max compression
+gzip compressed data, was "nodestream_plugin_shell-0.12.0rc1.tar", max compression
```

## Comparing `nodestream_plugin_shell-0.11.11.tar` & `nodestream_plugin_shell-0.12.0rc1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-03-14 16:31:08.563385 nodestream_plugin_shell-0.11.11/LICENSE
--rw-r--r--   0        0        0     1478 2024-03-15 15:00:25.678543 nodestream_plugin_shell-0.11.11/README.md
--rw-r--r--   0        0        0       47 2024-03-15 15:00:25.679489 nodestream_plugin_shell-0.11.11/nodestream_plugin_shell/__init__.py
--rw-r--r--   0        0        0     2858 2024-03-15 15:00:25.680320 nodestream_plugin_shell-0.11.11/nodestream_plugin_shell/shell.py
--rw-r--r--   0        0        0      696 2024-03-15 15:01:44.553833 nodestream_plugin_shell-0.11.11/pyproject.toml
--rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 nodestream_plugin_shell-0.11.11/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 14:32:39.712113 nodestream_plugin_shell-0.12.0rc1/LICENSE
+-rw-r--r--   0        0        0     1478 2024-04-03 14:32:39.712463 nodestream_plugin_shell-0.12.0rc1/README.md
+-rw-r--r--   0        0        0       47 2024-04-03 14:32:39.712685 nodestream_plugin_shell-0.12.0rc1/nodestream_plugin_shell/__init__.py
+-rw-r--r--   0        0        0     2858 2024-04-03 14:32:39.712823 nodestream_plugin_shell-0.12.0rc1/nodestream_plugin_shell/shell.py
+-rw-r--r--   0        0        0      701 2024-04-03 14:35:02.660226 nodestream_plugin_shell-0.12.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 nodestream_plugin_shell-0.12.0rc1/PKG-INFO
```

### Comparing `nodestream_plugin_shell-0.11.11/LICENSE` & `nodestream_plugin_shell-0.12.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_shell-0.11.11/README.md` & `nodestream_plugin_shell-0.12.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_shell-0.11.11/nodestream_plugin_shell/shell.py` & `nodestream_plugin_shell-0.12.0rc1/nodestream_plugin_shell/shell.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_shell-0.11.11/pyproject.toml` & `nodestream_plugin_shell-0.12.0rc1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nodestream-plugin-shell"
-version = "0.11.11"
+version = "0.12.0rc1"
 description = "A plugin for nodestream providing pipeline shell execution."
 authors = ["Grant Hoffman <Grant_Hoffman@intuit.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nodestream = "^0.11.0"
+nodestream = "^0.12.0rc2"
 
 [tool.poetry.plugins."nodestream.plugins"]
 pipeline = "nodestream_plugin_shell"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
```

### Comparing `nodestream_plugin_shell-0.11.11/PKG-INFO` & `nodestream_plugin_shell-0.12.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-shell
-Version: 0.11.11
+Version: 0.12.0rc1
 Summary: A plugin for nodestream providing pipeline shell execution.
 License: Apache 2.0
 Author: Grant Hoffman
 Author-email: Grant_Hoffman@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nodestream (>=0.11.0,<0.12.0)
+Requires-Dist: nodestream (>=0.12.0rc2,<0.13.0)
 Description-Content-Type: text/markdown
 
 # Nodestream Shell Plugin
 
 This plugin provides a [Nodestream](https://github.com/nodestream-proj/nodestream) shell extractor. 
 
 **NOTE: This plugin is currently in development and is not yet ready for production use.**
```

