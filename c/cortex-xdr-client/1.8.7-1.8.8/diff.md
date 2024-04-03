# Comparing `tmp/cortex_xdr_client-1.8.7.tar.gz` & `tmp/cortex_xdr_client-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cortex_xdr_client-1.8.7.tar", max compression
+gzip compressed data, was "cortex_xdr_client-1.8.8.tar", max compression
```

## Comparing `cortex_xdr_client-1.8.7.tar` & `cortex_xdr_client-1.8.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1072 2023-08-08 18:00:11.998844 cortex_xdr_client-1.8.7/LICENSE
--rw-r--r--   0        0        0     3059 2023-08-08 18:00:11.998844 cortex_xdr_client-1.8.7/README.rst
--rw-r--r--   0        0        0       61 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/__init__.py
--rw-r--r--   0        0        0        0 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/__init__.py
--rw-r--r--   0        0        0     2059 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/actions_api.py
--rw-r--r--   0        0        0     3387 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/alerts_api.py
--rw-r--r--   0        0        0     1544 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/authentication.py
--rw-r--r--   0        0        0     2376 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/base_api.py
--rw-r--r--   0        0        0      890 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/download_api.py
--rw-r--r--   0        0        0    15782 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/endpoints_api.py
--rw-r--r--   0        0        0     5261 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/incidents_api.py
--rw-r--r--   0        0        0     1175 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/ioc_api.py
--rw-r--r--   0        0        0        0 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/__init__.py
--rw-r--r--   0        0        0      390 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/action_status.py
--rw-r--r--   0        0        0     5902 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/alerts.py
--rw-r--r--   0        0        0     2716 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/endpoints.py
--rw-r--r--   0        0        0      692 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/exceptions.py
--rw-r--r--   0        0        0     2835 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/filters.py
--rw-r--r--   0        0        0     7770 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/incidents.py
--rw-r--r--   0        0        0     2617 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/ioc.py
--rw-r--r--   0        0        0     2392 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/scripts.py
--rw-r--r--   0        0        0    12326 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/scripts_api.py
--rw-r--r--   0        0        0     5414 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/api/xql_api.py
--rw-r--r--   0        0        0     2497 2023-08-08 18:00:12.002844 cortex_xdr_client-1.8.7/cortex_xdr_client/client.py
--rw-r--r--   0        0        0      646 2023-08-08 18:00:34.863235 cortex_xdr_client-1.8.7/pyproject.toml
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/LICENSE
+-rw-r--r--   0        0        0     3175 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/README.rst
+-rw-r--r--   0        0        0       61 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/__init__.py
+-rw-r--r--   0        0        0     2059 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/actions_api.py
+-rw-r--r--   0        0        0     3387 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/alerts_api.py
+-rw-r--r--   0        0        0     1544 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/authentication.py
+-rw-r--r--   0        0        0     2376 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/base_api.py
+-rw-r--r--   0        0        0      890 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/download_api.py
+-rw-r--r--   0        0        0    18253 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/endpoints_api.py
+-rw-r--r--   0        0        0     5261 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/incidents_api.py
+-rw-r--r--   0        0        0     1175 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/ioc_api.py
+-rw-r--r--   0        0        0        0 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/__init__.py
+-rw-r--r--   0        0        0      390 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/action_status.py
+-rw-r--r--   0        0        0     5902 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/alerts.py
+-rw-r--r--   0        0        0     2775 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/endpoints.py
+-rw-r--r--   0        0        0      692 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/exceptions.py
+-rw-r--r--   0        0        0     2835 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/filters.py
+-rw-r--r--   0        0        0     7770 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/incidents.py
+-rw-r--r--   0        0        0     2617 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/ioc.py
+-rw-r--r--   0        0        0     2392 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/scripts.py
+-rw-r--r--   0        0        0    12326 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/scripts_api.py
+-rw-r--r--   0        0        0     5414 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/api/xql_api.py
+-rw-r--r--   0        0        0     2497 2024-04-03 10:21:50.021368 cortex_xdr_client-1.8.8/cortex_xdr_client/client.py
+-rw-r--r--   0        0        0      646 2024-04-03 10:22:05.361466 cortex_xdr_client-1.8.8/pyproject.toml
+-rw-r--r--   0        0        0     3933 1970-01-01 00:00:00.000000 cortex_xdr_client-1.8.8/PKG-INFO
```

### Comparing `cortex_xdr_client-1.8.7/LICENSE` & `cortex_xdr_client-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/README.rst` & `cortex_xdr_client-1.8.8/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 *Endpoints API:*
 
 -  `Get All Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/89535019b740f-get-all-endpoints>`__
 -  `Get Endpoint <https://cortex-panw.stoplight.io/docs/cortex-xdr/b149d40bd4c51-get-endpoint>`__
 -  `Isolate Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/9c730a966cdd8-isolate-endpoints>`__
 -  `Unisolate Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/c719336adb46b-unisolate-endpoints>`__
 -  `Scan Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/2e666ee0be1c6-scan-endpoints>`__
