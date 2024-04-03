# Comparing `tmp/labkey-3.0.0.tar.gz` & `tmp/labkey-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labkey-3.0.0.tar", last modified: Tue Jan 30 22:06:43 2024, max compression
+gzip compressed data, was "labkey-3.1.0.tar", last modified: Wed Apr  3 21:05:54 2024, max compression
```

## Comparing `labkey-3.0.0.tar` & `labkey-3.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-01-30 22:06:43.527952 labkey-3.0.0/
--rw-r--r--   0 alan       (504) staff       (20)    10477 2024-01-30 21:40:23.000000 labkey-3.0.0/CHANGE.txt
--rw-r--r--   0 alan       (504) staff       (20)    11358 2024-01-02 22:01:26.000000 labkey-3.0.0/LICENSE.txt
--rw-r--r--   0 alan       (504) staff       (20)       62 2024-01-02 22:01:26.000000 labkey-3.0.0/MANIFEST.in
--rw-r--r--   0 alan       (504) staff       (20)     1072 2024-01-30 22:06:43.527845 labkey-3.0.0/PKG-INFO
--rw-r--r--   0 alan       (504) staff       (20)     5757 2024-01-30 21:40:23.000000 labkey-3.0.0/README.md
-drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-01-30 22:06:43.525641 labkey-3.0.0/labkey/
--rw-r--r--   0 alan       (504) staff       (20)      695 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/__init__.py
--rw-r--r--   0 alan       (504) staff       (20)     1351 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/api_wrapper.py
--rw-r--r--   0 alan       (504) staff       (20)     5497 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/container.py
--rw-r--r--   0 alan       (504) staff       (20)    22486 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/domain.py
--rw-r--r--   0 alan       (504) staff       (20)     2929 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/exceptions.py
--rw-r--r--   0 alan       (504) staff       (20)     8804 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/experiment.py
--rw-r--r--   0 alan       (504) staff       (20)    23995 2024-01-30 21:40:23.000000 labkey-3.0.0/labkey/query.py
--rw-r--r--   0 alan       (504) staff       (20)    15284 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/security.py
--rw-r--r--   0 alan       (504) staff       (20)     6950 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/server_context.py
--rw-r--r--   0 alan       (504) staff       (20)     6144 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/storage.py
--rw-r--r--   0 alan       (504) staff       (20)     3233 2024-01-02 22:01:26.000000 labkey-3.0.0/labkey/utils.py
-drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-01-30 22:06:43.527023 labkey-3.0.0/labkey.egg-info/
--rw-r--r--   0 alan       (504) staff       (20)     1072 2024-01-30 22:06:43.000000 labkey-3.0.0/labkey.egg-info/PKG-INFO
--rw-r--r--   0 alan       (504) staff       (20)      452 2024-01-30 22:06:43.000000 labkey-3.0.0/labkey.egg-info/SOURCES.txt
--rw-r--r--   0 alan       (504) staff       (20)        1 2024-01-30 22:06:43.000000 labkey-3.0.0/labkey.egg-info/dependency_links.txt
--rw-r--r--   0 alan       (504) staff       (20)       49 2024-01-30 22:06:43.000000 labkey-3.0.0/labkey.egg-info/requires.txt
--rw-r--r--   0 alan       (504) staff       (20)        7 2024-01-30 22:06:43.000000 labkey-3.0.0/labkey.egg-info/top_level.txt
--rw-r--r--   0 alan       (504) staff       (20)       31 2024-01-02 22:01:26.000000 labkey-3.0.0/pyproject.toml
--rw-r--r--   0 alan       (504) staff       (20)      161 2024-01-02 22:01:26.000000 labkey-3.0.0/pytest.ini
--rw-r--r--   0 alan       (504) staff       (20)      193 2024-01-30 22:06:43.528367 labkey-3.0.0/setup.cfg
--rw-r--r--   0 alan       (504) staff       (20)     2249 2024-01-02 22:01:26.000000 labkey-3.0.0/setup.py
+drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-04-03 21:05:54.800325 labkey-3.1.0/
+-rw-r--r--   0 alan       (504) staff       (20)    10870 2024-04-03 21:05:46.000000 labkey-3.1.0/CHANGE.txt
+-rw-r--r--   0 alan       (504) staff       (20)    11358 2024-01-02 22:01:26.000000 labkey-3.1.0/LICENSE.txt
+-rw-r--r--   0 alan       (504) staff       (20)       62 2024-01-02 22:01:26.000000 labkey-3.1.0/MANIFEST.in
+-rw-r--r--   0 alan       (504) staff       (20)     1072 2024-04-03 21:05:54.800167 labkey-3.1.0/PKG-INFO
+-rw-r--r--   0 alan       (504) staff       (20)     5757 2024-01-30 21:40:23.000000 labkey-3.1.0/README.md
+drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-04-03 21:05:54.797478 labkey-3.1.0/labkey/
+-rw-r--r--   0 alan       (504) staff       (20)      695 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/__init__.py
+-rw-r--r--   0 alan       (504) staff       (20)     1427 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/api_wrapper.py
+-rw-r--r--   0 alan       (504) staff       (20)     5497 2024-01-02 22:01:26.000000 labkey-3.1.0/labkey/container.py
+-rw-r--r--   0 alan       (504) staff       (20)    22486 2024-01-02 22:01:26.000000 labkey-3.1.0/labkey/domain.py
+-rw-r--r--   0 alan       (504) staff       (20)     3619 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/exceptions.py
+-rw-r--r--   0 alan       (504) staff       (20)     8804 2024-01-02 22:01:26.000000 labkey-3.1.0/labkey/experiment.py
+-rw-r--r--   0 alan       (504) staff       (20)    24041 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/query.py
+-rw-r--r--   0 alan       (504) staff       (20)    15306 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/security.py
+-rw-r--r--   0 alan       (504) staff       (20)     7741 2024-04-03 21:05:46.000000 labkey-3.1.0/labkey/server_context.py
+-rw-r--r--   0 alan       (504) staff       (20)     6144 2024-01-02 22:01:26.000000 labkey-3.1.0/labkey/storage.py
+-rw-r--r--   0 alan       (504) staff       (20)     3233 2024-01-02 22:01:26.000000 labkey-3.1.0/labkey/utils.py
+drwxr-xr-x   0 alan       (504) staff       (20)        0 2024-04-03 21:05:54.799022 labkey-3.1.0/labkey.egg-info/
+-rw-r--r--   0 alan       (504) staff       (20)     1072 2024-04-03 21:05:54.000000 labkey-3.1.0/labkey.egg-info/PKG-INFO
+-rw-r--r--   0 alan       (504) staff       (20)      452 2024-04-03 21:05:54.000000 labkey-3.1.0/labkey.egg-info/SOURCES.txt
+-rw-r--r--   0 alan       (504) staff       (20)        1 2024-04-03 21:05:54.000000 labkey-3.1.0/labkey.egg-info/dependency_links.txt
+-rw-r--r--   0 alan       (504) staff       (20)       49 2024-04-03 21:05:54.000000 labkey-3.1.0/labkey.egg-info/requires.txt
+-rw-r--r--   0 alan       (504) staff       (20)        7 2024-04-03 21:05:54.000000 labkey-3.1.0/labkey.egg-info/top_level.txt
+-rw-r--r--   0 alan       (504) staff       (20)       31 2024-01-02 22:01:26.000000 labkey-3.1.0/pyproject.toml
+-rw-r--r--   0 alan       (504) staff       (20)      161 2024-01-02 22:01:26.000000 labkey-3.1.0/pytest.ini
+-rw-r--r--   0 alan       (504) staff       (20)      193 2024-04-03 21:05:54.800655 labkey-3.1.0/setup.cfg
+-rw-r--r--   0 alan       (504) staff       (20)     2249 2024-01-02 22:01:26.000000 labkey-3.1.0/setup.py
```

### Comparing `labkey-3.0.0/CHANGE.txt` & `labkey-3.1.0/CHANGE.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 +++++++++++
 LabKey Python Client API News
 +++++++++++
 
