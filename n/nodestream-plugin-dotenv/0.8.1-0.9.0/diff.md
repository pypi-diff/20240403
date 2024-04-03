# Comparing `tmp/nodestream_plugin_dotenv-0.8.1.tar.gz` & `tmp/nodestream_plugin_dotenv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_dotenv-0.8.1.tar", max compression
+gzip compressed data, was "nodestream_plugin_dotenv-0.9.0.tar", max compression
```

## Comparing `nodestream_plugin_dotenv-0.8.1.tar` & `nodestream_plugin_dotenv-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    32335 2023-08-10 14:01:45.975334 nodestream_plugin_dotenv-0.8.1/LICENSE
--rw-r--r--   0        0        0      539 2023-08-10 14:03:43.182070 nodestream_plugin_dotenv-0.8.1/README.md
--rw-r--r--   0        0        0        0 2023-08-09 18:16:36.281514 nodestream_plugin_dotenv-0.8.1/nodestream_plugin_dotenv/__init__.py
--rw-r--r--   0        0        0      246 2023-08-10 14:33:59.986507 nodestream_plugin_dotenv-0.8.1/nodestream_plugin_dotenv/plugin.py
--rw-r--r--   0        0        0     1337 2023-10-19 16:20:08.869850 nodestream_plugin_dotenv-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1767 1970-01-01 00:00:00.000000 nodestream_plugin_dotenv-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-10-20 15:15:43.367542 nodestream_plugin_dotenv-0.9.0/LICENSE
+-rw-r--r--   0        0        0      539 2023-08-10 14:03:43.182070 nodestream_plugin_dotenv-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-09 18:16:36.281514 nodestream_plugin_dotenv-0.9.0/nodestream_plugin_dotenv/__init__.py
+-rw-r--r--   0        0        0      246 2023-08-10 14:33:59.986507 nodestream_plugin_dotenv-0.9.0/nodestream_plugin_dotenv/plugin.py
+-rw-r--r--   0        0        0     1264 2023-11-20 19:57:00.368312 nodestream_plugin_dotenv-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 nodestream_plugin_dotenv-0.9.0/PKG-INFO
```

### Comparing `nodestream_plugin_dotenv-0.8.1/README.md` & `nodestream_plugin_dotenv-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_dotenv-0.8.1/pyproject.toml` & `nodestream_plugin_dotenv-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "nodestream-plugin-dotenv"
-version = "0.8.1"
+version = "0.9.0"
 description = "A plugin to nodestream for loading environment variables from a .env file"
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 packages = [{include = "nodestream_plugin_dotenv"}]
-license = "GPL-3.0-only"
+license = "Apache 2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nodestream-proj/nodestream"
 repository = "https://github.com/nodestream-proj/nodestream-plugin-dotenv"
 documentation = "https://nodestream-proj.github.io/nodestream-plugin-dotenv"
 
 keywords = ["etl", "neo4j", "declarative", "data", "kafka", "ingest", "nodestream"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
     "Natural Language :: English",
     "Topic :: Database"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nodestream = "^0.8.0"
+nodestream = "^0.9.0"
 python-dotenv = ">=0.21.0,< 2"
 
 [tool.poetry.plugins."nodestream.plugins"]
 projects = "nodestream_plugin_dotenv.plugin"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `nodestream_plugin_dotenv-0.8.1/PKG-INFO` & `nodestream_plugin_dotenv-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-dotenv
-Version: 0.8.1
+Version: 0.9.0
 Summary: A plugin to nodestream for loading environment variables from a .env file
 Home-page: https://github.com/nodestream-proj/nodestream
-License: GPL-3.0-only
+License: Apache 2.0
 Keywords: etl,neo4j,declarative,data,kafka,ingest,nodestream
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
-Requires-Dist: nodestream (>=0.8.0,<0.9.0)
+Requires-Dist: nodestream (>=0.9.0,<0.10.0)
 Requires-Dist: python-dotenv (>=0.21.0,<2)
 Project-URL: Documentation, https://nodestream-proj.github.io/nodestream-plugin-dotenv
 Project-URL: Repository, https://github.com/nodestream-proj/nodestream-plugin-dotenv
 Description-Content-Type: text/markdown
 
 # Nodestream Dotenv Plugin
```

