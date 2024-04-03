# Comparing `tmp/python-teamcity-0.2.8.dev2.tar.gz` & `tmp/python-teamcity-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-teamcity-0.2.8.dev2.tar", last modified: Thu Mar 14 11:07:12 2024, max compression
+gzip compressed data, was "python-teamcity-0.2.9.tar", last modified: Wed Apr  3 11:54:30 2024, max compression
```

## Comparing `python-teamcity-0.2.8.dev2.tar` & `python-teamcity-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.418521 python-teamcity-0.2.8.dev2/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.408486 python-teamcity-0.2.8.dev2/.github/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.411546 python-teamcity-0.2.8.dev2/.github/workflows/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/.github/workflows/codeql.yml
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/AUTHORS
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1532 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/ChangeLog
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/LICENSE
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-03-14 11:07:12.418339 python-teamcity-0.2.8.dev2/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/README.md
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.412692 python-teamcity-0.2.8.dev2/examples/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/examples/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/examples/auth_sample.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3279 2024-03-14 09:12:36.000000 python-teamcity-0.2.8.dev2/examples/sample.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.417868 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      517 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/SOURCES.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/dependency_links.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/not-zip-safe
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/pbr.json
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/requires.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-03-14 11:07:12.000000 python-teamcity-0.2.8.dev2/python_teamcity.egg-info/top_level.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/requirements.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-03-14 11:07:12.418929 python-teamcity-0.2.8.dev2/setup.cfg
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/setup.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.416895 python-teamcity-0.2.8.dev2/teamcity/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/teamcity/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    21641 2024-03-14 09:12:36.000000 python-teamcity-0.2.8.dev2/teamcity/teamcity.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      225 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/teamcity/teamcity_const.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-14 11:07:12.417502 python-teamcity-0.2.8.dev2/tests/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.8.dev2/tests/__init__.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.889756 python-teamcity-0.2.9/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.878920 python-teamcity-0.2.9/.github/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.882324 python-teamcity-0.2.9/.github/workflows/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/.github/workflows/codeql.yml
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/AUTHORS
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1617 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/ChangeLog
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/LICENSE
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-03 11:54:30.889580 python-teamcity-0.2.9/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/README.md
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.884129 python-teamcity-0.2.9/examples/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/examples/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_auth.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_build.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1034 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_const.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3194 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_test.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.889126 python-teamcity-0.2.9/python_teamcity.egg-info/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      576 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/SOURCES.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/dependency_links.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.2.9/python_teamcity.egg-info/not-zip-safe
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/pbr.json
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/requires.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/top_level.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/requirements.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-04-03 11:54:30.890151 python-teamcity-0.2.9/setup.cfg
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/setup.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.888247 python-teamcity-0.2.9/teamcity/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/teamcity/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    22108 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/teamcity/teamcity.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      225 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/teamcity/teamcity_const.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.888717 python-teamcity-0.2.9/tests/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/tests/__init__.py
```

### Comparing `python-teamcity-0.2.8.dev2/.github/workflows/codeql.yml` & `python-teamcity-0.2.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.8.dev2/ChangeLog` & `python-teamcity-0.2.9/ChangeLog`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+v0.2.9
+------
+
+* Support to get latest build detail by build type id
+
+v0.2.8
+------
+
 * Update version info in setup.cfg to solve packing issue
 * Update version info in setup.cfg
 
 v0.2.5
 ------
 
 * Update sample.py
```

### Comparing `python-teamcity-0.2.8.dev2/LICENSE` & `python-teamcity-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.8.dev2/PKG-INFO` & `python-teamcity-0.2.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.2.8.dev2
+Version: 0.2.9
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.2.8.dev2/examples/sample.py` & `python-teamcity-0.2.9/examples/example_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # ********************************************************************************
 # © 2022-2024 Yunlin Tan. All Rights Reserved.
 # ********************************************************************************
 
 """
-@package examples.sample.py
+@package examples.example_test.py
 
 @brief python-teamcity example.
 
 @author Yunlin Tan
 
 @date 2/8/2024
 
@@ -17,59 +17,58 @@
 
 Arguments
 ---------
     - None
 
 Example Usage
 -------------
-    python3 examples/sample.py
+    python3 examples/example_test.py
 
 Update Record
 -------------
     None
 
 Depends On
 ----------
 **Python Dependencies:**
     - python-teamcity
 
 **Other Dependencies:**
     - None
 """
-import os
-
+from examples.example_const import *
 from teamcity import TeamCity
 
-# It is recommended to obtain TeamCity authorization via environment variables.
-TEAMCITY_SERVER = os.environ.get('TEAMCITY_SERVER', None)
-TEAMCITY_TOKENS = os.environ.get('TEAMCITY_TOKENS', None)
-
 # Initialize the TeamCity object with your server and tokens
 tc = TeamCity(server=TEAMCITY_SERVER, tokens=TEAMCITY_TOKENS)  # Recommended method
 
 # Get latest successful build details of a specific build_type_id
