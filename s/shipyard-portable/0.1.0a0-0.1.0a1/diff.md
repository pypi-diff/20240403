# Comparing `tmp/shipyard_portable-0.1.0a0.tar.gz` & `tmp/shipyard_portable-0.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_portable-0.1.0a0.tar", max compression
+gzip compressed data, was "shipyard_portable-0.1.0a1.tar", max compression
```

## Comparing `shipyard_portable-0.1.0a0.tar` & `shipyard_portable-0.1.0a1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a0/README.md
--rw-r--r--   0        0        0      436 2024-04-03 03:08:51.351654 shipyard_portable-0.1.0a0/pyproject.toml
--rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a0/shipyard_portable/__init__.py
--rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a0/shipyard_portable/cli/authtest.py
--rw-r--r--   0        0        0     2244 2024-04-02 21:09:20.397029 shipyard_portable-0.1.0a0/shipyard_portable/cli/trigger.py
--rw-r--r--   0        0        0     5699 2024-04-03 02:57:58.757662 shipyard_portable-0.1.0a0/shipyard_portable/portable.py
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 15:03:42.247940 shipyard_portable-0.1.0a1/README.md
+-rw-r--r--   0        0        0      436 2024-04-03 03:25:36.717283 shipyard_portable-0.1.0a1/pyproject.toml
+-rw-r--r--   0        0        0       37 2024-04-02 16:20:17.198256 shipyard_portable-0.1.0a1/shipyard_portable/__init__.py
+-rw-r--r--   0        0        0      248 2024-04-02 20:49:57.732518 shipyard_portable-0.1.0a1/shipyard_portable/cli/authtest.py
+-rw-r--r--   0        0        0     2220 2024-04-03 03:25:25.814716 shipyard_portable-0.1.0a1/shipyard_portable/cli/trigger.py
+-rw-r--r--   0        0        0     5700 2024-04-03 03:22:04.023388 shipyard_portable-0.1.0a1/shipyard_portable/portable.py
+-rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 shipyard_portable-0.1.0a1/PKG-INFO
```

### Comparing `shipyard_portable-0.1.0a0/shipyard_portable/cli/trigger.py` & `shipyard_portable-0.1.0a1/shipyard_portable/cli/trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,34 +33,33 @@
         flow_response = portable.trigger_sync(args.flow_id)
 
         wait = shipyard.args.convert_to_boolean(args.wait_for_completion)
         flow_status = portable.get_sync_status(flow_id)
         flow_disposition = flow_status["disposition"]
         exit_code = portable.determine_sync_status(flow_status)
         if wait:
-            logger.info("Waiting for flow to complete")
+            logger.info("The flow will be checked every 60 seconds until completion")
             while flow_disposition not in ("SUCCEEDED", "FAILED"):
                 flow_status = portable.get_sync_status(args.flow_id)
                 flow_disposition = flow_status["disposition"]
                 flow_lifecyle = flow_status["lifecycle"]
                 exit_code = portable.determine_sync_status(flow_status)
                 logger.info(
-                    f"Flow has a status of {flow_lifecyle}, waiting for completion"
+                    f"Current state of flow is {flow_lifecyle}, waiting for completion"
                 )
                 time.sleep(INTERVAL)
 
         logger.info(f"Flow has a status of {flow_disposition}, exiting now")
 
     except ExitCodeException as ec:
         logger.error(ec.message)
         sys.exit(ec.exit_code)
     except Exception as e:
         logger.error(f"An unexpected error occurred: {e}")
         sys.exit(Etl.EXIT_CODE_UNKNOWN_ERROR)
     else:
-        logger.debug("Saving response data to artifacts")
         Artifact("portable").responses.write_json("flow_response.json", flow_status)
         sys.exit(exit_code)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `shipyard_portable-0.1.0a0/shipyard_portable/portable.py` & `shipyard_portable-0.1.0a1/shipyard_portable/portable.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             else:
                 logger.debug(f"Status code {response.status_code}")
                 raise ExitCodeException(
                     f"Failed to fetch status for flow {flow_id} due to an expected error. Message from the API: {response.text}",
                     self.EXIT_CODE_UNKNOWN_ERROR,
                 )
         else:
-            logger.info(f"Successfully fetched sync status")
+            logger.debug(f"Successfully fetched sync status")
             return response.json()
 
     def determine_sync_status(self, response_data: Dict[str, str]) -> int:
         """
         Determines the synchronization status based on the response data.
 
         Args:
```

### Comparing `shipyard_portable-0.1.0a0/PKG-INFO` & `shipyard_portable-0.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-portable
-Version: 0.1.0a0
+Version: 0.1.0a1
 Summary: 
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

