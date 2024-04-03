# Comparing `tmp/kservehelper-1.2.1.tar.gz` & `tmp/kservehelper-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kservehelper-1.2.1.tar", last modified: Fri Mar 22 13:17:00 2024, max compression
+gzip compressed data, was "kservehelper-1.2.2.tar", last modified: Wed Apr  3 03:06:00 2024, max compression
```

## Comparing `kservehelper-1.2.1.tar` & `kservehelper-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.504782 kservehelper-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-03-22 13:17:00.504782 kservehelper-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-22 13:16:53.000000 kservehelper-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.496781 kservehelper-1.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.496781 kservehelper-1.2.1/examples/blur-image/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/blur-image/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.496781 kservehelper-1.2.1/examples/dummy/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/dummy/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.496781 kservehelper-1.2.1/examples/rotate-image/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/rotate-image/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.496781 kservehelper-1.2.1/examples/stable-diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/stable-diffusion/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/stable-diffusion/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.500781 kservehelper-1.2.1/examples/stable-diffusion-xl/
--rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-03-22 13:16:53.000000 kservehelper-1.2.1/examples/stable-diffusion-xl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.500781 kservehelper-1.2.1/kservehelper/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.500781 kservehelper-1.2.1/kservehelper/kserve/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/kserve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/kserve/model_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.504782 kservehelper-1.2.1/kservehelper/kserve/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/kserve/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/kserve/rest/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/kserve/rest/v1_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-03-22 13:16:53.000000 kservehelper-1.2.1/kservehelper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.504782 kservehelper-1.2.1/kservehelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-22 13:17:00.000000 kservehelper-1.2.1/kservehelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 13:17:00.504782 kservehelper-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-22 13:16:53.000000 kservehelper-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 13:17:00.504782 kservehelper-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_batch_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_model_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_predict.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-22 13:16:53.000000 kservehelper-1.2.1/tests/test_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-03 03:06:00.181577 kservehelper-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-03 03:05:52.000000 kservehelper-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/blur-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/blur-image/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/dummy/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/rotate-image/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/rotate-image/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/stable-diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.173577 kservehelper-1.2.2/examples/stable-diffusion-xl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-04-03 03:05:52.000000 kservehelper-1.2.2/examples/stable-diffusion-xl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14033 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9089 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/kserve/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/model_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.177577 kservehelper-1.2.2/kservehelper/kserve/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/kserve/rest/v1_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11422 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9883 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-03 03:05:52.000000 kservehelper-1.2.2/kservehelper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/kservehelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:05:59.000000 kservehelper-1.2.2/kservehelper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 03:06:00.000000 kservehelper-1.2.2/kservehelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 03:06:00.181577 kservehelper-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 03:05:52.000000 kservehelper-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:06:00.181577 kservehelper-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_batch_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_model_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-03 03:05:52.000000 kservehelper-1.2.2/tests/test_upload.py
```

### Comparing `kservehelper-1.2.1/PKG-INFO` & `kservehelper-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kservehelper
-Version: 1.2.1
+Version: 1.2.2
 Summary: A KServe Model Wrapper
 Home-page: https://github.com/yangwenz/kserve-helper
 Author: Wenzhuo Yang
 License: 3-Clause BSD
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Requires-Dist: kserve==0.10.2
```

### Comparing `kservehelper-1.2.1/README.md` & `kservehelper-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/examples/blur-image/model.py` & `kservehelper-1.2.2/examples/blur-image/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/examples/dummy/model.py` & `kservehelper-1.2.2/examples/dummy/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/examples/rotate-image/model.py` & `kservehelper-1.2.2/examples/rotate-image/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/examples/stable-diffusion/model.py` & `kservehelper-1.2.2/examples/stable-diffusion/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/examples/stable-diffusion-xl/model.py` & `kservehelper-1.2.2/examples/stable-diffusion-xl/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/cache.py` & `kservehelper-1.2.2/kservehelper/cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/cli.py` & `kservehelper-1.2.2/kservehelper/cli.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/docker.py` & `kservehelper-1.2.2/kservehelper/docker.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/kserve/model_server.py` & `kservehelper-1.2.2/kservehelper/kserve/model_server.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/kserve/rest/server.py` & `kservehelper-1.2.2/kservehelper/kserve/rest/server.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/kserve/rest/v1_endpoints.py` & `kservehelper-1.2.2/kservehelper/kserve/rest/v1_endpoints.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/model.py` & `kservehelper-1.2.2/kservehelper/model.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/storage.py` & `kservehelper-1.2.2/kservehelper/storage.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/types.py` & `kservehelper-1.2.2/kservehelper/types.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/kservehelper/utils.py` & `kservehelper-1.2.2/kservehelper/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import requests
 import concurrent.futures
 from typing import List
 from contextlib import contextmanager
 from kservehelper.types import Path
 
 
-def upload_files(webhook_url: str, paths: List[Path], timeout=90):
+def upload_files(webhook_url: str, paths: List[Path], timeout=60):
     # outputs = asyncio.run(_upload_v2(webhook_url, paths, timeout))
     # return outputs
     if webhook_url.endswith("upload"):
         outputs = _upload_multithread(webhook_url, paths, timeout)
     elif webhook_url.endswith("upload_batch"):
         outputs = _upload_batch(webhook_url, paths, timeout)
     else:
