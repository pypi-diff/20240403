# Comparing `tmp/betfair_parser-0.9.0.tar.gz` & `tmp/betfair_parser-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betfair_parser-0.9.0.tar", max compression
+gzip compressed data, was "betfair_parser-0.9.1.tar", max compression
```

## Comparing `betfair_parser-0.9.0.tar` & `betfair_parser-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1286 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/LICENSE.txt
--rw-r--r--   0        0        0     3394 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/README.md
--rw-r--r--   0        0        0        0 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/__init__.py
--rw-r--r--   0        0        0     8890 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/cache.py
--rw-r--r--   0        0        0     2090 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/client.py
--rw-r--r--   0        0        0     2632 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/endpoints.py
--rw-r--r--   0        0        0      930 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/exceptions.py
--rw-r--r--   0        0        0        0 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/__init__.py
--rw-r--r--   0        0        0      977 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/accounts/__init__.py
--rw-r--r--   0        0        0     2929 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/accounts/enums.py
--rw-r--r--   0        0        0     3154 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/accounts/operations.py
--rw-r--r--   0        0        0    11141 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/accounts/type_definitions.py
--rw-r--r--   0        0        0     2301 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/__init__.py
--rw-r--r--   0        0        0    21875 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/enums.py
--rw-r--r--   0        0        0     9223 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/listings.py
--rw-r--r--   0        0        0      134 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/operations.py
--rw-r--r--   0        0        0     8621 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/orders.py
--rw-r--r--   0        0        0    33043 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/betting/type_definitions.py
--rw-r--r--   0        0        0      853 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/common/__init__.py
--rw-r--r--   0        0        0     9771 2023-11-05 01:28:28.743436 betfair_parser-0.9.0/betfair_parser/spec/common/enums.py
--rw-r--r--   0        0        0     6633 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/common/messages.py
--rw-r--r--   0        0        0     1806 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/common/type_definitions.py
--rw-r--r--   0        0        0     2852 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/heartbeat.py
--rw-r--r--   0        0        0     8651 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/identity.py
--rw-r--r--   0        0        0     3891 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/navigation.py
--rw-r--r--   0        0        0     3239 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/race_status.py
--rw-r--r--   0        0        0     1712 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/streaming/__init__.py
--rw-r--r--   0        0        0     4864 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/streaming/enums.py
--rw-r--r--   0        0        0     6219 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/streaming/messages.py
--rw-r--r--   0        0        0    17054 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/spec/streaming/type_definitions.py
--rw-r--r--   0        0        0     5555 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/stream.py
--rw-r--r--   0        0        0     2477 2023-11-05 01:28:28.747436 betfair_parser-0.9.0/betfair_parser/strenums.py
--rw-r--r--   0        0        0     2150 2023-11-05 01:28:45.435589 betfair_parser-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 betfair_parser-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1286 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/LICENSE.txt
+-rw-r--r--   0        0        0     3394 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/README.md
+-rw-r--r--   0        0        0        0 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/__init__.py
+-rw-r--r--   0        0        0     8890 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/cache.py
+-rw-r--r--   0        0        0     2090 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/client.py
+-rw-r--r--   0        0        0     2632 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/endpoints.py
+-rw-r--r--   0        0        0      930 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/exceptions.py
+-rw-r--r--   0        0        0        0 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/spec/__init__.py
+-rw-r--r--   0        0        0      977 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/spec/accounts/__init__.py
+-rw-r--r--   0        0        0     2929 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/spec/accounts/enums.py
+-rw-r--r--   0        0        0     3154 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/spec/accounts/operations.py
+-rw-r--r--   0        0        0    11141 2023-11-06 00:01:16.837925 betfair_parser-0.9.1/betfair_parser/spec/accounts/type_definitions.py
+-rw-r--r--   0        0        0     2301 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/__init__.py
+-rw-r--r--   0        0        0    21875 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/enums.py
+-rw-r--r--   0        0        0     9223 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/listings.py
+-rw-r--r--   0        0        0      134 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/operations.py
+-rw-r--r--   0        0        0     8621 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/orders.py
+-rw-r--r--   0        0        0    33043 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/betting/type_definitions.py
+-rw-r--r--   0        0        0      853 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/common/__init__.py
+-rw-r--r--   0        0        0     9771 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/common/enums.py
+-rw-r--r--   0        0        0     6633 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/common/messages.py
+-rw-r--r--   0        0        0     1806 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/common/type_definitions.py
+-rw-r--r--   0        0        0     2852 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/heartbeat.py
+-rw-r--r--   0        0        0     8666 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/identity.py
+-rw-r--r--   0        0        0     3891 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/navigation.py
+-rw-r--r--   0        0        0     3239 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/race_status.py
+-rw-r--r--   0        0        0     1712 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/streaming/__init__.py
+-rw-r--r--   0        0        0     4864 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/streaming/enums.py
+-rw-r--r--   0        0        0     6219 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/streaming/messages.py
+-rw-r--r--   0        0        0    17054 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/spec/streaming/type_definitions.py
+-rw-r--r--   0        0        0     5555 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/stream.py
+-rw-r--r--   0        0        0     2477 2023-11-06 00:01:16.841925 betfair_parser-0.9.1/betfair_parser/strenums.py
+-rw-r--r--   0        0        0     2150 2023-11-06 00:01:27.933875 betfair_parser-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3894 1970-01-01 00:00:00.000000 betfair_parser-0.9.1/PKG-INFO
```

### Comparing `betfair_parser-0.9.0/LICENSE.txt` & `betfair_parser-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/README.md` & `betfair_parser-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/cache.py` & `betfair_parser-0.9.1/betfair_parser/cache.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/client.py` & `betfair_parser-0.9.1/betfair_parser/client.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/endpoints.py` & `betfair_parser-0.9.1/betfair_parser/endpoints.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/exceptions.py` & `betfair_parser-0.9.1/betfair_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/accounts/__init__.py` & `betfair_parser-0.9.1/betfair_parser/spec/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/accounts/enums.py` & `betfair_parser-0.9.1/betfair_parser/spec/accounts/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/accounts/operations.py` & `betfair_parser-0.9.1/betfair_parser/spec/accounts/operations.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/accounts/type_definitions.py` & `betfair_parser-0.9.1/betfair_parser/spec/accounts/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/betting/__init__.py` & `betfair_parser-0.9.1/betfair_parser/spec/betting/__init__.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/betting/enums.py` & `betfair_parser-0.9.1/betfair_parser/spec/betting/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/betting/listings.py` & `betfair_parser-0.9.1/betfair_parser/spec/betting/listings.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/betting/orders.py` & `betfair_parser-0.9.1/betfair_parser/spec/betting/orders.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/betting/type_definitions.py` & `betfair_parser-0.9.1/betfair_parser/spec/betting/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/common/__init__.py` & `betfair_parser-0.9.1/betfair_parser/spec/common/__init__.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/common/enums.py` & `betfair_parser-0.9.1/betfair_parser/spec/common/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/common/messages.py` & `betfair_parser-0.9.1/betfair_parser/spec/common/messages.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/common/type_definitions.py` & `betfair_parser-0.9.1/betfair_parser/spec/common/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/heartbeat.py` & `betfair_parser-0.9.1/betfair_parser/spec/heartbeat.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/identity.py` & `betfair_parser-0.9.1/betfair_parser/spec/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         return self.login_status if self.is_error else None
 
     @property
     def is_error(self):
         return self.status != LoginExceptionCode.SUCCESS
 
 
