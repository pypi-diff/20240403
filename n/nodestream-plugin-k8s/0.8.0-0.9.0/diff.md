# Comparing `tmp/nodestream_plugin_k8s-0.8.0.tar.gz` & `tmp/nodestream_plugin_k8s-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_k8s-0.8.0.tar", max compression
+gzip compressed data, was "nodestream_plugin_k8s-0.9.0.tar", max compression
```

## Comparing `nodestream_plugin_k8s-0.8.0.tar` & `nodestream_plugin_k8s-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-10-20 14:56:59.621165 nodestream_plugin_k8s-0.8.0/LICENSE
--rw-r--r--   0        0        0     2773 2023-10-20 15:01:45.821889 nodestream_plugin_k8s-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-10-19 19:59:38.857400 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/__init__.py
--rw-r--r--   0        0        0      195 2023-10-20 15:17:58.674576 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/commands/__init__.py
--rw-r--r--   0        0        0      419 2023-10-20 14:54:58.883527 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/commands/destroy_command.py
--rw-r--r--   0        0        0     1560 2023-10-20 15:18:11.852563 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/commands/list_command.py
--rw-r--r--   0        0        0      473 2023-10-20 14:55:07.070380 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/commands/sync_command.py
--rw-r--r--   0        0        0        0 2023-10-19 20:12:33.403496 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/operations/__init__.py
--rw-r--r--   0        0        0     2045 2023-10-20 15:18:11.830545 nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/project_resource_manager.py
--rw-r--r--   0        0        0      660 2023-10-20 15:17:31.832469 nodestream_plugin_k8s-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3289 1970-01-01 00:00:00.000000 nodestream_plugin_k8s-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-10-20 14:56:59.621165 nodestream_plugin_k8s-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2773 2023-10-20 15:01:45.821889 nodestream_plugin_k8s-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-10-19 19:59:38.857400 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/__init__.py
+-rw-r--r--   0        0        0      195 2023-10-20 15:17:58.674576 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/commands/__init__.py
+-rw-r--r--   0        0        0      419 2023-10-20 14:54:58.883527 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/commands/destroy_command.py
+-rw-r--r--   0        0        0     1560 2023-10-20 15:18:11.852563 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/commands/list_command.py
+-rw-r--r--   0        0        0      473 2023-10-20 14:55:07.070380 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/commands/sync_command.py
+-rw-r--r--   0        0        0        0 2023-10-19 20:12:33.403496 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/operations/__init__.py
+-rw-r--r--   0        0        0     2045 2023-11-02 16:37:12.756621 nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/project_resource_manager.py
+-rw-r--r--   0        0        0      660 2023-11-20 19:56:34.468294 nodestream_plugin_k8s-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 nodestream_plugin_k8s-0.9.0/PKG-INFO
```

### Comparing `nodestream_plugin_k8s-0.8.0/LICENSE` & `nodestream_plugin_k8s-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_k8s-0.8.0/README.md` & `nodestream_plugin_k8s-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/commands/list_command.py` & `nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_k8s-0.8.0/nodestream_plugin_k8s/project_resource_manager.py` & `nodestream_plugin_k8s-0.9.0/nodestream_plugin_k8s/project_resource_manager.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_k8s-0.8.0/pyproject.toml` & `nodestream_plugin_k8s-0.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "nodestream-plugin-k8s"
-version = "0.8.0"
+version = "0.9.0"
 description = "A plugin for nodestream that manages k8s resources."
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 readme = "README.md"
 license = "Apache 2.0"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nodestream = "^0.8.2"
+nodestream = "^0.9.0"
 
 [tool.poetry.plugins."nodestream.plugins"]
 commands = "nodestream_plugin_k8s.commands"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
```

### Comparing `nodestream_plugin_k8s-0.8.0/PKG-INFO` & `nodestream_plugin_k8s-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-k8s
-Version: 0.8.0
+Version: 0.9.0
 Summary: A plugin for nodestream that manages k8s resources.
 License: Apache 2.0
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: nodestream (>=0.8.2,<0.9.0)
+Requires-Dist: nodestream (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # Nodestream Kubernetes Plugin 
 
 NOTE: This plugin is still in development and is not ready for production use.
 
 ## Overview
```