@@ -33,73 +33,81 @@
         if response.status_code != 200:
             raise RuntimeError("failed to call upload webhook")
         r = json.loads(response.text)
         outputs.append(r["url"])
     return outputs
 
 
-def _upload_batch(webhook_url: str, paths: List[Path], timeout, retires=4):
-    files, file_list = {}, []
-    for i, path in enumerate(paths):
-        filepath = str(path)
-        f = open(filepath, "rb")
-        files[f"file_{i}"] = (filepath, f)
-        file_list.append(f)
-
+def _upload_batch(webhook_url: str, paths: List[Path], timeout, retires=3):
     error = None
-    for i in range(retires):
+    result = {}
+
+    for retry in range(retires):
+        # Open a list of files
+        files, file_list = {}, []
+        for i, path in enumerate(paths):
+            filepath = str(path)
+            f = open(filepath, "rb")
+            files[f"file_{i}"] = (filepath, f)
+            file_list.append(f)
+
+        # Send a batch of files
         try:
             response = requests.post(
                 webhook_url,
                 headers={"NUM_FILES": str(len(file_list))},
                 files=files,
                 timeout=timeout
             )
+            if response.status_code != 200:
+                raise RuntimeError(f"response status code is {response.status_code}")
             error = None
-            break
+            result = json.loads(response.text)
         except Exception as e:
             print(f"UPLOAD ERROR: {str(e)}")
             error = e
-            time.sleep(2 * (i + 1))
+            time.sleep(2 * (retry + 1))
+
+        # Close the files
+        for f in file_list:
+            f.close()
+        if error is None:
+            break
 
-    for f in file_list:
-        f.close()
     if error is not None:
         raise error
-    if response.status_code != 200:
-        raise RuntimeError("failed to call upload_batch webhook")
-    r = json.loads(response.text)
-    return r["urls"]
+    return result["urls"]
 
 
-def _upload_multithread(webhook_url: str, paths: List[Path], timeout):
+def _upload_multithread(webhook_url: str, paths: List[Path], timeout, retires=3):
     def _make_request(filepath):
-        with open(filepath, "rb") as f:
-            files = {"file": (filepath, f)}
-            for i in range(3):
+        for i in range(retires):
+            with open(filepath, "rb") as f:
+                files = {"file": (filepath, f)}
                 try:
                     response = requests.post(webhook_url, files=files, timeout=timeout)
                     if response.status_code != 200:
                         raise RuntimeError(f"response status code is {response.status_code}")
                     r = json.loads(response.text)
                     return filepath, r["url"]
                 except Exception as e:
                     print(f"ERROR: {e}")
                     print(f"Retrying {i + 1}...")
-            return None
+                    time.sleep((i + 1) * 2)
+        return None
 
     with concurrent.futures.ThreadPoolExecutor(max_workers=4) as executor:
         jobs = [executor.submit(_make_request, str(path)) for path in paths]
         outputs = [job.result() for job in concurrent.futures.as_completed(jobs)]
         for path in paths:
             file = str(path)
             if os.path.exists(file):
                 os.remove(file)
         if None in outputs:
-            raise RuntimeError("failed to call upload webhook")
+            raise RuntimeError("failed to upload files")
 
     filename2url = dict(outputs)
     return [filename2url[str(path)] for path in paths]
 
 
 async def _async_upload_v1(webhook_url: str, paths: List[Path], timeout):
     outputs = []
```

### Comparing `kservehelper-1.2.1/kservehelper.egg-info/PKG-INFO` & `kservehelper-1.2.2/kservehelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kservehelper
-Version: 1.2.1
+Version: 1.2.2
 Summary: A KServe Model Wrapper
 Home-page: https://github.com/yangwenz/kserve-helper
 Author: Wenzhuo Yang
 License: 3-Clause BSD
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
 Requires-Dist: kserve==0.10.2
```

### Comparing `kservehelper-1.2.1/kservehelper.egg-info/SOURCES.txt` & `kservehelper-1.2.2/kservehelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/setup.py` & `kservehelper-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="kservehelper",
-    version="1.2.1",
+    version="1.2.2",
     author="Wenzhuo Yang",
     description="A KServe Model Wrapper",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/yangwenz/kserve-helper",
     license="3-Clause BSD",
     packages=find_namespace_packages(include="kservehelper.*"),
```

### Comparing `kservehelper-1.2.1/tests/test_batch_inputs.py` & `kservehelper-1.2.2/tests/test_batch_inputs.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_cache.py` & `kservehelper-1.2.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_model_cache.py` & `kservehelper-1.2.2/tests/test_model_cache.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_predict.py` & `kservehelper-1.2.2/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_s3.py` & `kservehelper-1.2.2/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_transform.py` & `kservehelper-1.2.2/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `kservehelper-1.2.1/tests/test_upload.py` & `kservehelper-1.2.2/tests/test_upload.py`

 * *Files identical despite different names*

