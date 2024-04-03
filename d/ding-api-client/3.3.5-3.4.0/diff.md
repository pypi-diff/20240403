# Comparing `tmp/ding_api_client-3.3.5.tar.gz` & `tmp/ding_api_client-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ding_api_client-3.3.5.tar", last modified: Wed Mar 27 00:11:22 2024, max compression
+gzip compressed data, was "ding_api_client-3.4.0.tar", last modified: Wed Apr  3 00:11:57 2024, max compression
```

## Comparing `ding_api_client-3.3.5.tar` & `ding_api_client-3.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.496784 ding_api_client-3.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.496784 ding_api_client-3.3.5/src/ding/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.496784 ding_api_client-3.3.5/src/ding/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.496784 ding_api_client-3.3.5/src/ding/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/src/ding/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/createauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/createauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/createcheckrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/createcheckresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/feedbackrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/feedbackresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/lookupresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/retryauthenticationrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/retryauthenticationresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/components/security.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/src/ding/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/errors/errorresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/src/ding/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/check.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/create_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/models/operations/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    14780 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/otp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/src/ding/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-03-27 00:11:13.000000 ding_api_client-3.3.5/src/ding/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:11:22.500784 ding_api_client-3.3.5/src/ding_api_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-27 00:11:22.000000 ding_api_client-3.3.5/src/ding_api_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-27 00:11:22.000000 ding_api_client-3.3.5/src/ding_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:11:22.000000 ding_api_client-3.3.5/src/ding_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 00:11:22.000000 ding_api_client-3.3.5/src/ding_api_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-27 00:11:22.000000 ding_api_client-3.3.5/src/ding_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.745812 ding_api_client-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createcheckrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/createcheckresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/feedbackrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/feedbackresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/lookupresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/retryauthenticationrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/retryauthenticationresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/components/security.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.749812 ding_api_client-3.4.0/src/ding/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/errorresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/create_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/models/operations/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15282 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-03 00:11:46.000000 ding_api_client-3.4.0/src/ding/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:11:57.753812 ding_api_client-3.4.0/src/ding_api_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9342 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 00:11:57.000000 ding_api_client-3.4.0/src/ding_api_client.egg-info/top_level.txt
```

### Comparing `ding_api_client-3.3.5/PKG-INFO` & `ding_api_client-3.4.0/src/ding_api_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: ding_api_client
-Version: 3.3.5
+Name: ding-api-client
+Version: 3.4.0
 Summary: Python Client SDK
-Home-page: UNKNOWN
+Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
         
         <!-- Start SDK Installation [installation] -->
@@ -121,15 +121,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object         | Status Code          | Content Type         |
         | -------------------- | -------------------- | -------------------- |
         | errors.ErrorResponse | 400                  | application/json     |
-        | errors.SDKError      | 4x-5xx               | */*                  |
+        | errors.SDKError      | 4xx-5xx              | */*                  |
         
         ### Example
         
         ```python
         import ding
         from ding.models import components, errors
         
@@ -229,15 +229,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import ding
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = ding.Ding(client: http_client)
+        s = ding.Ding(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         <!-- Start Authentication [security] -->
         ## Authentication
         
         ### Per-Client Security Schemes
```

### Comparing `ding_api_client-3.3.5/README.md` & `ding_api_client-3.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object         | Status Code          | Content Type         |
 | -------------------- | -------------------- | -------------------- |
 | errors.ErrorResponse | 400                  | application/json     |
-| errors.SDKError      | 4x-5xx               | */*                  |
+| errors.SDKError      | 4xx-5xx              | */*                  |
 
 ### Example
 
 ```python
 import ding
 from ding.models import components, errors
 
@@ -222,15 +222,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import ding
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = ding.Ding(client: http_client)
+s = ding.Ding(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 <!-- Start Authentication [security] -->
 ## Authentication
 
 ### Per-Client Security Schemes
```

### Comparing `ding_api_client-3.3.5/setup.py` & `ding_api_client-3.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="ding_api_client",
-    version="3.3.5",
+    version="3.4.0",
     author="Ding",
     description="Python Client SDK",
+    url="https://github.com/ding-live/ding-python.git",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
```

### Comparing `ding_api_client-3.3.5/src/ding/_hooks/sdkhooks.py` & `ding_api_client-3.4.0/src/ding/_hooks/sdkhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -25,27 +25,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `ding_api_client-3.3.5/src/ding/_hooks/types.py` & `ding_api_client-3.4.0/src/ding/_hooks/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
```

### Comparing `ding_api_client-3.3.5/src/ding/lookup.py` & `ding_api_client-3.4.0/src/ding/lookup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from ding import utils
-from ding._hooks import HookContext
+from ding._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from ding.models import components, errors, operations
 from typing import Optional
 
 class Lookup:
     r"""Retrieve up-to-date metadata about a specific phone number"""
     sdk_configuration: SDKConfiguration
 
