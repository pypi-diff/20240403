# Comparing `tmp/workos-4.1.0.tar.gz` & `tmp/workos-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.1.0.tar", last modified: Tue Apr  2 23:20:33 2024, max compression
+gzip compressed data, was "workos-4.2.0.tar", last modified: Wed Apr  3 20:47:43 2024, max compression
```

## Comparing `workos-4.1.0.tar` & `workos-4.2.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 23:20:25.000000 workos-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-02 23:20:33.309790 workos-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-02 23:20:25.000000 workos-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:20:33.309790 workos-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-02 23:20:25.000000 workos-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.305790 workos-4.1.0/workos/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 23:20:25.000000 workos-4.1.0/workos/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 23:20:25.000000 workos-4.1.0/workos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-02 23:20:25.000000 workos-4.1.0/workos/audit_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-02 23:20:25.000000 workos-4.1.0/workos/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-02 23:20:25.000000 workos-4.1.0/workos/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 23:20:25.000000 workos-4.1.0/workos/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-02 23:20:25.000000 workos-4.1.0/workos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-02 23:20:25.000000 workos-4.1.0/workos/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-02 23:20:25.000000 workos-4.1.0/workos/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 23:20:25.000000 workos-4.1.0/workos/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 23:20:25.000000 workos-4.1.0/workos/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/audit_logs_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/directory_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/event.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/event_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/passwordless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-02 23:20:25.000000 workos-4.1.0/workos/sso.py
--rw-r--r--   0 runner    (1001) docker     (127)    38748 2024-04-02 23:20:25.000000 workos-4.1.0/workos/user_management.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/connection_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/pagination_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/sso_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/um_provider_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-02 23:20:25.000000 workos-4.1.0/workos/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:20:31.000000 workos-4.1.0/workos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 20:47:35.000000 workos-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 20:47:43.169553 workos-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-03 20:47:35.000000 workos-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:47:43.169553 workos-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 20:47:35.000000 workos-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.165553 workos-4.2.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 20:47:35.000000 workos-4.2.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 20:47:35.000000 workos-4.2.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-03 20:47:35.000000 workos-4.2.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 20:47:35.000000 workos-4.2.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-03 20:47:35.000000 workos-4.2.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 20:47:35.000000 workos-4.2.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 20:47:35.000000 workos-4.2.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-03 20:47:35.000000 workos-4.2.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-03 20:47:35.000000 workos-4.2.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-03 20:47:35.000000 workos-4.2.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-03 20:47:35.000000 workos-4.2.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-03 20:47:35.000000 workos-4.2.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-03 20:47:35.000000 workos-4.2.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38748 2024-04-03 20:47:35.000000 workos-4.2.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 20:47:35.000000 workos-4.2.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-03 20:47:35.000000 workos-4.2.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:43.169553 workos-4.2.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:41.000000 workos-4.2.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 20:47:43.000000 workos-4.2.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.1.0/LICENSE` & `workos-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/PKG-INFO` & `workos-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.1.0
+Version: 4.2.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.1.0/README.md` & `workos-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/setup.py` & `workos-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/audit_logs.py` & `workos-4.2.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/client.py` & `workos-4.2.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/directory_sync.py` & `workos-4.2.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/events.py` & `workos-4.2.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/exceptions.py` & `workos-4.2.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/mfa.py` & `workos-4.2.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/organizations.py` & `workos-4.2.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/passwordless.py` & `workos-4.2.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/portal.py` & `workos-4.2.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/audit_logs_export.py` & `workos-4.2.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/base.py` & `workos-4.2.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/directory_sync.py` & `workos-4.2.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/event.py` & `workos-4.2.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/list.py` & `workos-4.2.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/mfa.py` & `workos-4.2.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/organizations.py` & `workos-4.2.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/passwordless.py` & `workos-4.2.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/sso.py` & `workos-4.2.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/resources/user_management.py` & `workos-4.2.0/workos/resources/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/sso.py` & `workos-4.2.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/user_management.py` & `workos-4.2.0/workos/user_management.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/utils/connection_types.py` & `workos-4.2.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/utils/request.py` & `workos-4.2.0/workos/utils/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 REQUEST_METHOD_POST = "post"
 REQUEST_METHOD_PUT = "put"
 
 
 class RequestHelper(object):
     def __init__(self):
         self.set_base_api_url(workos.base_api_url)
+        self.set_request_timeout(workos.request_timeout)
+
+    def set_request_timeout(self, request_timeout):
+        self.request_timeout = request_timeout
 
     def set_base_api_url(self, base_api_url):
         """Creates an accessible template for constructing the URL for an API request.
 
         Args:
             base_api_url (str): Base URL for api requests (Should end with a /)
         """
@@ -69,17 +73,21 @@
             headers["Authorization"] = "Bearer {}".format(token)
 
         headers.update(BASE_HEADERS)
         url = self.generate_api_url(path)
 
         request_fn = getattr(requests, method)
         if method == REQUEST_METHOD_GET:
-            response = request_fn(url, headers=headers, params=params)
+            response = request_fn(
+                url, headers=headers, params=params, timeout=self.request_timeout
+            )
         else:
-            response = request_fn(url, headers=headers, json=params)
+            response = request_fn(
+                url, headers=headers, json=params, timeout=self.request_timeout
+            )
 
         response_json = None
         content_type = (
             response.headers.get("content-type")
             if response.headers is not None
             else None
         )
@@ -95,12 +103,14 @@
                 raise AuthenticationException(response)
             elif status_code == 403:
                 raise AuthorizationException(response)
             elif status_code == 404:
                 raise NotFoundException(response)
             error = response_json.get("error")
             error_description = response_json.get("error_description")
-            raise BadRequestException(response)
+            raise BadRequestException(
+                response, error=error, error_description=error_description
+            )
         elif status_code >= 500 and status_code < 600:
             raise ServerException(response)
 
         return response_json
```

### Comparing `workos-4.1.0/workos/utils/validation.py` & `workos-4.2.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos/webhooks.py` & `workos-4.2.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.1.0/workos.egg-info/PKG-INFO` & `workos-4.2.0/workos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.1.0
+Version: 4.2.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `workos-4.1.0/workos.egg-info/SOURCES.txt` & `workos-4.2.0/workos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