+-  `Set an Endpoint Alias <https://cortex-panw.stoplight.io/docs/cortex-xdr/c1ff89fa71c74-set-an-endpoint-alias>`__
 -  `Retrieve File <https://cortex-panw.stoplight.io/docs/cortex-xdr/08b1ba9fcfae0-retrieve-file>`__
 -  `Quarantine File <https://cortex-panw.stoplight.io/docs/cortex-xdr/76e8cca7fcb2e-quarantine-files>`__
 
 
 *Incidents API:*
 
 -  `Get Incidents <https://cortex-panw.stoplight.io/docs/cortex-xdr/a61eadc13dd54-get-all-incidents>`__
```

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/actions_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/actions_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/alerts_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/authentication.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/authentication.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/base_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/base_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/download_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/download_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/endpoints_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/endpoints_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from cortex_xdr_client.api.base_api import BaseAPI
 from cortex_xdr_client.api.models.endpoints import (EndpointPlatform,
                                                     EndpointStatus,
                                                     GetAllEndpointsResponse,
                                                     GetEndpointResponse,
                                                     IsolateStatus,
                                                     ResponseActionResponse,
+                                                    ResponseStatusResponse,
                                                     ScanStatus,
                                                     )
 from cortex_xdr_client.api.models.filters import (new_request_data, request_filter, request_gte_lte_filter)
 
 
 class EndpointsAPI(BaseAPI):
     def __init__(self, auth: Authentication, fqdn: str, timeout: Tuple[int, int]) -> None:
@@ -216,14 +217,60 @@
 
         request_data = new_request_data(filters=filters)
 
         response = self._call(call_name="scan",
                               json_value=request_data)
         return ResponseActionResponse.parse_obj(response.json())
 
+    # https://docs-cortex.paloaltonetworks.com/r/Cortex-XDR-REST-API/Set-an-Endpoint-Alias
+    def set_endpoint_alias(self,
+                           new_alias: str,
+                           endpoint_id_list: List[str] = None,
+                           endpoint_status: EndpointStatus = None,
+                           dist_name: str = None,
+                           ip_list: List[str] = None,
+                           group_name: List[str] = None,
+                           platform: List[EndpointPlatform] = None,
+                           alias: List[str] = None,
+                           isolate: List[IsolateStatus] = None,
+                           hostname: List[str] = None,
+                           ) -> Optional[ResponseStatusResponse]:
+        """
+        Set or modify an Alias field for your endpoints.
+
+        :param new_alias: The alias name you want to set or modify.
+        :param endpoint_id_list: List of endpoint IDs.
+        :param endpoint_status: Status of the endpoint ID.
+        :param dist_name: Distribution / Installation Package name.
+        :param ip_list: List of IP addresses.
+        :param group_name: Group name the agent belongs to.
+        :param platform: Platform name.
+        :param alias: Alias name.
+        :param isolate: If the endpoint was isolated.
+        :param hostname: Hostname
+        :return: A ResponseStatusResponse if successful.
+        """
+        filters = self._get_common_endpoint_filters(endpoint_id_list=endpoint_id_list,
+                                                    dist_name=dist_name,
+                                                    ip_list=ip_list,
+                                                    group_name=group_name,
+                                                    platform=platform,
+                                                    alias=alias,
+                                                    isolate=isolate,
+                                                    hostname=hostname)
+        if endpoint_status is not None:
+            filters.append(request_filter("endpoint_status", "in", endpoint_status))
+
+        request_data = new_request_data(filters=filters, other={"alias": new_alias})
+
+        response = self._call(call_name="update_agent_name",
+                              json_value=request_data)
+
+        return ResponseStatusResponse.parse_obj(response.json())
+
     # https://docs.paloaltonetworks.com/cortex/cortex-xdr/cortex-xdr-api/cortex-xdr-apis/response-actions/retrieve-file.html
     def retrieve_file(self,
                       endpoint_id_list: List[str] = None,
                       files: Dict[str, List[str]] = None,
                       incident_id: str = None,
                       ) -> Optional[ResponseActionResponse]:
         """
```

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/incidents_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/incidents_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/ioc_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/ioc_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/alerts.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/alerts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/endpoints.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,7 +104,11 @@
     action_id: Optional[str]
     status: Optional[int]
     endpoints_count: Optional[int]
 
 
 class ResponseActionResponse(BaseModel):
     reply: ResponseActionResponseItem
