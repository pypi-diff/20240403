# Comparing `tmp/ithaca_py-0.1.2.tar.gz` & `tmp/ithaca_py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.1.2.tar", max compression
+gzip compressed data, was "ithaca_py-0.1.4.tar", max compression
```

## Comparing `ithaca_py-0.1.2.tar` & `ithaca_py-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/README.md
--rw-r--r--   0        0        0     2124 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/__init__.py
--rw-r--r--   0        0        0     3656 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/analytics.py
--rw-r--r--   0        0        0    10546 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/calculation.py
--rw-r--r--   0        0        0     2921 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/client.py
--rw-r--r--   0        0        0     1787 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/constants.py
--rw-r--r--   0        0        0    11748 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/market.py
--rw-r--r--   0        0        0     6467 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/protocol.py
--rw-r--r--   0        0        0     2210 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/ithaca/socket.py
--rw-r--r--   0        0        0      909 2024-03-26 05:16:58.359021 ithaca_py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1787 1970-01-01 00:00:00.000000 ithaca_py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/README.md
+-rw-r--r--   0        0        0     3879 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/__init__.py
+-rw-r--r--   0        0        0     3656 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/analytics.py
+-rw-r--r--   0        0        0    10546 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/calculation.py
+-rw-r--r--   0        0        0     2921 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/constants.py
+-rw-r--r--   0        0        0    11748 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/market.py
+-rw-r--r--   0        0        0     6467 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/protocol.py
+-rw-r--r--   0        0        0     2210 2024-04-03 03:01:35.502890 ithaca_py-0.1.4/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-04-03 03:01:35.506890 ithaca_py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.1.4/PKG-INFO
```

### Comparing `ithaca_py-0.1.2/README.md` & `ithaca_py-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/analytics.py` & `ithaca_py-0.1.4/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/auth.py` & `ithaca_py-0.1.4/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/calculation.py` & `ithaca_py-0.1.4/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/client.py` & `ithaca_py-0.1.4/ithaca/client.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/constants.py` & `ithaca_py-0.1.4/ithaca/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Environment Constants."""
+"""
+Environment Constants. (Depreciated in favor of manually specifying endpoints))
+"""
 
 ENVS = {
     "PRODUCTION": {
         "base_url": "https://app.ithacaprotocol.io/api/v1",
         "ws_url": "wss://app.ithacaprotocol.io",
         "rpc_url": "https://arbitrum.llamarpc.com",
         "subgraph": "https://api.studio.thegraph.com/query/43740/ithaca-arbitrum/v1.1.0",  # type: ignore  # noqa: E501
```

### Comparing `ithaca_py-0.1.2/ithaca/fundlock.py` & `ithaca_py-0.1.4/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/market.py` & `ithaca_py-0.1.4/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/orders.py` & `ithaca_py-0.1.4/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/protocol.py` & `ithaca_py-0.1.4/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/ithaca/socket.py` & `ithaca_py-0.1.4/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.1.2/pyproject.toml` & `ithaca_py-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.1.2"
+version = "0.1.4"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.31.0"
+tenacity = "^8.2.3"
 pre-commit = "^3.6.0"
 eth-account = "^0.10.0"
 pandas = "^2.1.4"
 scipy = "^1.11.4"
 pydantic = "^2.5.3"
 websocket-client = "^1.7.0"
 web3 = "^6.13.0"
```

### Comparing `ithaca_py-0.1.2/PKG-INFO` & `ithaca_py-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.1.2
+Version: 0.1.4
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,14 +13,15 @@
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: eth-account (>=0.10.0,<0.11.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pre-commit (>=3.6.0,<4.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
+Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: web3 (>=6.13.0,<7.0.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Ithaca SDK
 
 ## Modules
```

