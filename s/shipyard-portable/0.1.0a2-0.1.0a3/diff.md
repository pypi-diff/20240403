# Comparing `tmp/shipyard_portable-0.1.0a2.tar.gz` & `tmp/shipyard_portable-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_portable-0.1.0a2.tar", max compression
+gzip compressed data, was "shipyard_portable-0.1.0a3.tar", max compression
```

## Comparing `shipyard_portable-0.1.0a2.tar` & `shipyard_portable-0.1.0a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a2/README.md
--rw-r--r--   0        0        0      436 2024-04-03 14:38:38.807423 shipyard_portable-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a2/shipyard_portable/__init__.py
--rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a2/shipyard_portable/cli/authtest.py
--rw-r--r--   0        0        0     2227 2024-04-03 14:43:11.258898 shipyard_portable-0.1.0a2/shipyard_portable/cli/trigger.py
--rw-r--r--   0        0        0     5750 2024-04-03 14:29:15.588987 shipyard_portable-0.1.0a2/shipyard_portable/portable.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a3/README.md
+-rw-r--r--   0        0        0      436 2024-04-03 15:34:58.699308 shipyard_portable-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a3/shipyard_portable/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a3/shipyard_portable/cli/authtest.py
+-rw-r--r--   0        0        0     2227 2024-04-03 14:43:11.258898 shipyard_portable-0.1.0a3/shipyard_portable/cli/trigger.py
+-rw-r--r--   0        0        0     5929 2024-04-03 15:34:50.002848 shipyard_portable-0.1.0a3/shipyard_portable/portable.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a3/PKG-INFO
```

### Comparing `shipyard_portable-0.1.0a2/shipyard_portable/cli/trigger.py` & `shipyard_portable-0.1.0a3/shipyard_portable/cli/trigger.py`

 * *Files identical despite different names*

### Comparing `shipyard_portable-0.1.0a2/shipyard_portable/portable.py` & `shipyard_portable-0.1.0a3/shipyard_portable/portable.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,21 @@
 
         except Exception as e:
             if response.status_code == 401:
                 raise UnauthorizedError(response.text)
 
             elif response.status_code == 400:
                 raise BadRequestError(response.text)
+            elif response.status_code == 404:
+                raise ExitCodeException(f"Failed to trigger sync for flow {flow_id}. Flow not found", self.EXIT_CODE_BAD_REQUEST)
+
             else:
                 logger.debug(f"Status code {response.status_code}")
                 raise ExitCodeException(
-                    f"Failed to trigger sync for flow {flow_id} due to an expected error. Message from the API: {response.text}",
+                    f"Failed to trigger sync for flow {flow_id} due to an unexpected error. Message from the API: {response.text}",
                     self.EXIT_CODE_UNKNOWN_ERROR,
                 )
         else:
             return response.json()
 
     def get_sync_status(self, flow_id: str) -> Dict[str, str]:
         """
```

### Comparing `shipyard_portable-0.1.0a2/PKG-INFO` & `shipyard_portable-0.1.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-portable
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