+What's New in the LabKey 3.1.0 package
+==============================
+
+*Release date: 04/03/2024*
+- ServerContext
+    - Add allow_redirects flag (defaults to False) to constructor
+    - Add allow_redirects flag to make_request
+- APIWrapper: Add allow_redirects flag (defaults to False)
+- Add UnexpectedRedirectError
+    - thrown when allow_redirects is False and the server issues a redirect
+
 What's New in the LabKey 3.0.0 package
 ==============================
 
 *Release date: 12/14/2023*
 - Query API - WAF encode "sql" parameter for execute_sql
     - WAF encoding of parameters is initially supported with LabKey Server v23.09
     - WAF encoding can be opted out of on execute_sql calls by specifying waf_encode_sql=False
```

### Comparing `labkey-3.0.0/LICENSE.txt` & `labkey-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/PKG-INFO` & `labkey-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labkey
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python client API for LabKey Server
 Home-page: https://github.com/LabKey/labkey-api-python
 Author: LabKey
 Author-email: alanv@labkey.com
 Maintainer: Alan Vezina
 Maintainer-email: alanv@labkey.com
 License: Apache License 2.0
```

### Comparing `labkey-3.0.0/README.md` & `labkey-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey/__init__.py` & `labkey-3.1.0/labkey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 __title__ = "labkey"
-__version__ = "3.0.0"
+__version__ = "3.1.0"
 __author__ = "LabKey"
 __license__ = "Apache License 2.0"
