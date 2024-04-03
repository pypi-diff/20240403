# Comparing `tmp/air-sdk-python-0.9.0.tar.gz` & `tmp/air-sdk-python-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "air-sdk-python-0.9.0.tar", last modified: Sat Oct 21 00:19:31 2023, max compression
+gzip compressed data, was "air-sdk-python-0.9.1.tar", last modified: Sat Oct 28 00:18:53 2023, max compression
```

## Comparing `air-sdk-python-0.9.0.tar` & `air-sdk-python-0.9.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     2445 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1095 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/
--rwxr-xr-x   0 runner    (1001) docker     (127)      127 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4373 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/models/errors/
--rwxr-xr-x   0 runner    (1001) docker     (127)      471 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/errors/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4751 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/errors/initiatecall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      700 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/operations/initiatecall.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      973 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/shared/call.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      330 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      999 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3786 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2023-10-21 00:19:13.000000 air-sdk-python-0.9.0/src/air/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 00:19:31.372664 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2023-10-21 00:19:30.000000 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-21 00:19:31.000000 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 00:19:30.000000 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-21 00:19:30.000000 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-21 00:19:30.000000 air-sdk-python-0.9.0/src/air_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.099195 air-sdk-python-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2023-10-28 00:18:53.099195 air-sdk-python-0.9.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5679 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 00:18:53.099195 air-sdk-python-0.9.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1095 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.091195 air-sdk-python-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.091195 air-sdk-python-0.9.1/src/air/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      127 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4373 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.091195 air-sdk-python-0.9.1/src/air/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.095195 air-sdk-python-0.9.1/src/air/models/errors/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      471 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/errors/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4751 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/errors/initiatecall.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      700 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.095195 air-sdk-python-0.9.1/src/air/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1153 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/operations/initiatecall.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.095195 air-sdk-python-0.9.1/src/air/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      973 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/shared/call.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      330 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2147 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      999 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.095195 air-sdk-python-0.9.1/src/air/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3786 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29304 2023-10-28 00:18:39.000000 air-sdk-python-0.9.1/src/air/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 00:18:53.099195 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2023-10-28 00:18:52.000000 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2023-10-28 00:18:53.000000 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 00:18:52.000000 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-10-28 00:18:52.000000 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-10-28 00:18:52.000000 air-sdk-python-0.9.1/src/air_sdk_python.egg-info/top_level.txt
```

### Comparing `air-sdk-python-0.9.0/LICENSE.md` & `air-sdk-python-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/setup.py` & `air-sdk-python-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="air-sdk-python",
-    version="0.9.0",
+    version="0.9.1",
     author="air",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
```

### Comparing `air-sdk-python-0.9.0/src/air/call.py` & `air-sdk-python-0.9.1/src/air/call.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/models/errors/initiatecall.py` & `air-sdk-python-0.9.1/src/air/models/errors/initiatecall.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/models/errors/sdkerror.py` & `air-sdk-python-0.9.1/src/air/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/models/operations/initiatecall.py` & `air-sdk-python-0.9.1/src/air/models/operations/initiatecall.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/models/shared/call.py` & `air-sdk-python-0.9.1/src/air/models/shared/call.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/sdk.py` & `air-sdk-python-0.9.1/src/air/sdk.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/sdkconfiguration.py` & `air-sdk-python-0.9.1/src/air/sdkconfiguration.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 class SDKConfiguration:
     client: requests.Session
     security_client: requests.Session
     server_url: str = ''
     server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.0'
-    sdk_version: str = '0.9.0'
-    gen_version: str = '2.169.0'
-    user_agent: str = 'speakeasy-sdk/python 0.9.0 2.169.0 1.0.0 air-sdk-python'
+    sdk_version: str = '0.9.1'
+    gen_version: str = '2.173.0'
+    user_agent: str = 'speakeasy-sdk/python 0.9.1 2.173.0 1.0.0 air-sdk-python'
     retry_config: RetryConfig = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url:
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `air-sdk-python-0.9.0/src/air/utils/retries.py` & `air-sdk-python-0.9.1/src/air/utils/retries.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air/utils/utils.py` & `air-sdk-python-0.9.1/src/air/utils/utils.py`

 * *Files identical despite different names*

### Comparing `air-sdk-python-0.9.0/src/air_sdk_python.egg-info/SOURCES.txt` & `air-sdk-python-0.9.1/src/air_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

