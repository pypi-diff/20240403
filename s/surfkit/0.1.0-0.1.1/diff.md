# Comparing `tmp/surfkit-0.1.0.tar.gz` & `tmp/surfkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.0.tar", max compression
+gzip compressed data, was "surfkit-0.1.1.tar", max compression
```

## Comparing `surfkit-0.1.0.tar` & `surfkit-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.0/LICENSE
--rw-r--r--   0        0        0      158 2024-04-02 20:50:12.966277 surfkit-0.1.0/README.md
--rw-r--r--   0        0        0      442 2024-04-02 20:44:52.171622 surfkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      610 2024-04-02 20:50:51.383715 surfkit-0.1.0/surfkit/agent.py
--rw-r--r--   0        0        0        0 2024-04-02 20:19:29.385009 surfkit-0.1.0/surfkit/cli.py
--rw-r--r--   0        0        0      195 2024-04-02 20:23:26.016439 surfkit-0.1.0/surfkit/env.py
--rw-r--r--   0        0        0     5444 2024-04-02 20:43:49.583063 surfkit-0.1.0/surfkit/llm.py
--rw-r--r--   0        0        0      672 2024-04-02 20:45:45.180939 surfkit-0.1.0/surfkit/models.py
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 surfkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.1/README.md
+-rw-r--r--   0        0        0      442 2024-04-03 02:49:25.687997 surfkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-02 20:50:51.383715 surfkit-0.1.1/surfkit/agent.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:19:29.385009 surfkit-0.1.1/surfkit/cli.py
+-rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.1/surfkit/db/conn.py
+-rw-r--r--   0        0        0     5176 2024-04-03 02:09:57.525061 surfkit-0.1.1/surfkit/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:23:26.016439 surfkit-0.1.1/surfkit/env.py
+-rw-r--r--   0        0        0     5444 2024-04-02 20:43:49.583063 surfkit-0.1.1/surfkit/llm.py
+-rw-r--r--   0        0        0     1656 2024-04-03 02:10:36.829145 surfkit-0.1.1/surfkit/models.py
+-rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.1/surfkit/types.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.1/PKG-INFO
```

### Comparing `surfkit-0.1.0/LICENSE` & `surfkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.0/surfkit/agent.py` & `surfkit-0.1.1/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.0/surfkit/llm.py` & `surfkit-0.1.1/surfkit/llm.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.0/PKG-INFO` & `surfkit-0.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolkit to build GUI surfing AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -27,11 +27,23 @@
 pip install surfkit
 ```
 
 ## Usage
 
 Create a new agent
 
-```
+```sh
 surfkit init [NAME]
 ```
 
+Run the agent
+
+```sh
+surfkit run . --provider kubernetes
+```
+
+Publish the agent
+
+```sh
+surfkit publish .
+```
+
```

