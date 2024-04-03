# Comparing `tmp/shipyard_portable-0.1.0a1.tar.gz` & `tmp/shipyard_portable-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_portable-0.1.0a1.tar", max compression
+gzip compressed data, was "shipyard_portable-0.1.0a2.tar", max compression
```

## Comparing `shipyard_portable-0.1.0a1.tar` & `shipyard_portable-0.1.0a2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a1/README.md
--rw-r--r--   0        0        0      436 2024-04-03 03:25:36.717283 shipyard_portable-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a1/shipyard_portable/__init__.py
--rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a1/shipyard_portable/cli/authtest.py
--rw-r--r--   0        0        0     2220 2024-04-03 03:25:25.814716 shipyard_portable-0.1.0a1/shipyard_portable/cli/trigger.py
--rw-r--r--   0        0        0     5700 2024-04-03 03:22:04.023388 shipyard_portable-0.1.0a1/shipyard_portable/portable.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a2/README.md
+-rw-r--r--   0        0        0      436 2024-04-03 14:38:38.807423 shipyard_portable-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a2/shipyard_portable/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a2/shipyard_portable/cli/authtest.py
+-rw-r--r--   0        0        0     2227 2024-04-03 14:43:11.258898 shipyard_portable-0.1.0a2/shipyard_portable/cli/trigger.py
+-rw-r--r--   0        0        0     5750 2024-04-03 14:29:15.588987 shipyard_portable-0.1.0a2/shipyard_portable/portable.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a2/PKG-INFO
```

### Comparing `shipyard_portable-0.1.0a1/shipyard_portable/cli/trigger.py` & `shipyard_portable-0.1.0a2/shipyard_portable/cli/trigger.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,23 +25,24 @@
 
 
 def main():
     try:
         args = get_args()
         flow_id = args.flow_id
         portable = PortableClient(args.access_token)
-        portable.connect()
         flow_response = portable.trigger_sync(args.flow_id)
 
         wait = shipyard.args.convert_to_boolean(args.wait_for_completion)
         flow_status = portable.get_sync_status(flow_id)
         flow_disposition = flow_status["disposition"]
         exit_code = portable.determine_sync_status(flow_status)
         if wait:
-            logger.info("The flow will be checked every 60 seconds until completion")
+            logger.info(
+                f"The flow will be checked every {INTERVAL} seconds until completion"
+            )
             while flow_disposition not in ("SUCCEEDED", "FAILED"):
                 flow_status = portable.get_sync_status(args.flow_id)
                 flow_disposition = flow_status["disposition"]
                 flow_lifecyle = flow_status["lifecycle"]
                 exit_code = portable.determine_sync_status(flow_status)
                 logger.info(
                     f"Current state of flow is {flow_lifecyle}, waiting for completion"
@@ -53,13 +54,13 @@
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"An unexpected error occurred: {e}")
         sys.exit(Etl.EXIT_CODE_UNKNOWN_ERROR)
     else:
-        Artifact("portable").responses.write_json("flow_response.json", flow_status)
+        Artifact("portable").responses.write_json("flow_response", flow_status)
         sys.exit(exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_portable-0.1.0a1/shipyard_portable/portable.py` & `shipyard_portable-0.1.0a2/shipyard_portable/portable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import requests
 from shipyard_templates import ShipyardLogger, ExitCodeException
 from shipyard_templates import Etl
+from shipyard_templates.etl import UnauthorizedError, BadRequestError
 from typing import Dict
 
 logger = ShipyardLogger.get_logger()
 
 
 class PortableClient(Etl):
     def __init__(self, access_token: str) -> None:
@@ -57,18 +58,18 @@
             response.raise_for_status()
 
             if response.status_code == 201:
                 logger.info(f"Successfully triggered sync for flow {flow_id}")
 
         except Exception as e:
             if response.status_code == 401:
-                raise self.UnauthorizedError(response.text)
+                raise UnauthorizedError(response.text)
 
             elif response.status_code == 400:
-                raise self.BadRequestError(response.text)
+                raise BadRequestError(response.text)
             else:
                 logger.debug(f"Status code {response.status_code}")
                 raise ExitCodeException(
                     f"Failed to trigger sync for flow {flow_id} due to an expected error. Message from the API: {response.text}",
                     self.EXIT_CODE_UNKNOWN_ERROR,
                 )
         else:
@@ -92,17 +93,17 @@
         try:
             response = requests.get(
                 f"{self.flow_url}/{flow_id}/status", headers=self.headers
             )
             response.raise_for_status()
         except Exception as e:
             if response.status_code == 401:
-                raise self.UnauthorizedError(response.text)
+                raise UnauthorizedError(response.text)
             elif response.status_code == 400:
-                raise self.BadRequestError(response.text)
+                raise BadRequestError(response.text)
             else:
                 logger.debug(f"Status code {response.status_code}")
                 raise ExitCodeException(
                     f"Failed to fetch status for flow {flow_id} due to an expected error. Message from the API: {response.text}",
                     self.EXIT_CODE_UNKNOWN_ERROR,
                 )
         else:
```

### Comparing `shipyard_portable-0.1.0a1/PKG-INFO` & `shipyard_portable-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: shipyard-portable
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: shipyard-bp-utils (>=1.2.0,<2.0.0)
-Requires-Dist: shipyard-templates (>=0.8.1a0,<0.9.0)
+Requires-Dist: shipyard-templates (>=0.8.1a1,<0.9.0)
 Description-Content-Type: text/markdown
```

