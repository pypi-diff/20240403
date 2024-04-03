# Comparing `tmp/vy_lambda_tools-0.3.0.tar.gz` & `tmp/vy_lambda_tools-0.4.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vy_lambda_tools-0.3.0.tar", max compression
+gzip compressed data, was "vy_lambda_tools-0.4.0b0.tar", max compression
```

## Comparing `vy_lambda_tools-0.3.0.tar` & `vy_lambda_tools-0.4.0b0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0       88 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/README.adoc
--rw-r--r--   0        0        0      605 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/__init__.py
--rw-r--r--   0        0        0      904 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/configuration.py
--rw-r--r--   0        0        0      217 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/feature_flag/__init__.py
--rw-r--r--   0        0        0     1988 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/feature_flag/base.py
--rw-r--r--   0        0        0     3088 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/feature_flag/providers.py
--rw-r--r--   0        0        0      312 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/__init__.py
--rw-r--r--   0        0        0     3990 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/api_gateway.py
--rw-r--r--   0        0        0     1205 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/dynamodb.py
--rw-r--r--   0        0        0      857 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/handler.py
--rw-r--r--   0        0        0     2850 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/sqs.py
--rw-r--r--   0        0        0     2360 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/instrumentation.py
--rw-r--r--   0        0        0        0 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/py.typed
--rw-r--r--   0        0        0     3939 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/test_helpers.py
--rw-r--r--   0        0        0      421 2024-03-27 08:23:09.000000 vy_lambda_tools-0.3.0/vy_lambda_tools/types.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 vy_lambda_tools-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       88 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/README.adoc
+-rw-r--r--   0        0        0      607 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/configuration.py
+-rw-r--r--   0        0        0      217 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/feature_flag/__init__.py
+-rw-r--r--   0        0        0     1988 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/feature_flag/base.py
+-rw-r--r--   0        0        0     3088 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/feature_flag/providers.py
+-rw-r--r--   0        0        0      312 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/__init__.py
+-rw-r--r--   0        0        0     3990 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/api_gateway.py
+-rw-r--r--   0        0        0     1205 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/dynamodb.py
+-rw-r--r--   0        0        0      857 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/handler.py
+-rw-r--r--   0        0        0     2850 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/sqs.py
+-rw-r--r--   0        0        0     2360 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/instrumentation.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/py.typed
+-rw-r--r--   0        0        0     7217 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/routing.py
+-rw-r--r--   0        0        0     4476 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/test_helpers.py
+-rw-r--r--   0        0        0      421 2024-04-03 12:29:18.000000 vy_lambda_tools-0.4.0b0/vy_lambda_tools/types.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 vy_lambda_tools-0.4.0b0/PKG-INFO
```

### Comparing `vy_lambda_tools-0.3.0/pyproject.toml` & `vy_lambda_tools-0.4.0b0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vy-lambda-tools"
-version = "0.3.0"
+version = "0.4.0b0"
 description = ""
 authors = ["Nicolas Harlem Eide <nicolas@harlemeide.net>"]
 readme = "README.adoc"
 packages = [{include = "vy_lambda_tools"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/configuration.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/configuration.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/feature_flag/base.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/feature_flag/base.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/feature_flag/providers.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/feature_flag/providers.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/api_gateway.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/api_gateway.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/dynamodb.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/dynamodb.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/handler.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/handlers/sqs.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/handlers/sqs.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/instrumentation.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/instrumentation.py`

 * *Files identical despite different names*

### Comparing `vy_lambda_tools-0.3.0/vy_lambda_tools/test_helpers.py` & `vy_lambda_tools-0.4.0b0/vy_lambda_tools/test_helpers.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,22 +39,25 @@
     metadata: Optional[dict[str, Any]] = None,
 ) -> dict[str, Any]:
     if metadata is None:
         metadata = {}
     return {
         "Records": [
             {
+                "eventSource": "aws:sqs",
                 "messageId": md5(json.dumps(body).encode()),
                 "body": json.dumps(envelope(body, metadata)),
             }
         ]
     }
 
 
 def generate_api_gateway_event(
+    resource: Optional[str] = None,
+    method: Optional[str] = None,
     body: Optional[Union[dict[str, Any], str]] = None,
     path_parameters: Optional[dict[str, str]] = None,
     query_parameters: Optional[dict[str, str]] = None,
     caller_account_id: Optional[str] = None,
     jwt_claims: Optional[dict[str, Any]] = None,
     jwt_scopes: Optional[list[str]] = None,
     headers: Optional[dict[str, str]] = None,
@@ -65,25 +68,29 @@
         body = ""
     elif "application/x-www-form-urlencoded" not in headers.get("Content-Type", ""):
         try:
             body = json.dumps(body)
         except json.JSONDecodeError:
             body = body
 
-    return {
+    event = {
+        "resource": resource,
+        "httpMethod": method,
         "body": body,
         "pathParameters": path_parameters,
         "queryStringParameters": query_parameters,
         "requestContext": {
             "identity": {"accountId": caller_account_id},
             "authorizer": {"claims": jwt_claims, "scopes": jwt_scopes},
         },
         "headers": headers,
     }
 
+    return event
+
 
 def generate_api_gateway_event_without_jwt(
     body: Optional[Union[dict[str, Any], str]] = None,
     path_parameters: Optional[dict[str, str]] = None,
     caller_account_id: Optional[str] = None,
     headers: Optional[dict[str, str]] = None,
 ) -> dict[str, Any]:
@@ -103,29 +110,42 @@
         "requestContext": {
             "identity": {"accountId": caller_account_id},
         },
         "headers": headers,
     }
 
 
-def generate_dynamodb_event(old_value: Optional[dict[str, Any]]) -> dict[str, Any]:
+def generate_dynamodb_event(
+    old_value: Optional[dict[str, Any]],
+    table_name: str,
+    aws_region: str = "eu-west-1",
+    aws_account_id: str = "123456789012",
+) -> dict[str, Any]:
     ts = TypeSerializer()
+
+    stream_arn = (
+        f"arn:aws:dynamodb:{aws_region}:{aws_account_id}"
+        f":table/{table_name}/stream/2024-12-01T00:00:00.000"
+    )
+
     return {
         "Records": [
             {
+                "eventSource": "aws:dynamodb",
+                "eventSourceARN": stream_arn,
                 "dynamodb": {
                     # We don't care about the sequence number, but it is needed
                     "SequenceNumber": md5(str(datetime.now()).encode()),
                     "OldImage": {
                         key: ts.serialize(
                             value
                             if not isinstance(value, datetime)
                             else int(value.timestamp())
                         )
                         for key, value in old_value.items()
                     }
                     if old_value is not None
                     else {},
-                }
+                },
             }
         ]
     }
```

### Comparing `vy_lambda_tools-0.3.0/PKG-INFO` & `vy_lambda_tools-0.4.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vy-lambda-tools
-Version: 0.3.0
+Version: 0.4.0b0
 Summary: 
 Author: Nicolas Harlem Eide
 Author-email: nicolas@harlemeide.net
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

