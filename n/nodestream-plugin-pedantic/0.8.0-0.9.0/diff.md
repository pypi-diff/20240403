# Comparing `tmp/nodestream_plugin_pedantic-0.8.0.tar.gz` & `tmp/nodestream_plugin_pedantic-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_pedantic-0.8.0.tar", max compression
+gzip compressed data, was "nodestream_plugin_pedantic-0.9.0.tar", max compression
```

## Comparing `nodestream_plugin_pedantic-0.8.0.tar` & `nodestream_plugin_pedantic-0.9.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-10-20 14:31:16.448237 nodestream_plugin_pedantic-0.8.0/LICENSE
--rw-r--r--   0        0        0      884 2023-10-20 14:48:12.846829 nodestream_plugin_pedantic-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-08-10 14:41:59.246641 nodestream_plugin_pedantic-0.8.0/nodestream_plugin_pedantic/__init__.py
--rw-r--r--   0        0        0     4631 2023-10-20 14:48:02.469632 nodestream_plugin_pedantic-0.8.0/nodestream_plugin_pedantic/audits.py
--rw-r--r--   0        0        0     1363 2023-10-20 14:31:43.294907 nodestream_plugin_pedantic-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 nodestream_plugin_pedantic-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-10-20 14:31:16.448237 nodestream_plugin_pedantic-0.9.0/LICENSE
+-rw-r--r--   0        0        0      884 2023-10-20 14:48:12.846829 nodestream_plugin_pedantic-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-08-10 14:41:59.246641 nodestream_plugin_pedantic-0.9.0/nodestream_plugin_pedantic/__init__.py
+-rw-r--r--   0        0        0     4631 2023-10-20 14:48:02.469632 nodestream_plugin_pedantic-0.9.0/nodestream_plugin_pedantic/audits.py
+-rw-r--r--   0        0        0     1363 2023-11-20 19:57:34.403713 nodestream_plugin_pedantic-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2065 1970-01-01 00:00:00.000000 nodestream_plugin_pedantic-0.9.0/PKG-INFO
```

### Comparing `nodestream_plugin_pedantic-0.8.0/LICENSE` & `nodestream_plugin_pedantic-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_pedantic-0.8.0/README.md` & `nodestream_plugin_pedantic-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_pedantic-0.8.0/nodestream_plugin_pedantic/audits.py` & `nodestream_plugin_pedantic-0.9.0/nodestream_plugin_pedantic/audits.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_pedantic-0.8.0/pyproject.toml` & `nodestream_plugin_pedantic-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nodestream-plugin-pedantic"
-version = "0.8.0"
+version = "0.9.0"
 description = "A nodestream plugin that provides a series of audits to ensure high quality and consistent nodestream projects."
 authors = ["Zach Probst <Zach_Probst@intuit.com>"]
 packages = [{include = "nodestream_plugin_pedantic"}]
 license = "Apache-2.0"
 
 readme = "README.md"
 homepage = "https://github.com/nodestream-proj/nodestream"
@@ -19,15 +19,15 @@
     "Intended Audience :: Information Technology",
     "Natural Language :: English",
     "Topic :: Database"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-nodestream = "^0.8.0"
+nodestream = "^0.9.0"
 inflection = "^0.5.1"
 
 [tool.poetry.plugins."nodestream.plugins"]
 audits = "nodestream_plugin_pedantic.audits"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
```

### Comparing `nodestream_plugin_pedantic-0.8.0/PKG-INFO` & `nodestream_plugin_pedantic-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-pedantic
-Version: 0.8.0
+Version: 0.9.0
 Summary: A nodestream plugin that provides a series of audits to ensure high quality and consistent nodestream projects.
 Home-page: https://github.com/nodestream-proj/nodestream
 License: Apache-2.0
 Keywords: etl,neo4j,declarative,data,kafka,ingest,nodestream
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
 Requires-Python: >=3.10,<4.0
@@ -15,15 +15,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
-Requires-Dist: nodestream (>=0.8.0,<0.9.0)
+Requires-Dist: nodestream (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://nodestream-proj.github.io/nodestream-plugin-pedantic
 Project-URL: Repository, https://github.com/nodestream-proj/nodestream-plugin-pedantic
 Description-Content-Type: text/markdown
 
 # Nodestream pedantic Plugin
 
 This plugin adds a pedantic mode to nodestream. It will check for the following:
```