-latest_successful_build = tc.get_latest_build(build_type_id='build_type_id')  # Replace with your build_type_id
+latest_successful_build = tc.get_latest_build(build_type_id=EX_BUILD_TYPE_ID)
 print(latest_successful_build)
 
 # Get latest build details of a specific build_type_id
-latest_build = tc.get_latest_build(build_type_id='build_type_id', success_only=False)  # Replace with your build_type_id
+latest_build = tc.get_latest_build(build_type_id=EX_BUILD_TYPE_ID, success_only=False)
 print(latest_build)
 
 # Get details of a specific build using its build_id
-build_details = tc.get_build_details(build_id=33651345)  # Replace with your build_id
+build_details = tc.get_build_details(build_id=EX_BUILD_ID)  # Replace with your build_id
 print(build_details)
 
 # Get actual build parameters of the matching build.
-build_parameters = tc.get_build_actual_parameters(build_id=33651345)  # Replace with your build_id
+build_parameters = tc.get_build_actual_parameters(build_id=EX_BUILD_ID)  # Replace with your build_id
 print(build_parameters)
 
 # Get specific actual build parameter of the matching build.
-specific_parameters = tc.get_build_actual_parameters(build_id=33651345, property_name='build.number')
+specific_parameters = tc.get_build_actual_parameters(build_id=EX_BUILD_ID, property_name='build.number')
 print(specific_parameters)
 
+# Get canceled info of a specific build by build_id
+canceled_info = tc.get_canceled_info(build_id=EX_BUILD_ID)
+print(canceled_info)
+
 # # Get a list of all running builds
 # running_builds = tc.get_running_builds()
 # print(running_builds)
 #
 # # Get a list of artifacts for a specific build
 # artifacts_list = tc.get_artifacts_list(build_id=20240001)
 # print(artifacts_list)
```

### Comparing `python-teamcity-0.2.8.dev2/python_teamcity.egg-info/PKG-INFO` & `python-teamcity-0.2.9/python_teamcity.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.2.8.dev2
+Version: 0.2.9
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.2.8.dev2/setup.cfg` & `python-teamcity-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-teamcity
-version = 0.2.8
+version = 0.2.9
 author = Yunlin Tan
 author_email = tanyunlin2003@norbread.com
 summary = Python library for triggering TeamCity by REST API
 description_file = README.md
 license = MIT
 home_page = https://github.com/norbread2003/python-teamcity
 classifier =
```

### Comparing `python-teamcity-0.2.8.dev2/teamcity/teamcity.py` & `python-teamcity-0.2.9/teamcity/teamcity.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Arguments
 ---------
     - None
 
 Example Usage
 -------------
-    python3 examples/sample.py
+    python3 examples/example_test.py
 
 Update Record
 -------------
 0.1.0.1122   11/22/2022   Yunlin Tan([None])            Python API for triggering TeamCity by REST API.
 0.1.1        11/25/2022   Yunlin Tan([None])            Add more functions by requests.
 0.1.5        5/25/2023    Yunlin Tan([None])            Multiple features added.
 0.1.6        5/26/2023    Yunlin Tan([None])            Optimize get_build_dependencies function.
@@ -34,14 +34,15 @@
 0.1.9        10/18/2023   Yunlin Tan([None])            Support rerunning builds.
 0.2.0        11/13/2023   Yunlin Tan([None])            Change packing method.
 0.2.1        1/23/2024    Yunlin Tan([None])            Add agent-related functions.
 0.2.1        1/23/2024    Yunlin Tan([None])            Support to get agent details.
 0.2.3        2/1/2024     Yunlin Tan([None])            Support to get all agents (including unauthorized).
 0.2.4        3/4/2024     Yunlin Tan([None])            Support to get actual build parameters by resulting-properties.
 0.2.5        3/13/2024    Yunlin Tan([None])            Add more functions to get builds.
+0.2.9        4/3/2024     Yunlin Tan([None])            Support to get latest build detail by build type id.
 
 Depends On
 ----------
 **Python Dependencies:**
     - requests
 
 **Other Dependencies:**
@@ -59,15 +60,14 @@
     def __init__(self, server=None, tokens=None, user=None, password=None, guest=False):
         self.server = self.process_server_address(server or os.environ.get('TEAMCITY_SERVER', None))
         self.tokens = tokens or os.environ.get('TEAMCITY_TOKENS', None)
         self.user = user or os.environ.get('TEAMCITY_USER', None)
         self.password = password or os.environ.get('TEAMCITY_PASSWORD', None)
         self.guest = guest or os.environ.get('TEAMCITY_GUEST', False)
         self.authentication_method, self.base_url, self.header = self.check_auth_method()
-        self.session = requests.Session()
 
     @staticmethod
     def process_server_address(server: object):
         """Process server address."""
         if not server:
             logging.error('Failed to detect TeamCity server.')
             raise ValueError('TeamCity server is not set.')
