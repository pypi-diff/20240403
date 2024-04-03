# Comparing `tmp/pluto_client-0.0.4.tar.gz` & `tmp/pluto_client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluto_client-0.0.4.tar", max compression
+gzip compressed data, was "pluto_client-0.0.5.tar", max compression
```

## Comparing `pluto_client-0.0.4.tar` & `pluto_client-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10139 2024-03-04 09:36:11.277261 pluto_client-0.0.4/LICENSE
--rw-r--r--   0        0        0      241 2024-03-04 09:53:06.700908 pluto_client-0.0.4/README.md
--rw-r--r--   0        0        0      213 2024-03-15 13:09:08.015459 pluto_client-0.0.4/pluto_client/__init__.py
--rw-r--r--   0        0        0        0 2024-03-15 13:09:08.015577 pluto_client-0.0.4/pluto_client/clients/__init__.py
--rw-r--r--   0        0        0      153 2024-03-15 13:09:08.015893 pluto_client-0.0.4/pluto_client/clients/aws/__init__.py
--rw-r--r--   0        0        0     2788 2024-03-15 13:09:08.016207 pluto_client-0.0.4/pluto_client/clients/aws/function_lambda.py
--rw-r--r--   0        0        0     1018 2024-03-21 07:20:28.915114 pluto_client-0.0.4/pluto_client/clients/aws/kvstore_dynamodb.py
--rw-r--r--   0        0        0     1198 2024-03-19 08:53:57.300643 pluto_client-0.0.4/pluto_client/clients/aws/queue_sns.py
--rw-r--r--   0        0        0     1137 2024-03-19 08:11:58.019950 pluto_client-0.0.4/pluto_client/clients/aws/sagemaker.py
--rw-r--r--   0        0        0      566 2024-03-19 08:50:14.849372 pluto_client-0.0.4/pluto_client/clients/aws/utils.py
--rw-r--r--   0        0        0      187 2024-03-15 13:09:08.018112 pluto_client-0.0.4/pluto_client/clients/errors.py
--rw-r--r--   0        0        0       33 2024-03-15 13:09:08.018977 pluto_client-0.0.4/pluto_client/clients/shared/__init__.py
--rw-r--r--   0        0        0      407 2024-03-15 13:09:08.019149 pluto_client-0.0.4/pluto_client/clients/shared/router.py
--rw-r--r--   0        0        0     1811 2024-03-19 07:46:00.418455 pluto_client-0.0.4/pluto_client/function.py
--rw-r--r--   0        0        0     1703 2024-03-21 07:19:28.117834 pluto_client-0.0.4/pluto_client/kvstore.py
--rw-r--r--   0        0        0     1889 2024-03-19 07:53:52.860963 pluto_client-0.0.4/pluto_client/queue.py
--rw-r--r--   0        0        0     1961 2024-03-19 07:47:09.883777 pluto_client-0.0.4/pluto_client/router.py
--rw-r--r--   0        0        0     3610 2024-03-21 07:58:44.060299 pluto_client-0.0.4/pluto_client/sagemaker.py
--rw-r--r--   0        0        0      796 2024-03-21 12:17:31.347653 pluto_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    10139 2024-03-22 03:06:50.256126 pluto_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0      241 2024-03-22 03:06:50.261224 pluto_client-0.0.5/README.md
+-rw-r--r--   0        0        0      213 2024-03-22 03:06:50.263830 pluto_client-0.0.5/pluto_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-22 03:06:50.264201 pluto_client-0.0.5/pluto_client/clients/__init__.py
+-rw-r--r--   0        0        0      153 2024-03-22 03:06:50.267637 pluto_client-0.0.5/pluto_client/clients/aws/__init__.py
+-rw-r--r--   0        0        0     2788 2024-03-22 03:06:50.270114 pluto_client-0.0.5/pluto_client/clients/aws/function_lambda.py
+-rw-r--r--   0        0        0     1018 2024-03-25 12:43:18.628466 pluto_client-0.0.5/pluto_client/clients/aws/kvstore_dynamodb.py
+-rw-r--r--   0        0        0     1198 2024-03-22 03:06:50.273165 pluto_client-0.0.5/pluto_client/clients/aws/queue_sns.py
+-rw-r--r--   0        0        0     1137 2024-03-22 03:06:50.274687 pluto_client-0.0.5/pluto_client/clients/aws/sagemaker.py
+-rw-r--r--   0        0        0      566 2024-03-22 03:06:50.276066 pluto_client-0.0.5/pluto_client/clients/aws/utils.py
+-rw-r--r--   0        0        0      187 2024-03-22 03:06:50.277629 pluto_client-0.0.5/pluto_client/clients/errors.py
+-rw-r--r--   0        0        0       33 2024-03-22 03:06:50.279344 pluto_client-0.0.5/pluto_client/clients/shared/__init__.py
+-rw-r--r--   0        0        0      407 2024-03-22 03:06:50.281053 pluto_client-0.0.5/pluto_client/clients/shared/router.py
+-rw-r--r--   0        0        0     1811 2024-03-22 03:06:50.282386 pluto_client-0.0.5/pluto_client/function.py
+-rw-r--r--   0        0        0     1703 2024-03-25 12:43:18.630810 pluto_client-0.0.5/pluto_client/kvstore.py
+-rw-r--r--   0        0        0     1889 2024-03-22 03:06:50.285147 pluto_client-0.0.5/pluto_client/queue.py
+-rw-r--r--   0        0        0     2059 2024-04-01 03:42:12.388520 pluto_client-0.0.5/pluto_client/router.py
+-rw-r--r--   0        0        0     3610 2024-03-25 12:43:18.634467 pluto_client-0.0.5/pluto_client/sagemaker.py
+-rw-r--r--   0        0        0      796 2024-04-03 08:24:36.909155 pluto_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1146 1970-01-01 00:00:00.000000 pluto_client-0.0.5/PKG-INFO
```

### Comparing `pluto_client-0.0.4/LICENSE` & `pluto_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/clients/aws/function_lambda.py` & `pluto_client-0.0.5/pluto_client/clients/aws/function_lambda.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/clients/aws/kvstore_dynamodb.py` & `pluto_client-0.0.5/pluto_client/clients/aws/kvstore_dynamodb.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/clients/aws/queue_sns.py` & `pluto_client-0.0.5/pluto_client/clients/aws/queue_sns.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/clients/aws/sagemaker.py` & `pluto_client-0.0.5/pluto_client/clients/aws/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/clients/aws/utils.py` & `pluto_client-0.0.5/pluto_client/clients/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/function.py` & `pluto_client-0.0.5/pluto_client/function.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/kvstore.py` & `pluto_client-0.0.5/pluto_client/kvstore.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/queue.py` & `pluto_client-0.0.5/pluto_client/queue.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pluto_client/router.py` & `pluto_client-0.0.5/pluto_client/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     def put(self, path: str, fn: RequestHandler):
         raise NotImplementedError
 
     def delete(self, path: str, fn: RequestHandler):
         raise NotImplementedError
 
+    def all(self, path: str, fn: Callable, raw: bool = False):
+        raise NotImplementedError
+
 
 class IRouterCapturedProps(resource.IResourceCapturedProps):
     def url(self) -> str:
         raise NotImplementedError
 
 
 class IRouterClient(IRouterClientApi, IRouterCapturedProps):
```

### Comparing `pluto_client-0.0.4/pluto_client/sagemaker.py` & `pluto_client-0.0.5/pluto_client/sagemaker.py`

 * *Files identical despite different names*

### Comparing `pluto_client-0.0.4/pyproject.toml` & `pluto_client-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pluto-client"
-version = "0.0.4"
+version = "0.0.5"
 description = "The Client Library for Pluto Programming Language."
 authors = ["Jade Zheng <zheng.shoujian@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 classifiers = [
     'Development Status :: 1 - Planning',
     'Environment :: Console',
```

### Comparing `pluto_client-0.0.4/PKG-INFO` & `pluto_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluto-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: The Client Library for Pluto Programming Language.
 License: Apache-2.0
 Author: Jade Zheng
 Author-email: zheng.shoujian@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