```

### Comparing `labkey-3.0.0/labkey/api_wrapper.py` & `labkey-3.1.0/labkey/api_wrapper.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,23 +18,25 @@
         domain,
         container_path,
         context_path=None,
         use_ssl=True,
         verify_ssl=True,
         api_key=None,
         disable_csrf=False,
+        allow_redirects=False,
     ):
         self.server_context = ServerContext(
             domain=domain,
             container_path=container_path,
             context_path=context_path,
             use_ssl=use_ssl,
             verify_ssl=verify_ssl,
             api_key=api_key,
             disable_csrf=disable_csrf,
+            allow_redirects=allow_redirects,
         )
         self.container = ContainerWrapper(self.server_context)
         self.domain = DomainWrapper(self.server_context)
         self.experiment = ExperimentWrapper(self.server_context)
         self.query = QueryWrapper(self.server_context)
         self.security = SecurityWrapper(self.server_context)
         self.storage = StorageWrapper(self.server_context)
```

### Comparing `labkey-3.0.0/labkey/container.py` & `labkey-3.1.0/labkey/container.py`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey/domain.py` & `labkey-3.1.0/labkey/domain.py`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey/exceptions.py` & `labkey-3.1.0/labkey/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -43,15 +43,30 @@
                 pass
 
             self.message = "{0}: {1}".format(self.response.status_code, msg)
         else:
             self.message = "No response received"
 
     def __str__(self):
-        return repr(self.message)
+        return str(self.message)
+
+
+class UnexpectedRedirectError(RequestError):
+    default_msg = "Unexpected redirect occurred"
+
+    def __init__(self, server_response, **kwargs):
+        super().__init__(server_response, **kwargs)
+
+        location = server_response.headers.get("Location", "")
+
+        # If the server is redirecting from http to https the user probably has a misconfigured ServerContext with use_ssl=False
+        if server_response.url.startswith("http://") and location.startswith("https://"):
+            self.message = "Redirected from http to https, set use_ssl=True in your APIWrapper or ServerContext"
+        elif location != "":
+            self.message = f"Unexpected redirect to: {location}"
 
 
 class QueryNotFoundError(RequestError):
     default_msg = "Query Resource Not Found"
 
 
 class RequestAuthorizationError(RequestError):