+
+
+class ResponseStatusResponse(BaseModel):
+    reply: bool
```

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/exceptions.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/filters.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/filters.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/incidents.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/incidents.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/ioc.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/ioc.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/models/scripts.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/models/scripts.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/scripts_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/scripts_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/api/xql_api.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/api/xql_api.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/cortex_xdr_client/client.py` & `cortex_xdr_client-1.8.8/cortex_xdr_client/client.py`

 * *Files identical despite different names*

### Comparing `cortex_xdr_client-1.8.7/pyproject.toml` & `cortex_xdr_client-1.8.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "cortex-xdr-client"
 packages= [
     { include = "cortex_xdr_client", from="." },
 ]
-version = "v1.8.7"
+version = "v1.8.8"
 description = "API client for Cortex XDR Prevent"
 authors = ["ebarti"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/ebarti/cortex-xdr-client"
 repository = "https://github.com/ebarti/cortex-xdr-client"
```

### Comparing `cortex_xdr_client-1.8.7/PKG-INFO` & `cortex_xdr_client-1.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cortex-xdr-client
-Version: 1.8.7
+Version: 1.8.8
 Summary: API client for Cortex XDR Prevent
 Home-page: https://github.com/ebarti/cortex-xdr-client
 License: MIT
 Author: ebarti
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Project-URL: Repository, https://github.com/ebarti/cortex-xdr-client
 Description-Content-Type: text/x-rst
 
 About the cortex-xdr-client
 ###########################
@@ -38,14 +39,15 @@
 *Endpoints API:*
 
 -  `Get All Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/89535019b740f-get-all-endpoints>`__
 -  `Get Endpoint <https://cortex-panw.stoplight.io/docs/cortex-xdr/b149d40bd4c51-get-endpoint>`__
 -  `Isolate Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/9c730a966cdd8-isolate-endpoints>`__
 -  `Unisolate Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/c719336adb46b-unisolate-endpoints>`__
 -  `Scan Endpoints <https://cortex-panw.stoplight.io/docs/cortex-xdr/2e666ee0be1c6-scan-endpoints>`__
+-  `Set an Endpoint Alias <https://cortex-panw.stoplight.io/docs/cortex-xdr/c1ff89fa71c74-set-an-endpoint-alias>`__
 -  `Retrieve File <https://cortex-panw.stoplight.io/docs/cortex-xdr/08b1ba9fcfae0-retrieve-file>`__
 -  `Quarantine File <https://cortex-panw.stoplight.io/docs/cortex-xdr/76e8cca7fcb2e-quarantine-files>`__
 
 
 *Incidents API:*
 
 -  `Get Incidents <https://cortex-panw.stoplight.io/docs/cortex-xdr/a61eadc13dd54-get-all-incidents>`__
```

