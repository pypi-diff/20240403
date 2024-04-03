# Comparing `tmp/ithaca_py-0.1.4.tar.gz` & `tmp/ithaca_py-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.1.4.tar", max compression
+gzip compressed data, was "ithaca_py-0.1.5.tar", max compression
```

## Comparing `ithaca_py-0.1.4.tar` & `ithaca_py-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/README.md
--rw-r--r--   0        0        0     3879 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/analytics.py
--rw-r--r--   0        0        0    10546 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/calculation.py
--rw-r--r--   0        0        0     2921 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/constants.py
--rw-r--r--   0        0        0    11748 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/market.py
--rw-r--r--   0        0        0     6467 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-04-03 03:01:35.506890 ithaca_py-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-03 05:55:39.961056 ithaca_py-0.1.5/README.md
+-rw-r--r--   0        0        0     3858 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/analytics.py
+-rw-r--r--   0        0        0    10546 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/calculation.py
+-rw-r--r--   0        0        0     2921 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/constants.py
+-rw-r--r--   0        0        0    11748 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/market.py
+-rw-r--r--   0        0        0     6467 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-03 05:55:39.965056 ithaca_py-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.5/PKG-INFO
```

### Comparing `ithaca_py-0.1.4/README.md` & `ithaca_py-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/__init__.py` & `ithaca_py-0.1.5/ithaca/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,32 +33,32 @@
         fundlock (Fundlock): Fundlock
         analytics (Analytics): Analytics
     """
 
     def __init__(
             self, 
             private_key, 
-            api_endpoint,
-            ws_endpoint,
-            graphql_endpoint,
-            rpc_endpoint,
+            api_endpoint=None,
+            ws_endpoint=None,
+            graphql_endpoint=None,
+            rpc_endpoint=None,
             env_name="CANARY"):
         """
         Ithaca SDK Constructor. By default, one should specify a private_key for on-chain and backend authentication followed by the environment one wishes to access.
         
         Args:
           private_key (str): Private Key
           api_endpoint (str): API Endpoint
           ws_endpoint (str): Websocket Endpoint
           graphql_endpoint (str): Graphql Endpoint
           rpc_endpoint (str): RPC Endpoint
           env_name (str): (Depreciated) Environment Name
         """
-        if all(endpoint is not None for endpoint in [api_endpoint, ws_endpoint, graphql_endpoint, rpc_endpoint]):
-          logging.warning("Endpoint specifications not found, defaulting to 'env_name: {0}".format(env_name))
+        if not all([api_endpoint, ws_endpoint, graphql_endpoint, rpc_endpoint]):
+          logging.warning(f"Endpoint specifications not found, defaulting to 'env_name': {env_name}")
           self.env = ENVS.get(env_name)
         else:
           self.env = {
             "base_url": api_endpoint,
             "ws_url": ws_endpoint,
             "subgraph": graphql_endpoint,
             "rpc_url": rpc_endpoint
```

### Comparing `ithaca_py-0.1.4/ithaca/analytics.py` & `ithaca_py-0.1.5/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/auth.py` & `ithaca_py-0.1.5/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/calculation.py` & `ithaca_py-0.1.5/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/client.py` & `ithaca_py-0.1.5/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/constants.py` & `ithaca_py-0.1.5/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/fundlock.py` & `ithaca_py-0.1.5/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/market.py` & `ithaca_py-0.1.5/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/orders.py` & `ithaca_py-0.1.5/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/protocol.py` & `ithaca_py-0.1.5/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/ithaca/socket.py` & `ithaca_py-0.1.5/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.4/pyproject.toml` & `ithaca_py-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.1.4/PKG-INFO` & `ithaca_py-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