```

### Comparing `labkey-3.0.0/labkey/experiment.py` & `labkey-3.1.0/labkey/experiment.py`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey/query.py` & `labkey-3.1.0/labkey/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
     sort: str = None,
     offset: int = None,
     container_filter: str = None,
     save_in_session: bool = None,
     parameters: dict = None,
     required_version: float = None,
     timeout: int = _default_timeout,
-    waf_encode_sql: bool = True
+    waf_encode_sql: bool = True,
 ):
     """
     Execute sql query against a LabKey server.
 
     :param server_context: A LabKey server context. See utils.create_server_context.
     :param schema_name: schema of table
     :param sql: String of labkey sql to execute
@@ -531,15 +531,20 @@
     :param audit_behavior: used to override the audit behavior for the update. See class query.AuditBehavior
     :param audit_user_comment: used to provide a comment that will be attached to certain detailed audit log records
     :param timeout: timeout of request in seconds (defaults to 30s)
     :return:
     """
     url = server_context.build_url("query", "moveRows.api", container_path=container_path)
 
-    payload = {"targetContainerPath": target_container_path, "schemaName": schema_name, "queryName": query_name, "rows": rows}
+    payload = {
+        "targetContainerPath": target_container_path,
+        "schemaName": schema_name,
+        "queryName": query_name,
+        "rows": rows,
+    }
 
     if transacted is False:
         payload["transacted"] = transacted
 
     if audit_behavior is not None:
         payload["auditBehavior"] = audit_behavior
 
@@ -578,15 +583,15 @@
             schema_name,
             query_name,
             rows,
             container_path,
             transacted,
             audit_behavior,
             audit_user_comment,
-            timeout
+            timeout,
         )
 
     @functools.wraps(truncate_table)
     def truncate_table(
         self, schema_name, query_name, container_path=None, timeout=_default_timeout
     ):
         return truncate_table(self.server_context, schema_name, query_name, container_path, timeout)
@@ -601,30 +606,30 @@
         sort: str = None,
         offset: int = None,
         container_filter: str = None,
         save_in_session: bool = None,
         parameters: dict = None,
         required_version: float = None,
         timeout: int = _default_timeout,
-        waf_encode_sql: bool = True
+        waf_encode_sql: bool = True,
     ):
         return execute_sql(
             self.server_context,
             schema_name,
             sql,
             container_path,
             max_rows,
             sort,
             offset,
             container_filter,
             save_in_session,
             parameters,
             required_version,
             timeout,
-            waf_encode_sql
+            waf_encode_sql,
         )
 
     @functools.wraps(insert_rows)
     def insert_rows(
         self,
         schema_name: str,
         query_name: str,
@@ -642,15 +647,15 @@
             query_name,
             rows,
             container_path,
             skip_reselect_rows,
             transacted,
             audit_behavior,
             audit_user_comment,
-            timeout
+            timeout,
         )
 
     @functools.wraps(select_rows)
     def select_rows(
         self,
         schema_name: str,
         query_name: str,
@@ -712,15 +717,15 @@
             schema_name,
             query_name,
             rows,
             container_path,
             transacted,
             audit_behavior,
             audit_user_comment,
-            timeout
+            timeout,
         )
 
     @functools.wraps(move_rows)
     def move_rows(
         self,
         target_container_path: str,
         schema_name: str,
@@ -738,9 +743,9 @@
             schema_name,
             query_name,
             rows,
             container_path,
             transacted,
             audit_behavior,
             audit_user_comment,
-            timeout
+            timeout,
         )
```

### Comparing `labkey-3.0.0/labkey/security.py` & `labkey-3.1.0/labkey/security.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
 
 
 def stop_impersonating(server_context: ServerContext):
     """
     Stop impersonating a user while keeping the original user logged in.
     """
     url = server_context.build_url(LOGIN_CONTROLLER, "stopImpersonating.api")
-    return server_context.make_request(url)
+    return server_context.make_request(url, allow_redirects=True)
 
 
 @dataclass
 class WhoAmI:
     id: int
     email: str
     display_name: str
```

### Comparing `labkey-3.0.0/labkey/server_context.py` & `labkey-3.1.0/labkey/server_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from requests.exceptions import RequestException
 from labkey.exceptions import (
     RequestError,
     RequestAuthorizationError,
     QueryNotFoundError,
     ServerContextError,
     ServerNotFoundError,
+    UnexpectedRedirectError,
 )
 
 API_KEY_TOKEN = "apikey"
 CSRF_TOKEN = "X-LABKEY-CSRF"
 
 
 def handle_response(response, non_json_response=False):
@@ -25,15 +26,16 @@
         except ValueError:
             result = dict(
                 status_code=sc,
                 message="Request was successful but did not return valid json",
                 content=response.content,
             )
             return result
