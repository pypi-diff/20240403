# Comparing `tmp/giza_actions-0.2.5.tar.gz` & `tmp/giza_actions-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "giza_actions-0.2.5.tar", max compression
+gzip compressed data, was "giza_actions-0.2.6.tar", max compression
```

## Comparing `giza_actions-0.2.5.tar` & `giza_actions-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1074 2024-03-19 17:17:05.549675 giza_actions-0.2.5/LICENSE
--rw-r--r--   0        0        0     3529 2024-03-19 17:17:05.549675 giza_actions-0.2.5/README.md
--rw-r--r--   0        0        0      243 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/__init__.py
--rw-r--r--   0        0        0     5915 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/action.py
--rw-r--r--   0        0        0      542 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/deployments.py
--rw-r--r--   0        0        0      225 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/logger.py
--rw-r--r--   0        0        0     3051 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/logging.yaml
--rw-r--r--   0        0        0    14203 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/model.py
--rw-r--r--   0        0        0      519 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/task.py
--rw-r--r--   0        0        0     1597 2024-03-19 17:17:05.561675 giza_actions-0.2.5/giza_actions/utils.py
--rw-r--r--   0        0        0     1077 2024-03-19 17:17:05.561675 giza_actions-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 giza_actions-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-03 15:29:00.127403 giza_actions-0.2.6/LICENSE
+-rw-r--r--   0        0        0     3529 2024-04-03 15:29:00.127403 giza_actions-0.2.6/README.md
+-rw-r--r--   0        0        0      243 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/__init__.py
+-rw-r--r--   0        0        0     5915 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/action.py
+-rw-r--r--   0        0        0      542 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/deployments.py
+-rw-r--r--   0        0        0      225 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/logger.py
+-rw-r--r--   0        0        0     3051 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/logging.yaml
+-rw-r--r--   0        0        0    14203 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/model.py
+-rw-r--r--   0        0        0      519 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/task.py
+-rw-r--r--   0        0        0     1597 2024-04-03 15:29:00.135403 giza_actions-0.2.6/giza_actions/utils.py
+-rw-r--r--   0        0        0     1077 2024-04-03 15:29:00.139403 giza_actions-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4419 1970-01-01 00:00:00.000000 giza_actions-0.2.6/PKG-INFO
```

### Comparing `giza_actions-0.2.5/LICENSE` & `giza_actions-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/README.md` & `giza_actions-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/action.py` & `giza_actions-0.2.6/giza_actions/action.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/deployments.py` & `giza_actions-0.2.6/giza_actions/deployments.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/logging.yaml` & `giza_actions-0.2.6/giza_actions/logging.yaml`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/model.py` & `giza_actions-0.2.6/giza_actions/model.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/task.py` & `giza_actions-0.2.6/giza_actions/task.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/giza_actions/utils.py` & `giza_actions-0.2.6/giza_actions/utils.py`

 * *Files identical despite different names*

### Comparing `giza_actions-0.2.5/pyproject.toml` & `giza_actions-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "giza-actions"
-version = "0.2.5"
+version = "0.2.6"
 
 description = "A Python SDK for Giza platform"
 authors = [
     "Francisco Algaba <fran@gizatech.xyz>",
     "Raphael Doukhan <raphael@gizatech.xyz>",
     "Gonzalo Mellizo-Soto <gonzalo@gizatech.xyz>"]
 readme = "README.md"
```

### Comparing `giza_actions-0.2.5/PKG-INFO` & `giza_actions-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: giza-actions
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Python SDK for Giza platform
 License: MIT
 Author: Francisco Algaba
 Author-email: fran@gizatech.xyz
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