-class CertLogin(_IdentityRequest, kw_only=True, frozen=True):
+class CertLogin(_IdentityRequest, kw_only=True, frozen=True, tag=str.lower):
     # Subclassing Login would have been more obvious, but then mypy freaks out
     # due to a different return_type
 
     endpoint_type = EndpointType.IDENTITY_CERT
     params: _LoginParams
     return_type = CertLoginResponse
     throws = LoginImpossible
```

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/navigation.py` & `betfair_parser-0.9.1/betfair_parser/spec/navigation.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/race_status.py` & `betfair_parser-0.9.1/betfair_parser/spec/race_status.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/streaming/__init__.py` & `betfair_parser-0.9.1/betfair_parser/spec/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/streaming/enums.py` & `betfair_parser-0.9.1/betfair_parser/spec/streaming/enums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/streaming/messages.py` & `betfair_parser-0.9.1/betfair_parser/spec/streaming/messages.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/spec/streaming/type_definitions.py` & `betfair_parser-0.9.1/betfair_parser/spec/streaming/type_definitions.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/stream.py` & `betfair_parser-0.9.1/betfair_parser/stream.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/betfair_parser/strenums.py` & `betfair_parser-0.9.1/betfair_parser/strenums.py`

 * *Files identical despite different names*

### Comparing `betfair_parser-0.9.0/pyproject.toml` & `betfair_parser-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 [project.urls]
 Homepage = "https://github.com/limx0/betfair_parser"
 Documentation = "https://limx0.github.io/betfair_parser/"
 "Bug Tracker" = "https://github.com/limx0/betfair_parser/issues"
 
 [tool.poetry]
 name = "betfair_parser"
-version = "0.9.0"
+version = "0.9.1"
 description = "A betfair parser"
 readme = "README.md"
 authors = ["Bradley McElroy <bradley.mcelroy@live.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 msgspec = ">=0.18"
```

### Comparing `betfair_parser-0.9.0/PKG-INFO` & `betfair_parser-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betfair_parser
-Version: 0.9.0
+Version: 0.9.1
 Summary: A betfair parser
 Author: Bradley McElroy
 Author-email: bradley.mcelroy@live.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