-
+    elif sc == 302:
+        raise UnexpectedRedirectError(response)
     elif sc == 401:
         raise RequestAuthorizationError(response)
     elif sc == 404:
         try:
             if non_json_response:
                 return response
             response.json()  # attempt to decode response
@@ -58,22 +60,24 @@
         domain,
         container_path,
         context_path=None,
         use_ssl=True,
         verify_ssl=True,
         api_key=None,
         disable_csrf=False,
+        allow_redirects=False,
     ):
         self._container_path = container_path
         self._context_path = context_path
         self._domain = domain
         self._use_ssl = use_ssl
         self._verify_ssl = verify_ssl
         self._api_key = api_key
         self._disable_csrf = disable_csrf
+        self.allow_redirects = allow_redirects
         self._session = requests.Session()
         self._session.headers.update({"User-Agent": f"LabKey Python API/{__version__}"})
 
         if self._use_ssl:
             self._scheme = "https://"
             if not self._verify_ssl:
                 self._session.verify = False
@@ -170,47 +174,66 @@
         payload: any = None,
         headers: dict = None,
         timeout: int = 300,
         method: str = "POST",
         non_json_response: bool = False,
         file_payload: any = None,
         json: dict = None,
+        allow_redirects=False,
     ) -> any:
+        allow_redirects_ = allow_redirects or self.allow_redirects
         if self._api_key is not None:
             if self._session.headers.get(API_KEY_TOKEN) is not self._api_key:
                 self._session.headers.update({API_KEY_TOKEN: self._api_key})
 
         if not self._disable_csrf and CSRF_TOKEN not in self._session.headers.keys():
             try:
                 csrf_url = self.build_url("login", "whoami.api")
                 response = handle_response(self._session.get(csrf_url))
                 self._session.headers.update({CSRF_TOKEN: response["CSRF"]})
             except RequestException as e:
                 self.handle_request_exception(e)
 
         try:
             if method == "GET":
-                response = self._session.get(url, params=payload, headers=headers, timeout=timeout)
+                response = self._session.get(
+                    url,
+                    params=payload,
+                    headers=headers,
+                    timeout=timeout,
+                    allow_redirects=allow_redirects_,
+                )
             else:
                 if file_payload is not None:
                     response = self._session.post(
                         url,
                         data=payload,
                         files=file_payload,
                         headers=headers,
                         timeout=timeout,
+                        allow_redirects=allow_redirects_,
                     )
                 elif json is not None:
                     if headers is None:
                         headers = {}
 
                     headers_ = {**headers, "Content-Type": "application/json"}
                     # sort_keys is a hack to make unit tests work
                     data = json_dumps(json, sort_keys=True)
-                    response = self._session.post(url, data=data, headers=headers_, timeout=timeout)
+                    response = self._session.post(
+                        url,
+                        data=data,
+                        headers=headers_,
+                        timeout=timeout,
+                        allow_redirects=allow_redirects_,
+                    )
                 else:
                     response = self._session.post(
-                        url, data=payload, headers=headers, timeout=timeout
+                        url,
+                        data=payload,
+                        headers=headers,
+                        timeout=timeout,
+                        allow_redirects=allow_redirects_,
                     )
             return handle_response(response, non_json_response)
         except RequestException as e:
             self.handle_request_exception(e)
```

### Comparing `labkey-3.0.0/labkey/storage.py` & `labkey-3.1.0/labkey/storage.py`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey/utils.py` & `labkey-3.1.0/labkey/utils.py`

 * *Files identical despite different names*

### Comparing `labkey-3.0.0/labkey.egg-info/PKG-INFO` & `labkey-3.1.0/labkey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labkey
-Version: 3.0.0
+Version: 3.1.0
 Summary: Python client API for LabKey Server
 Home-page: https://github.com/LabKey/labkey-api-python
 Author: LabKey
 Author-email: alanv@labkey.com
 Maintainer: Alan Vezina
 Maintainer-email: alanv@labkey.com
 License: Apache License 2.0
```

### Comparing `labkey-3.0.0/setup.py` & `labkey-3.1.0/setup.py`

 * *Files identical despite different names*

