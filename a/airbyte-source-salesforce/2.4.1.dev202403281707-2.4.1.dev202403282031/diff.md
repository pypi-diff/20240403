# Comparing `tmp/airbyte_source_salesforce-2.4.1.dev202403281707.tar.gz` & `tmp/airbyte_source_salesforce-2.4.1.dev202403282031.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_salesforce-2.4.1.dev202403281707.tar", max compression
+gzip compressed data, was "airbyte_source_salesforce-2.4.1.dev202403282031.tar", max compression
```

## Comparing `airbyte_source_salesforce-2.4.1.dev202403281707.tar` & `airbyte_source_salesforce-2.4.1.dev202403282031.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4568 2024-03-28 17:04:38.859047 airbyte_source_salesforce-2.4.1.dev202403281707/README.md
--rw-r--r--   0        0        0      842 2024-03-28 17:07:15.472020 airbyte_source_salesforce-2.4.1.dev202403281707/pyproject.toml
--rw-r--r--   0        0        0      131 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/__init__.py
--rw-r--r--   0        0        0    16806 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/api.py
--rw-r--r--   0        0        0     1667 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/availability_strategy.py
--rw-r--r--   0        0        0      808 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/exceptions.py
--rw-r--r--   0        0        0     2919 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/rate_limiting.py
--rw-r--r--   0        0        0     1619 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/run.py
--rw-r--r--   0        0        0     9747 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/schemas/Describe.json
--rw-r--r--   0        0        0    14130 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/source.py
--rw-r--r--   0        0        0     4769 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/spec.yaml
--rw-r--r--   0        0        0    40453 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/streams.py
--rw-r--r--   0        0        0     1024 2024-03-28 17:04:38.863047 airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/utils.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.1.dev202403281707/PKG-INFO
+-rw-r--r--   0        0        0     4568 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/README.md
+-rw-r--r--   0        0        0      842 2024-03-28 20:31:15.005513 airbyte_source_salesforce-2.4.1.dev202403282031/pyproject.toml
+-rw-r--r--   0        0        0      131 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/__init__.py
+-rw-r--r--   0        0        0    16806 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/api.py
+-rw-r--r--   0        0        0     1667 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/availability_strategy.py
+-rw-r--r--   0        0        0      808 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/exceptions.py
+-rw-r--r--   0        0        0     3633 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/rate_limiting.py
+-rw-r--r--   0        0        0     1619 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/run.py
+-rw-r--r--   0        0        0     9747 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/schemas/Describe.json
+-rw-r--r--   0        0        0    14130 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/source.py
+-rw-r--r--   0        0        0     4769 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/spec.yaml
+-rw-r--r--   0        0        0    40453 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/streams.py
+-rw-r--r--   0        0        0     1024 2024-03-28 20:28:28.059880 airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/utils.py
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 airbyte_source_salesforce-2.4.1.dev202403282031/PKG-INFO
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/README.md` & `airbyte_source_salesforce-2.4.1.dev202403282031/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/pyproject.toml` & `airbyte_source_salesforce-2.4.1.dev202403282031/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.4.1.dev202403281707"
+version = "2.4.1.dev202403282031"
 name = "airbyte-source-salesforce"
 description = "Source implementation for Salesforce."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/api.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/api.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/availability_strategy.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/availability_strategy.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/exceptions.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/rate_limiting.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/rate_limiting.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,25 +22,37 @@
     # Without much more information, we will make it retryable hoping that performing the same request will work.
     exceptions.ChunkedEncodingError,
     # We've had examples where the response from Salesforce was not a JSON response. Those cases where error cases though. For example:
     # https://github.com/airbytehq/airbyte-internal-issues/issues/6855. We will assume that this is an edge issue and that retry should help
     exceptions.JSONDecodeError,
 )
 
+_RETRYABLE_400_STATUS_CODE = {
+    # Using debug mode and breakpointing on the issue, we were able to validate that there issues are retryable. We've also opened a case
+    # with Salesforce to try to understand what is causing that as the response does not have a body.
+    406,
+    # Most of the time, they don't have a body but there was one from the Salesforce Edge mentioning "We are setting things up. This process
+    # can take a few minutes. This page will auto-refresh when ready. If it takes too long, please contact support or visit our <a>status
+    # page</a> for more information." We therefore assume this is a transient error and will retry on it.
+    420,
+    codes.too_many_requests,
+}
+
+
 logger = logging.getLogger("airbyte")
 
 
 def default_backoff_handler(max_tries: int, backoff_method={"method": backoff.expo, "params": {"factor": 15}}, **kwargs):
     def log_retry_attempt(details):
         _, exc, _ = sys.exc_info()
         logger.info(str(exc))
         logger.info(f"Caught retryable error after {details['tries']} tries. Waiting {details['wait']} seconds then retrying...")
 
     def should_give_up(exc):
-        give_up = exc.response is not None and exc.response.status_code != codes.too_many_requests and 400 <= exc.response.status_code < 500
+        give_up = exc.response is not None and exc.response.status_code not in _RETRYABLE_400_STATUS_CODE and 400 <= exc.response.status_code < 500
 
         # Salesforce can return an error with a limit using a 403 code error.
         if exc.response is not None and exc.response.status_code == codes.forbidden:
             error_data = exc.response.json()[0]
             if error_data.get("errorCode", "") == "REQUEST_LIMIT_EXCEEDED":
                 give_up = True
```

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/run.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/run.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/schemas/Describe.json` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/schemas/Describe.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/source.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/spec.yaml` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/spec.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/streams.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/source_salesforce/utils.py` & `airbyte_source_salesforce-2.4.1.dev202403282031/source_salesforce/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_salesforce-2.4.1.dev202403281707/PKG-INFO` & `airbyte_source_salesforce-2.4.1.dev202403282031/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-salesforce
-Version: 2.4.1.dev202403281707
+Version: 2.4.1.dev202403282031
 Summary: Source implementation for Salesforce.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