@@ -98,23 +98,24 @@
             authentication_method = AUTH_METHOD.LOGGED_IN
             base_url = f'{self.server}/app/rest'
         return authentication_method, base_url, header
 
     def request_base(self, url, method, extra_headers={}, data=None, json=None, timeout=None, retries=3):
         url, headers = f'{self.base_url}/{url}', self.header
         headers.update(extra_headers)
+        session = requests.Session()
         logging.info(f'Calling TeamCity API: {url}')
 
         while retries > 0:
             try:
                 if self.authentication_method in [AUTH_METHOD.TOKENS, AUTH_METHOD.GUEST]:
-                    response = self.session.request(method, url, headers=headers, data=data, json=json, timeout=timeout)
+                    response = session.request(method, url, headers=headers, data=data, json=json, timeout=timeout)
                 elif self.authentication_method == AUTH_METHOD.USER:
-                    response = self.session.request(method, url, auth=(self.user, self.password), headers=headers,
-                                                    data=data, json=json, timeout=timeout)
+                    response = session.request(method, url, auth=(self.user, self.password), headers=headers,
+                                               data=data, json=json, timeout=timeout)
                 elif self.authentication_method == AUTH_METHOD.LOGGED_IN:
                     logging.error('You are not logged in to TeamCity, POST method is not supported.')
                     raise ValueError('You are not logged in to TeamCity, POST method is not supported.')
                 else:
                     logging.error('Unknown authentication method.')
                     raise ValueError('Unknown authentication method.')
 
@@ -160,30 +161,14 @@
         """
         url = f'builds?locator=defaultFilter:false,count:{count}'
         if build_type_id != '':
             url += f',buildType:(id:{build_type_id})'
         data = self.get_request(url)['build']
         return [self.get_build_details(build['id']) for build in data] if details else data
 
-    def get_latest_build(self, build_type_id='', success_only=True):
-        """Get latest build from TeamCity.
-        :param build_type_id: build type id in TeamCity, must be provided.
-        :param success_only: True to get the latest successful build, False to get the latest build.
-        :return: dict format latest build details, empty dict if no build found.
-
-        """
-        if success_only:
-            url = f'builds?locator=defaultFilter:false,count:1,status:SUCCESS'
-        else:
-            url = f'builds?locator=defaultFilter:false,count:1'
-        if build_type_id != '':
-            url += f',buildType:(id:{build_type_id})'
-        data = self.get_request(url)['build']
-        return self.get_build_details(data[0]['id']) if data else dict()
-
     def get_builds_by_date(self, start_date='', finish_date='', build_type_id='', details=False, count=100000):
         """Get builds by date from TeamCity."""
         url = f'builds?locator=defaultFilter:false,count:{count}'
         if build_type_id != '':
             url += f',buildType:(id:{build_type_id})'
         if start_date != '':
             url += f',startDate:{start_date}'
@@ -246,24 +231,50 @@
         """Get running builds from TeamCity."""
         url = f'builds?locator=defaultFilter:false,count:{count},running:true'
         if build_type_id != '':
             url += f',buildType:(id:{build_type_id})'
         data = self.get_request(url)['build']
         return [self.get_build_details(build['id']) for build in data] if details else data
 
+    def get_latest_build(self, build_type_id='', success_only=True):
+        """Get latest build from TeamCity.
+        :param build_type_id: build type id in TeamCity, must be provided.
+        :param success_only: True to get the latest successful build, False to get the latest build.
+        :return: dict format latest build details, empty dict if no build found.
+
+        """
+        if success_only:
+            url = f'builds?locator=defaultFilter:false,count:1,status:SUCCESS'
+        else:
+            url = f'builds?locator=defaultFilter:false,count:1'
+        if build_type_id != '':
+            url += f',buildType:(id:{build_type_id})'
+        data = self.get_request(url)['build']
+        return self.get_build_details(data[0]['id']) if data else dict()
+
     def get_build_details(self, build_id):
         """Get detail build by build id from TeamCity."""
         url = f'builds/id:{build_id}'
         try:
             return self.get_request(url)
         except Exception as ex:
             logging.error(ex)
             logging.error(f'Failed to get build {build_id} details.')
             return dict()
 
+    def get_canceled_info(self, build_id):
+        """Get canceled info by build id from TeamCity."""
+        url = f'builds/id:{build_id}/canceledInfo'
+        try:
+            return self.get_request(url)
+        except Exception as ex:
+            logging.error(ex)
+            logging.error(f'Failed to get build {build_id} canceled info.')
+            return dict()
+
     def get_build_actual_parameters(self, build_id, property_name=''):
         """Get actual build parameters of the matching build by resulting-properties from TeamCity.
 
         :param build_id: TeamCity build id.
         :param property_name: A valid property name could be empty.
         :return: List format actual parameters or string format specific result attributes.
         """
```

