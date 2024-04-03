# Comparing `tmp/safe_ds_runner-0.7.0.tar.gz` & `tmp/safe_ds_runner-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe_ds_runner-0.7.0.tar", max compression
+gzip compressed data, was "safe_ds_runner-0.8.0.tar", max compression
```

## Comparing `safe_ds_runner-0.7.0.tar` & `safe_ds_runner-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-02-22 08:41:23.645965 safe_ds_runner-0.7.0/LICENSE
--rw-r--r--   0        0        0     1367 2024-02-22 08:41:23.645965 safe_ds_runner-0.7.0/docs/README.md
--rw-r--r--   0        0        0     1037 2024-02-22 08:42:05.226130 safe_ds_runner-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      229 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/__init__.py
--rw-r--r--   0        0        0       95 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/cli/__init__.py
--rw-r--r--   0        0        0     1368 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/cli/_cli.py
--rw-r--r--   0        0        0      165 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/main.py
--rw-r--r--   0        0        0      109 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/__init__.py
--rw-r--r--   0        0        0     1719 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_json_encoder.py
--rw-r--r--   0        0        0    10612 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_memoization_map.py
--rw-r--r--   0        0        0    14539 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_messages.py
--rw-r--r--   0        0        0     5214 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_module_manager.py
--rw-r--r--   0        0        0    13858 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_pipeline_manager.py
--rw-r--r--   0        0        0     8593 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/_server.py
--rw-r--r--   0        0        0      523 2024-02-22 08:41:23.653965 safe_ds_runner-0.7.0/src/safeds_runner/server/main.py
--rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 safe_ds_runner-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-03 09:11:40.541854 safe_ds_runner-0.8.0/LICENSE
+-rw-r--r--   0        0        0     1367 2024-04-03 09:11:40.541854 safe_ds_runner-0.8.0/docs/README.md
+-rw-r--r--   0        0        0     1037 2024-04-03 09:12:39.533680 safe_ds_runner-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/__init__.py
+-rw-r--r--   0        0        0       95 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/cli/__init__.py
+-rw-r--r--   0        0        0     1368 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/cli/_cli.py
+-rw-r--r--   0        0        0      165 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/main.py
+-rw-r--r--   0        0        0      109 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/__init__.py
+-rw-r--r--   0        0        0     1812 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_json_encoder.py
+-rw-r--r--   0        0        0    10612 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_memoization_map.py
+-rw-r--r--   0        0        0    14539 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_messages.py
+-rw-r--r--   0        0        0     5214 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_module_manager.py
+-rw-r--r--   0        0        0    14045 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_pipeline_manager.py
+-rw-r--r--   0        0        0     8593 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/_server.py
+-rw-r--r--   0        0        0      523 2024-04-03 09:11:40.545854 safe_ds_runner-0.8.0/src/safeds_runner/server/main.py
+-rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 safe_ds_runner-0.8.0/PKG-INFO
```

### Comparing `safe_ds_runner-0.7.0/LICENSE` & `safe_ds_runner-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/docs/README.md` & `safe_ds_runner-0.8.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/pyproject.toml` & `safe_ds_runner-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "safe-ds-runner"
-version = "0.7.0"
+version = "0.8.0"
 description = "Execute Safe-DS programs that were compiled to Python."
 authors = ["Lars Reimann <mail@larsreimann.com>"]
 license = "MIT"
 readme = "docs/README.md"
 repository = "https://github.com/Safe-DS/Runner"
 documentation = "https://safe-ds-runner.readthedocs.io"
 keywords = ["data-science", "machine-learning", "usability", "learnability"]
@@ -13,23 +13,23 @@
 ]
 
 [tool.poetry.scripts]
 safe-ds-runner = "safeds_runner.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11,<3.13"
-safe-ds = ">=0.19,<0.20"
+safe-ds = ">=0.19,<0.21"
 hypercorn = "^0.16.0"
 quart = "^0.19.4"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.4.4"
-pytest-cov = "^4.1.0"
-pytest-timeout = "^2.2.0"
-pytest-asyncio = "^0.23.4"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+pytest-timeout = "^2.3.1"
+pytest-asyncio = "^0.23.6"
 simple-websocket = "^1.0.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-glightbox = "^0.3.4"
 mkdocs-material = "^9.1.17"
```

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/cli/_cli.py` & `safe_ds_runner-0.8.0/src/safeds_runner/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_json_encoder.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_json_encoder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """Module containing JSON encoding utilities for Safe-DS types."""
 
 import base64
 import json
 import math
 from typing import Any
 
-from safeds.data.image.containers import Image
-from safeds.data.tabular.containers import Table
-
 
 class SafeDsEncoder(json.JSONEncoder):
     """JSON Encoder for custom Safe-DS types."""
 
     def default(self, o: Any) -> Any:
         """
         Convert specific Safe-DS types to a JSON-serializable representation.
@@ -26,14 +23,18 @@
             An object that needs to be encoded to JSON.
 
         Returns
         -------
         Any
             The passed object represented in a way that is serializable to JSON.
         """
+        # Moving these imports to the top drastically increases startup time
+        from safeds.data.image.containers import Image
+        from safeds.data.tabular.containers import Table
+
         if isinstance(o, Table):
             dict_with_nan_infinity = o.to_dict()
             # Convert NaN / Infinity to None, as the JSON encoder generates invalid JSON otherwise
             return {
                 key: [
                     value if not isinstance(value, float) or math.isfinite(value) else None
                     for value in dict_with_nan_infinity[key]
```

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_memoization_map.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_memoization_map.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_messages.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_messages.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_module_manager.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_module_manager.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_pipeline_manager.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_pipeline_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -225,14 +225,20 @@
         Parameters
         ----------
         placeholder_name : str
             Name of the placeholder.
         value : Any
             Actual value of the placeholder.
         """
+        from safeds.data.image.containers import Image
+
+        if isinstance(value, Image):
+            import torch
+
+            value = Image(value._image_tensor, torch.device("cpu"))
         self._placeholder_map[placeholder_name] = value
         placeholder_type = _get_placeholder_type(value)
         self._send_message(
             message_type_placeholder_type,
             create_placeholder_description(placeholder_name, placeholder_type),
         )
```

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/_server.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/_server.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/src/safeds_runner/server/main.py` & `safe_ds_runner-0.8.0/src/safeds_runner/server/main.py`

 * *Files identical despite different names*

### Comparing `safe_ds_runner-0.7.0/PKG-INFO` & `safe_ds_runner-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: safe-ds-runner
-Version: 0.7.0
+Version: 0.8.0
 Summary: Execute Safe-DS programs that were compiled to Python.
 Home-page: https://github.com/Safe-DS/Runner
 License: MIT
 Keywords: data-science,machine-learning,usability,learnability
 Author: Lars Reimann
 Author-email: mail@larsreimann.com
 Requires-Python: >=3.11,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: hypercorn (>=0.16.0,<0.17.0)
 Requires-Dist: quart (>=0.19.4,<0.20.0)
-Requires-Dist: safe-ds (>=0.19,<0.20)
+Requires-Dist: safe-ds (>=0.19,<0.21)
 Project-URL: Documentation, https://safe-ds-runner.readthedocs.io
 Project-URL: Repository, https://github.com/Safe-DS/Runner
 Description-Content-Type: text/markdown
 
 # Safe-DS Runner
 
 [![PyPI](https://img.shields.io/pypi/v/safe-ds-runner)](https://pypi.org/project/safe-ds-runner)
```

