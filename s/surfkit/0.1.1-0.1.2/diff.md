# Comparing `tmp/surfkit-0.1.1.tar.gz` & `tmp/surfkit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surfkit-0.1.1.tar", max compression
+gzip compressed data, was "surfkit-0.1.2.tar", max compression
```

## Comparing `surfkit-0.1.1.tar` & `surfkit-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.1/LICENSE
--rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.1/README.md
--rw-r--r--   0        0        0      442 2024-04-03 02:49:25.687997 surfkit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      610 2024-04-02 20:50:51.383715 surfkit-0.1.1/surfkit/agent.py
--rw-r--r--   0        0        0        0 2024-04-02 20:19:29.385009 surfkit-0.1.1/surfkit/cli.py
--rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.1/surfkit/db/conn.py
--rw-r--r--   0        0        0     5176 2024-04-03 02:09:57.525061 surfkit-0.1.1/surfkit/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:23:26.016439 surfkit-0.1.1/surfkit/env.py
--rw-r--r--   0        0        0     5444 2024-04-02 20:43:49.583063 surfkit-0.1.1/surfkit/llm.py
--rw-r--r--   0        0        0     1656 2024-04-03 02:10:36.829145 surfkit-0.1.1/surfkit/models.py
--rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.1/surfkit/types.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-02 20:08:38.101639 surfkit-0.1.2/LICENSE
+-rw-r--r--   0        0        0      270 2024-04-03 02:13:16.594885 surfkit-0.1.2/README.md
+-rw-r--r--   0        0        0      442 2024-04-03 04:02:46.035691 surfkit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      610 2024-04-02 20:50:51.383715 surfkit-0.1.2/surfkit/agent.py
+-rw-r--r--   0        0        0        0 2024-04-02 20:19:29.385009 surfkit-0.1.2/surfkit/cli.py
+-rw-r--r--   0        0        0     2013 2024-04-03 02:11:06.207281 surfkit-0.1.2/surfkit/db/conn.py
+-rw-r--r--   0        0        0     1499 2024-04-03 04:02:27.111787 surfkit-0.1.2/surfkit/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:23:26.016439 surfkit-0.1.2/surfkit/env.py
+-rw-r--r--   0        0        0     5444 2024-04-02 20:43:49.583063 surfkit-0.1.2/surfkit/llm.py
+-rw-r--r--   0        0        0     1656 2024-04-03 02:10:36.829145 surfkit-0.1.2/surfkit/models.py
+-rw-r--r--   0        0        0     9000 2024-04-03 02:10:58.047265 surfkit-0.1.2/surfkit/types.py
+-rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 surfkit-0.1.2/PKG-INFO
```

### Comparing `surfkit-0.1.1/LICENSE` & `surfkit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/surfkit/agent.py` & `surfkit-0.1.2/surfkit/agent.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/surfkit/db/conn.py` & `surfkit-0.1.2/surfkit/db/conn.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/surfkit/llm.py` & `surfkit-0.1.2/surfkit/llm.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/surfkit/models.py` & `surfkit-0.1.2/surfkit/models.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/surfkit/types.py` & `surfkit-0.1.2/surfkit/types.py`

 * *Files identical despite different names*

### Comparing `surfkit-0.1.1/PKG-INFO` & `surfkit-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surfkit
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit to build GUI surfing AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```