@@ -35,45 +35,44 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.LookupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.LookupResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.LookupResponse])
                 res.lookup_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `ding_api_client-3.3.5/src/ding/models/components/__init__.py` & `ding_api_client-3.4.0/src/ding/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/createauthenticationrequest.py` & `ding_api_client-3.4.0/src/ding/models/components/createauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/createauthenticationresponse.py` & `ding_api_client-3.4.0/src/ding/models/components/createauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/createcheckrequest.py` & `ding_api_client-3.4.0/src/ding/models/components/createcheckrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/createcheckresponse.py` & `ding_api_client-3.4.0/src/ding/models/components/createcheckresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/feedbackrequest.py` & `ding_api_client-3.4.0/src/ding/models/components/feedbackrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/feedbackresponse.py` & `ding_api_client-3.4.0/src/ding/models/components/feedbackresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/lookupresponse.py` & `ding_api_client-3.4.0/src/ding/models/components/lookupresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/retryauthenticationrequest.py` & `ding_api_client-3.4.0/src/ding/models/components/retryauthenticationrequest.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/components/retryauthenticationresponse.py` & `ding_api_client-3.4.0/src/ding/models/components/retryauthenticationresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/errors/errorresponse.py` & `ding_api_client-3.4.0/src/ding/models/errors/errorresponse.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/errors/sdkerror.py` & `ding_api_client-3.4.0/src/ding/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/operations/check.py` & `ding_api_client-3.4.0/src/ding/models/operations/check.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/operations/create_authentication.py` & `ding_api_client-3.4.0/src/ding/models/operations/create_authentication.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/operations/feedback.py` & `ding_api_client-3.4.0/src/ding/models/operations/feedback.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/operations/lookup.py` & `ding_api_client-3.4.0/src/ding/models/operations/lookup.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/models/operations/retry.py` & `ding_api_client-3.4.0/src/ding/models/operations/retry.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding/otp.py` & `ding_api_client-3.4.0/src/ding/otp.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from ding import utils
-from ding._hooks import HookContext
+from ding._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from ding.models import components, errors, operations
 from typing import Optional
 
 class Otp:
     r"""Send OTP codes to your users using their phone numbers."""
     sdk_configuration: SDKConfiguration
 
@@ -32,45 +32,44 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateAuthenticationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateAuthenticationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CreateAuthenticationResponse])
                 res.create_authentication_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -97,45 +96,44 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CheckResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CreateCheckResponse])
                 res.create_check_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -162,47 +160,46 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.FeedbackResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.FeedbackResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.FeedbackResponse])
                 res.feedback_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[errors.ErrorResponse])
                 res.error_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
 
         return res
@@ -225,45 +222,44 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.RetryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.RetryResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RetryAuthenticationResponse])
                 res.retry_authentication_response = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.ErrorResponse)
                 raise out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `ding_api_client-3.3.5/src/ding/sdk.py` & `ding_api_client-3.4.0/src/ding/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .lookup import Lookup
 from .otp import Otp
 from .sdkconfiguration import SDKConfiguration
+from .utils.retries import RetryConfig
 from ding import utils
 from ding._hooks import SDKHooks
 from ding.models import components
 from typing import Callable, Dict, Optional, Union
 
 class Ding:
     r"""Ding: The OTP API allows you to send authentication codes to your users using their phone numbers."""
@@ -20,30 +21,30 @@
 
     def __init__(self,
                  api_key: Union[str, Callable[[], str]],
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param api_key: The api_key required for authentication
         :type api_key: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(api_key):
             def security():
                 return components.Security(api_key = api_key())
```

### Comparing `ding_api_client-3.3.5/src/ding/sdkconfiguration.py` & `ding_api_client-3.4.0/src/ding/sdkconfiguration.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass
 from ding.models import components
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.ding.live/v1',
     # The production Ding API server
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '3.3.5'
-    gen_version: str = '2.291.0'
-    user_agent: str = 'speakeasy-sdk/python 3.3.5 2.291.0 1.0.0 ding_api_client'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '3.4.0'
+    gen_version: str = '2.298.0'
+    user_agent: str = 'speakeasy-sdk/python 3.4.0 2.298.0 1.0.0 ding_api_client'
+    retry_config: Optional[RetryConfig] = None
+    _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `ding_api_client-3.3.5/src/ding/utils/retries.py` & `ding_api_client-3.4.0/src/ding/utils/retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
```

### Comparing `ding_api_client-3.3.5/src/ding/utils/utils.py` & `ding_api_client-3.4.0/src/ding/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ding_api_client-3.3.5/src/ding_api_client.egg-info/PKG-INFO` & `ding_api_client-3.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: ding-api-client
-Version: 3.3.5
+Name: ding_api_client
+Version: 3.4.0
 Summary: Python Client SDK
-Home-page: UNKNOWN
+Home-page: https://github.com/ding-live/ding-python.git
 Author: Ding
 License: UNKNOWN
 Description: # Ding Python SDK
         
         The Ding Python library provides convenient access to the Ding API from applications written in the Python language.
         
         <!-- Start SDK Installation [installation] -->
@@ -121,15 +121,15 @@
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object         | Status Code          | Content Type         |
         | -------------------- | -------------------- | -------------------- |
         | errors.ErrorResponse | 400                  | application/json     |
-        | errors.SDKError      | 4x-5xx               | */*                  |
+        | errors.SDKError      | 4xx-5xx              | */*                  |
         
         ### Example
         
         ```python
         import ding
         from ding.models import components, errors
         
@@ -229,15 +229,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import ding
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = ding.Ding(client: http_client)
+        s = ding.Ding(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         <!-- Start Authentication [security] -->
         ## Authentication
         
         ### Per-Client Security Schemes
```

### Comparing `ding_api_client-3.3.5/src/ding_api_client.egg-info/SOURCES.txt` & `ding_api_client-3.4.0/src/ding_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

