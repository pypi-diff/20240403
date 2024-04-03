# Comparing `tmp/ibm-project-sdk-0.0.4.tar.gz` & `tmp/ibm-project-sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-project-sdk-0.0.4.tar", last modified: Wed Mar 20 16:17:00 2024, max compression
+gzip compressed data, was "ibm-project-sdk-0.0.5.tar", last modified: Wed Apr  3 08:19:27 2024, max compression
```

## Comparing `ibm-project-sdk-0.0.4.tar` & `ibm-project-sdk-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-20 16:17:00.538845 ibm-project-sdk-0.0.4/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     4009 2024-03-20 16:17:00.538845 ibm-project-sdk-0.0.4/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-20 16:17:00.538845 ibm-project-sdk-0.0.4/ibm_project_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      895 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/ibm_project_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/ibm_project_sdk/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   412210 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/ibm_project_sdk/project_v1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/ibm_project_sdk/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-03-20 16:17:00.538845 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/
--rw-r--r--   0 travis    (2000) travis    (2000)     4009 2024-03-20 16:17:00.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      430 2024-03-20 16:17:00.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-20 16:17:00.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-03-20 16:17:00.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2024-03-20 16:17:00.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-03-20 16:15:30.000000 ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)      129 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/requirements-dev.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-03-20 16:17:00.538845 ibm-project-sdk-0.0.4/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-03-20 16:15:01.000000 ibm-project-sdk-0.0.4/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       70 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4009 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3041 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/ibm_project_sdk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      895 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2304 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   495442 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/project_v1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      652 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/ibm_project_sdk/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/
+-rw-r--r--   0 travis    (2000) travis    (2000)     4009 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      430 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2024-04-03 08:19:27.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2024-04-03 08:17:44.000000 ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)       64 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      129 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/requirements-dev.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       34 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2024-04-03 08:19:27.060692 ibm-project-sdk-0.0.5/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2604 2024-04-03 08:17:15.000000 ibm-project-sdk-0.0.5/setup.py
```

### Comparing `ibm-project-sdk-0.0.4/LICENSE` & `ibm-project-sdk-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.4/PKG-INFO` & `ibm-project-sdk-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-project-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Project Services Python SDK
 Home-page: https://github.com/IBM/project-python-sdk
 Author: IBM
 Author-email: dvesperini@gmail.com
 License: Apache 2.0
 Keywords: ibm_project_sdk
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.4
+# Project Services Python SDK Version 0.0.5
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -76,15 +76,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.4
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.4/README.md` & `ibm-project-sdk-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.4
+# Project Services Python SDK Version 0.0.5
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -51,15 +51,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.4
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.4/ibm_project_sdk/__init__.py` & `ibm-project-sdk-0.0.5/ibm_project_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.4/ibm_project_sdk/common.py` & `ibm-project-sdk-0.0.5/ibm_project_sdk/common.py`

 * *Files identical despite different names*

### Comparing `ibm-project-sdk-0.0.4/ibm_project_sdk/project_v1.py` & `ibm-project-sdk-0.0.5/ibm_project_sdk/project_v1.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# IBM OpenAPI SDK Code Generator Version: 3.80.0-29334a73-20230925-151553
+# IBM OpenAPI SDK Code Generator Version: 3.87.0-91c7c775-20240320-213027
 
 """
 Manage infrastructure as code in IBM Cloud.
 
 API Version: 1.0.0
 """
 
 from datetime import datetime
 from enum import Enum
-from typing import Dict, List
+from typing import Dict, List, Optional
 import json
 
 from ibm_cloud_sdk_core import BaseService, DetailedResponse, get_query_param
 from ibm_cloud_sdk_core.authenticators.authenticator import Authenticator
 from ibm_cloud_sdk_core.get_authenticator import get_authenticator_from_environment
 from ibm_cloud_sdk_core.utils import convert_model, datetime_to_string, string_to_datetime
 
@@ -78,16 +78,16 @@
 
     def create_project(
         self,
         definition: 'ProjectPrototypeDefinition',
         location: str,
         resource_group: str,
         *,
-        configs: List['ProjectConfigPrototype'] = None,
-        environments: List['EnvironmentPrototype'] = None,
+        configs: Optional[List['ProjectConfigPrototype']] = None,
+        environments: Optional[List['EnvironmentPrototype']] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Create a project.
 
         Create a new project and asynchronously setup the tools to manage it. Add a
         deployable architecture by customizing the configuration. After the changes are
@@ -157,16 +157,16 @@
 
         response = self.send(request, **kwargs)
         return response
 
     def list_projects(
         self,
         *,
-        token: str = None,
-        limit: int = None,
+        token: Optional[str] = None,
+        limit: Optional[int] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         List projects.
 
         List existing projects. Projects are sorted by ID.
 
@@ -353,74 +353,14 @@
             url=url,
             headers=headers,
         )
 
         response = self.send(request, **kwargs)
         return response
 
-    def list_project_resources(
-        self,
-        id: str,
-        *,
-        start: str = None,
-        limit: int = None,
-        **kwargs,
-    ) -> DetailedResponse:
-        """
-        List all project resources.
-
-        List resources that are added to a project.
-
-        :param str id: The unique project ID.
-        :param str start: (optional) The last entry that is returned on the page.
-               The server uses this parameter to determine the first entry that is
-               returned on the next page. If this parameter is not specified, the logical
-               first page is returned.
-        :param int limit: (optional) The maximum number of resources to return. The
-               number of resources that are returned is the same, except for the last
-               page.
-        :param dict headers: A `dict` containing the request headers
-        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
-        :rtype: DetailedResponse with `dict` result representing a `ProjectResourceCollection` object
-        """
-
-        if not id:
-            raise ValueError('id must be provided')
-        headers = {}
-        sdk_headers = get_sdk_headers(
-            service_name=self.DEFAULT_SERVICE_NAME,
-            service_version='V1',
-            operation_id='list_project_resources',
-        )
-        headers.update(sdk_headers)
-
-        params = {
-            'start': start,
-            'limit': limit,
-        }
-
-        if 'headers' in kwargs:
-            headers.update(kwargs.get('headers'))
-            del kwargs['headers']
-        headers['Accept'] = 'application/json'
-
-        path_param_keys = ['id']
-        path_param_values = self.encode_path_vars(id)
-        path_param_dict = dict(zip(path_param_keys, path_param_values))
-        url = '/v1/projects/{id}/resources'.format(**path_param_dict)
-        request = self.prepare_request(
-            method='GET',
-            url=url,
-            headers=headers,
-            params=params,
-        )
-
-        response = self.send(request, **kwargs)
-        return response
-
     #########################
     # Environments
     #########################
 
     def create_project_environment(
         self,
         project_id: str,
@@ -481,16 +421,16 @@
         response = self.send(request, **kwargs)
         return response
 
     def list_project_environments(
         self,
         project_id: str,
         *,
-        token: str = None,
-        limit: int = None,
+        token: Optional[str] = None,
+        limit: Optional[int] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         List environments.
 
         List all available environments. For more information, see [Creating an
         environment](/docs/secure-enterprise?topic=secure-enterprise-create-env).
@@ -706,15 +646,15 @@
     #########################
 
     def create_config(
         self,
         project_id: str,
         definition: 'ProjectConfigDefinitionPrototype',
         *,
-        schematics: 'SchematicsWorkspace' = None,
+        schematics: Optional['SchematicsWorkspace'] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Add a new configuration.
 
         Add a new configuration to a project.
 
@@ -785,16 +725,16 @@
         response = self.send(request, **kwargs)
         return response
 
     def list_configs(
         self,
         project_id: str,
         *,
-        token: str = None,
-        limit: int = None,
+        token: Optional[str] = None,
+        limit: Optional[int] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         List all project configurations.
 
         Retrieve the collection of configurations.
 
@@ -1069,15 +1009,15 @@
         return response
 
     def approve(
         self,
         project_id: str,
         id: str,
         *,
-        comment: str = None,
+        comment: Optional[str] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Approve and merge a configuration draft.
 
         Approve and merge configuration edits to the main configuration.
 
@@ -1279,15 +1219,15 @@
         return response
 
     def sync_config(
         self,
         project_id: str,
         id: str,
         *,
-        schematics: 'SchematicsWorkspace' = None,
+        schematics: Optional['SchematicsWorkspace'] = None,
         **kwargs,
     ) -> DetailedResponse:
         """
         Sync a project configuration.
 
         Sync a project configuration by analyzing the associated pipeline runs and
         Schematics workspace logs to get the configuration back to a working state.
@@ -1400,14 +1340,253 @@
             url=url,
             headers=headers,
         )
 
         response = self.send(request, **kwargs)
         return response
 
+    def create_stack_definition(
+        self,
+        project_id: str,
+        id: str,
+        stack_definition: 'StackDefinitionBlockPrototype',
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Create a stack definition.
+
+        Defines inputs at the stack level that users need to configure along with input
+        values at the member level. These values are included in the catalog entry when
+        the deployable architecture stack is exported to a private catalog and are
+        required for the deployable architecture stack to deploy. You can add a reference
+        to a value, or add the value explicitly at the member level.
+
+        :param str project_id: The unique project ID.
+        :param str id: The unique configuration ID.
+        :param StackDefinitionBlockPrototype stack_definition: The definition block
+               for a stack definition.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `StackDefinition` object
+        """
+
+        if not project_id:
+            raise ValueError('project_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if stack_definition is None:
+            raise ValueError('stack_definition must be provided')
+        stack_definition = convert_model(stack_definition)
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='create_stack_definition',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'stack_definition': stack_definition,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['project_id', 'id']
+        path_param_values = self.encode_path_vars(project_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/projects/{project_id}/configs/{id}/stack_definition'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def get_stack_definition(
+        self,
+        project_id: str,
+        id: str,
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Get a stack definition.
+
+        Retrieve the stack definition that is associated to the configuration.
+
+        :param str project_id: The unique project ID.
+        :param str id: The unique configuration ID.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `StackDefinition` object
+        """
+
+        if not project_id:
+            raise ValueError('project_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='get_stack_definition',
+        )
+        headers.update(sdk_headers)
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['project_id', 'id']
+        path_param_values = self.encode_path_vars(project_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/projects/{project_id}/configs/{id}/stack_definition'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='GET',
+            url=url,
+            headers=headers,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def update_stack_definition(
+        self,
+        project_id: str,
+        id: str,
+        stack_definition: 'StackDefinitionBlockPrototype',
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Update a stack definition.
+
+        Update the stack definition that is associated with the configuration.
+
+        :param str project_id: The unique project ID.
+        :param str id: The unique configuration ID.
+        :param StackDefinitionBlockPrototype stack_definition: The definition block
+               for a stack definition.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `StackDefinition` object
+        """
+
+        if not project_id:
+            raise ValueError('project_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if stack_definition is None:
+            raise ValueError('stack_definition must be provided')
+        stack_definition = convert_model(stack_definition)
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='update_stack_definition',
+        )
+        headers.update(sdk_headers)
+
+        data = {
+            'stack_definition': stack_definition,
+        }
+        data = {k: v for (k, v) in data.items() if v is not None}
+        data = json.dumps(data)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['project_id', 'id']
+        path_param_values = self.encode_path_vars(project_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/projects/{project_id}/configs/{id}/stack_definition'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='PATCH',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
+    def export_stack_definition(
+        self,
+        project_id: str,
+        id: str,
+        settings: 'StackDefinitionExportRequest',
+        **kwargs,
+    ) -> DetailedResponse:
+        """
+        Export a deployable architecture stack to the private catalog.
+
+        Exports the deployable architecture stack to a private catalog. All member
+        deployable architectures within the stack must be validated and deployed before
+        the stack is exported. The stack definition must also exist before the stack is
+        exported. You can export the stack as a new product, or as a new version of an
+        existing product.
+
+        :param str project_id: The unique project ID.
+        :param str id: The unique configuration ID.
+        :param StackDefinitionExportRequest settings: The payload for the private
+               catalog export request.
+        :param dict headers: A `dict` containing the request headers
+        :return: A `DetailedResponse` containing the result, headers and HTTP status code.
+        :rtype: DetailedResponse with `dict` result representing a `StackDefinitionExportResponse` object
+        """
+
+        if not project_id:
+            raise ValueError('project_id must be provided')
+        if not id:
+            raise ValueError('id must be provided')
+        if settings is None:
+            raise ValueError('settings must be provided')
+        if isinstance(settings, StackDefinitionExportRequest):
+            settings = convert_model(settings)
+        headers = {}
+        sdk_headers = get_sdk_headers(
+            service_name=self.DEFAULT_SERVICE_NAME,
+            service_version='V1',
+            operation_id='export_stack_definition',
+        )
+        headers.update(sdk_headers)
+
+        data = json.dumps(settings)
+        headers['content-type'] = 'application/json'
+
+        if 'headers' in kwargs:
+            headers.update(kwargs.get('headers'))
+            del kwargs['headers']
+        headers['Accept'] = 'application/json'
+
+        path_param_keys = ['project_id', 'id']
+        path_param_values = self.encode_path_vars(project_id, id)
+        path_param_dict = dict(zip(path_param_keys, path_param_values))
+        url = '/v1/projects/{project_id}/configs/{id}/stack_definition/export'.format(**path_param_dict)
+        request = self.prepare_request(
+            method='POST',
+            url=url,
+            headers=headers,
+            data=data,
+        )
+
+        response = self.send(request, **kwargs)
+        return response
+
     def list_config_versions(
         self,
         project_id: str,
         id: str,
         **kwargs,
     ) -> DetailedResponse:
         """
@@ -1563,27 +1742,27 @@
 ##############################################################################
 
 
 class ActionJobApplyMessagesSummary:
     """
     The messages of apply jobs on the configuration.
 
-    :attr List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
+    :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
           collection of error messages. This property is reported only if Schematics
           triggered a Terraform apply job.
-    :attr List[TerraformLogAnalyzerSuccessMessage] success_messages: (optional) The
+    :param List[TerraformLogAnalyzerSuccessMessage] success_messages: (optional) The
           collection of success messages. This property is reported only if Schematics
           triggered a Terraform apply job.
     """
 
     def __init__(
         self,
         *,
-        error_messages: List['TerraformLogAnalyzerErrorMessage'] = None,
-        success_messages: List['TerraformLogAnalyzerSuccessMessage'] = None,
+        error_messages: Optional[List['TerraformLogAnalyzerErrorMessage']] = None,
+        success_messages: Optional[List['TerraformLogAnalyzerSuccessMessage']] = None,
     ) -> None:
         """
         Initialize a ActionJobApplyMessagesSummary object.
 
         :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional)
                The collection of error messages. This property is reported only if
                Schematics triggered a Terraform apply job.
@@ -1594,22 +1773,18 @@
         self.error_messages = error_messages
         self.success_messages = success_messages
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobApplyMessagesSummary':
         """Initialize a ActionJobApplyMessagesSummary object from a json dictionary."""
         args = {}
-        if 'error_messages' in _dict:
-            args['error_messages'] = [
-                TerraformLogAnalyzerErrorMessage.from_dict(v) for v in _dict.get('error_messages')
-            ]
-        if 'success_messages' in _dict:
-            args['success_messages'] = [
-                TerraformLogAnalyzerSuccessMessage.from_dict(v) for v in _dict.get('success_messages')
-            ]
+        if (error_messages := _dict.get('error_messages')) is not None:
+            args['error_messages'] = [TerraformLogAnalyzerErrorMessage.from_dict(v) for v in error_messages]
+        if (success_messages := _dict.get('success_messages')) is not None:
+            args['success_messages'] = [TerraformLogAnalyzerSuccessMessage.from_dict(v) for v in success_messages]
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobApplyMessagesSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1653,33 +1828,33 @@
         return not self == other
 
 
 class ActionJobApplySummary:
     """
     The summary of the apply jobs on the configuration.
 
-    :attr int success: (optional) The number of applied resources. This property is
+    :param int success: (optional) The number of applied resources. This property is
           reported only if Schematics triggered a Terraform apply job.
-    :attr int failed: (optional) The number of failed applied resources. This
+    :param int failed: (optional) The number of failed applied resources. This
           property is reported only if Schematics triggered a Terraform apply job.
-    :attr List[str] success_resources: (optional) The collection of successfully
+    :param List[str] success_resources: (optional) The collection of successfully
           applied resources. This property is reported only if Schematics triggered a
           Terraform apply job.
-    :attr List[str] failed_resources: (optional) The collection of failed applied
+    :param List[str] failed_resources: (optional) The collection of failed applied
           resources. This property is reported only if Schematics triggered a Terraform
           apply job.
     """
 
     def __init__(
         self,
         *,
-        success: int = None,
-        failed: int = None,
-        success_resources: List[str] = None,
-        failed_resources: List[str] = None,
+        success: Optional[int] = None,
+        failed: Optional[int] = None,
+        success_resources: Optional[List[str]] = None,
+        failed_resources: Optional[List[str]] = None,
     ) -> None:
         """
         Initialize a ActionJobApplySummary object.
 
         :param int success: (optional) The number of applied resources. This
                property is reported only if Schematics triggered a Terraform apply job.
         :param int failed: (optional) The number of failed applied resources. This
@@ -1696,22 +1871,22 @@
         self.success_resources = success_resources
         self.failed_resources = failed_resources
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobApplySummary':
         """Initialize a ActionJobApplySummary object from a json dictionary."""
         args = {}
-        if 'success' in _dict:
-            args['success'] = _dict.get('success')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'success_resources' in _dict:
-            args['success_resources'] = _dict.get('success_resources')
-        if 'failed_resources' in _dict:
-            args['failed_resources'] = _dict.get('failed_resources')
+        if (success := _dict.get('success')) is not None:
+            args['success'] = success
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (success_resources := _dict.get('success_resources')) is not None:
+            args['success_resources'] = success_resources
+        if (failed_resources := _dict.get('failed_resources')) is not None:
+            args['failed_resources'] = failed_resources
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobApplySummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1747,41 +1922,39 @@
         return not self == other
 
 
 class ActionJobDestroyMessagesSummary:
     """
     The messages of destroy jobs on the configuration.
 
-    :attr List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
+    :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
           collection of error messages. This property is reported only if Schematics
           triggered a Terraform destroy job.
     """
 
     def __init__(
         self,
         *,
-        error_messages: List['TerraformLogAnalyzerErrorMessage'] = None,
+        error_messages: Optional[List['TerraformLogAnalyzerErrorMessage']] = None,
     ) -> None:
         """
         Initialize a ActionJobDestroyMessagesSummary object.
 
         :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional)
                The collection of error messages. This property is reported only if
                Schematics triggered a Terraform destroy job.
         """
         self.error_messages = error_messages
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobDestroyMessagesSummary':
         """Initialize a ActionJobDestroyMessagesSummary object from a json dictionary."""
         args = {}
-        if 'error_messages' in _dict:
-            args['error_messages'] = [
-                TerraformLogAnalyzerErrorMessage.from_dict(v) for v in _dict.get('error_messages')
-            ]
+        if (error_messages := _dict.get('error_messages')) is not None:
+            args['error_messages'] = [TerraformLogAnalyzerErrorMessage.from_dict(v) for v in error_messages]
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobDestroyMessagesSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1817,32 +1990,32 @@
         return not self == other
 
 
 class ActionJobDestroySummary:
     """
     The summary of the destroy jobs on the configuration.
 
-    :attr int success: (optional) The number of destroyed resources. This property
+    :param int success: (optional) The number of destroyed resources. This property
           is reported only if Schematics triggered a Terraform destroy job.
-    :attr int failed: (optional) The number of failed resources. This property is
+    :param int failed: (optional) The number of failed resources. This property is
           reported only if Schematics triggered a Terraform destroy job.
-    :attr int tainted: (optional) The number of tainted resources. This property is
+    :param int tainted: (optional) The number of tainted resources. This property is
           reported only if Schematics triggered a Terraform destroy job.
-    :attr ActionJobDestroySummaryResources resources: (optional) The summary of
+    :param ActionJobDestroySummaryResources resources: (optional) The summary of
           results from destroyed resources from the job. This property is reported only if
           Schematics triggered a Terraform destroy job.
     """
 
     def __init__(
         self,
         *,
-        success: int = None,
-        failed: int = None,
-        tainted: int = None,
-        resources: 'ActionJobDestroySummaryResources' = None,
+        success: Optional[int] = None,
+        failed: Optional[int] = None,
+        tainted: Optional[int] = None,
+        resources: Optional['ActionJobDestroySummaryResources'] = None,
     ) -> None:
         """
         Initialize a ActionJobDestroySummary object.
 
         :param int success: (optional) The number of destroyed resources. This
                property is reported only if Schematics triggered a Terraform destroy job.
         :param int failed: (optional) The number of failed resources. This property
@@ -1858,22 +2031,22 @@
         self.tainted = tainted
         self.resources = resources
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobDestroySummary':
         """Initialize a ActionJobDestroySummary object from a json dictionary."""
         args = {}
-        if 'success' in _dict:
-            args['success'] = _dict.get('success')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'tainted' in _dict:
-            args['tainted'] = _dict.get('tainted')
-        if 'resources' in _dict:
-            args['resources'] = ActionJobDestroySummaryResources.from_dict(_dict.get('resources'))
+        if (success := _dict.get('success')) is not None:
+            args['success'] = success
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (tainted := _dict.get('tainted')) is not None:
+            args['tainted'] = tainted
+        if (resources := _dict.get('resources')) is not None:
+            args['resources'] = ActionJobDestroySummaryResources.from_dict(resources)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobDestroySummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1913,28 +2086,28 @@
 
 
 class ActionJobDestroySummaryResources:
     """
     The summary of results from destroyed resources from the job. This property is
     reported only if Schematics triggered a Terraform destroy job.
 
-    :attr List[str] success: (optional) The collection of destroyed resources. This
+    :param List[str] success: (optional) The collection of destroyed resources. This
           property is reported only if Schematics triggered a Terraform destroy job.
-    :attr List[str] failed: (optional) The collection of failed resources. This
+    :param List[str] failed: (optional) The collection of failed resources. This
           property is reported only if Schematics triggered a Terraform destroy job.
-    :attr List[str] tainted: (optional) The collection of tainted resources. This
+    :param List[str] tainted: (optional) The collection of tainted resources. This
           property is reported only if Schematics triggered a Terraform destroy job.
     """
 
     def __init__(
         self,
         *,
-        success: List[str] = None,
-        failed: List[str] = None,
-        tainted: List[str] = None,
+        success: Optional[List[str]] = None,
+        failed: Optional[List[str]] = None,
+        tainted: Optional[List[str]] = None,
     ) -> None:
         """
         Initialize a ActionJobDestroySummaryResources object.
 
         :param List[str] success: (optional) The collection of destroyed resources.
                This property is reported only if Schematics triggered a Terraform destroy
                job.
@@ -1949,20 +2122,20 @@
         self.failed = failed
         self.tainted = tainted
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobDestroySummaryResources':
         """Initialize a ActionJobDestroySummaryResources object from a json dictionary."""
         args = {}
-        if 'success' in _dict:
-            args['success'] = _dict.get('success')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'tainted' in _dict:
-            args['tainted'] = _dict.get('tainted')
+        if (success := _dict.get('success')) is not None:
+            args['success'] = success
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (tainted := _dict.get('tainted')) is not None:
+            args['tainted'] = tainted
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobDestroySummaryResources object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -1996,28 +2169,28 @@
         return not self == other
 
 
 class ActionJobMessageSummary:
     """
     The message summaries of jobs on the configuration.
 
-    :attr int info: (optional) The number of information messages. This property is
+    :param int info: (optional) The number of information messages. This property is
           reported only if Schematics triggered a Terraform job.
-    :attr int debug: (optional) The number of debug messages. This property is
+    :param int debug: (optional) The number of debug messages. This property is
           reported only if Schematics triggered a Terraform job.
-    :attr int error: (optional) The number of error messages. This property is
+    :param int error: (optional) The number of error messages. This property is
           reported only if Schematics triggered a Terraform job.
     """
 
     def __init__(
         self,
         *,
-        info: int = None,
-        debug: int = None,
-        error: int = None,
+        info: Optional[int] = None,
+        debug: Optional[int] = None,
+        error: Optional[int] = None,
     ) -> None:
         """
         Initialize a ActionJobMessageSummary object.
 
         :param int info: (optional) The number of information messages. This
                property is reported only if Schematics triggered a Terraform job.
         :param int debug: (optional) The number of debug messages. This property is
@@ -2029,20 +2202,20 @@
         self.debug = debug
         self.error = error
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobMessageSummary':
         """Initialize a ActionJobMessageSummary object from a json dictionary."""
         args = {}
-        if 'info' in _dict:
-            args['info'] = _dict.get('info')
-        if 'debug' in _dict:
-            args['debug'] = _dict.get('debug')
-        if 'error' in _dict:
-            args['error'] = _dict.get('error')
+        if (info := _dict.get('info')) is not None:
+            args['info'] = info
+        if (debug := _dict.get('debug')) is not None:
+            args['debug'] = debug
+        if (error := _dict.get('error')) is not None:
+            args['error'] = error
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobMessageSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2076,32 +2249,34 @@
         return not self == other
 
 
 class ActionJobPlanMessagesSummary:
     """
     The plan messages on the configuration.
 
-    :attr List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
+    :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional) The
           collection of error messages. This property is reported only if Schematics
           triggered a Terraform plan job.
-    :attr List[str] success_messages: (optional) The collection of success messages.
-          This property is reported only if Schematics triggered a Terraform plan job.
-    :attr List[str] update_messages: (optional) The collection of update messages.
-          This property is reported only if Schematics triggered a Terraform plan job.
-    :attr List[str] destroy_messages: (optional) The collection of destroy messages.
+    :param List[str] success_messages: (optional) The collection of success
+          messages. This property is reported only if Schematics triggered a Terraform
+          plan job.
+    :param List[str] update_messages: (optional) The collection of update messages.
           This property is reported only if Schematics triggered a Terraform plan job.
+    :param List[str] destroy_messages: (optional) The collection of destroy
+          messages. This property is reported only if Schematics triggered a Terraform
+          plan job.
     """
 
     def __init__(
         self,
         *,
-        error_messages: List['TerraformLogAnalyzerErrorMessage'] = None,
-        success_messages: List[str] = None,
-        update_messages: List[str] = None,
-        destroy_messages: List[str] = None,
+        error_messages: Optional[List['TerraformLogAnalyzerErrorMessage']] = None,
+        success_messages: Optional[List[str]] = None,
+        update_messages: Optional[List[str]] = None,
+        destroy_messages: Optional[List[str]] = None,
     ) -> None:
         """
         Initialize a ActionJobPlanMessagesSummary object.
 
         :param List[TerraformLogAnalyzerErrorMessage] error_messages: (optional)
                The collection of error messages. This property is reported only if
                Schematics triggered a Terraform plan job.
@@ -2120,24 +2295,22 @@
         self.update_messages = update_messages
         self.destroy_messages = destroy_messages
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobPlanMessagesSummary':
         """Initialize a ActionJobPlanMessagesSummary object from a json dictionary."""
         args = {}
-        if 'error_messages' in _dict:
-            args['error_messages'] = [
-                TerraformLogAnalyzerErrorMessage.from_dict(v) for v in _dict.get('error_messages')
-            ]
-        if 'success_messages' in _dict:
-            args['success_messages'] = _dict.get('success_messages')
-        if 'update_messages' in _dict:
-            args['update_messages'] = _dict.get('update_messages')
-        if 'destroy_messages' in _dict:
-            args['destroy_messages'] = _dict.get('destroy_messages')
+        if (error_messages := _dict.get('error_messages')) is not None:
+            args['error_messages'] = [TerraformLogAnalyzerErrorMessage.from_dict(v) for v in error_messages]
+        if (success_messages := _dict.get('success_messages')) is not None:
+            args['success_messages'] = success_messages
+        if (update_messages := _dict.get('update_messages')) is not None:
+            args['update_messages'] = update_messages
+        if (destroy_messages := _dict.get('destroy_messages')) is not None:
+            args['destroy_messages'] = destroy_messages
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobPlanMessagesSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2179,48 +2352,48 @@
         return not self == other
 
 
 class ActionJobPlanSummary:
     """
     The summary of the plan jobs on the configuration.
 
-    :attr int add: (optional) The number of resources to be added. This property is
+    :param int add: (optional) The number of resources to be added. This property is
           reported only if Schematics triggered a terraform plan job.
-    :attr int failed: (optional) The number of resources that failed during the plan
-          job. This property is reported only if Schematics triggered a Terraform plan
-          job.
-    :attr int update: (optional) The number of resources to be updated. This
+    :param int failed: (optional) The number of resources that failed during the
+          plan job. This property is reported only if Schematics triggered a Terraform
+          plan job.
+    :param int update: (optional) The number of resources to be updated. This
           property is reported only if Schematics triggered a Terraform plan job.
-    :attr int destroy: (optional) The number of resources to be destroyed. This
+    :param int destroy: (optional) The number of resources to be destroyed. This
           property is reported only if Schematics triggered a Terraform plan job.
-    :attr List[str] add_resources: (optional) The collection of planned added
+    :param List[str] add_resources: (optional) The collection of planned added
           resources. This property is reported only if Schematics triggered a Terraform
           plan job.
-    :attr List[str] failed_resources: (optional) The collection of failed planned
+    :param List[str] failed_resources: (optional) The collection of failed planned
           resources. This property is reported only if Schematics triggered a Terraform
           plan job.
-    :attr List[str] updated_resources: (optional) The collection of planned updated
+    :param List[str] updated_resources: (optional) The collection of planned updated
           resources. This property is reported only if Schematics triggered a Terraform
           plan job.
-    :attr List[str] destroy_resources: (optional) The collection of planned destroy
+    :param List[str] destroy_resources: (optional) The collection of planned destroy
           resources. This property is reported only if Schematics triggered a Terraform
           plan job.
     """
 
     def __init__(
         self,
         *,
-        add: int = None,
-        failed: int = None,
-        update: int = None,
-        destroy: int = None,
-        add_resources: List[str] = None,
-        failed_resources: List[str] = None,
-        updated_resources: List[str] = None,
-        destroy_resources: List[str] = None,
+        add: Optional[int] = None,
+        failed: Optional[int] = None,
+        update: Optional[int] = None,
+        destroy: Optional[int] = None,
+        add_resources: Optional[List[str]] = None,
+        failed_resources: Optional[List[str]] = None,
+        updated_resources: Optional[List[str]] = None,
+        destroy_resources: Optional[List[str]] = None,
     ) -> None:
         """
         Initialize a ActionJobPlanSummary object.
 
         :param int add: (optional) The number of resources to be added. This
                property is reported only if Schematics triggered a terraform plan job.
         :param int failed: (optional) The number of resources that failed during
@@ -2253,30 +2426,30 @@
         self.updated_resources = updated_resources
         self.destroy_resources = destroy_resources
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobPlanSummary':
         """Initialize a ActionJobPlanSummary object from a json dictionary."""
         args = {}
-        if 'add' in _dict:
-            args['add'] = _dict.get('add')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'update' in _dict:
-            args['update'] = _dict.get('update')
-        if 'destroy' in _dict:
-            args['destroy'] = _dict.get('destroy')
-        if 'add_resources' in _dict:
-            args['add_resources'] = _dict.get('add_resources')
-        if 'failed_resources' in _dict:
-            args['failed_resources'] = _dict.get('failed_resources')
-        if 'updated_resources' in _dict:
-            args['updated_resources'] = _dict.get('updated_resources')
-        if 'destroy_resources' in _dict:
-            args['destroy_resources'] = _dict.get('destroy_resources')
+        if (add := _dict.get('add')) is not None:
+            args['add'] = add
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (update := _dict.get('update')) is not None:
+            args['update'] = update
+        if (destroy := _dict.get('destroy')) is not None:
+            args['destroy'] = destroy
+        if (add_resources := _dict.get('add_resources')) is not None:
+            args['add_resources'] = add_resources
+        if (failed_resources := _dict.get('failed_resources')) is not None:
+            args['failed_resources'] = failed_resources
+        if (updated_resources := _dict.get('updated_resources')) is not None:
+            args['updated_resources'] = updated_resources
+        if (destroy_resources := _dict.get('destroy_resources')) is not None:
+            args['destroy_resources'] = destroy_resources
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobPlanSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2320,28 +2493,28 @@
         return not self == other
 
 
 class ActionJobSummary:
     """
     The summaries of jobs that were performed on the configuration.
 
-    :attr str version: The version of the job summary.
-    :attr ActionJobPlanSummary plan_summary: The summary of the plan jobs on the
+    :param str version: The version of the job summary.
+    :param ActionJobPlanSummary plan_summary: The summary of the plan jobs on the
           configuration.
-    :attr ActionJobApplySummary apply_summary: The summary of the apply jobs on the
+    :param ActionJobApplySummary apply_summary: The summary of the apply jobs on the
           configuration.
-    :attr ActionJobDestroySummary destroy_summary: The summary of the destroy jobs
+    :param ActionJobDestroySummary destroy_summary: The summary of the destroy jobs
           on the configuration.
-    :attr ActionJobMessageSummary message_summary: The message summaries of jobs on
+    :param ActionJobMessageSummary message_summary: The message summaries of jobs on
           the configuration.
-    :attr ActionJobPlanMessagesSummary plan_messages: The plan messages on the
+    :param ActionJobPlanMessagesSummary plan_messages: The plan messages on the
           configuration.
-    :attr ActionJobApplyMessagesSummary apply_messages: The messages of apply jobs
+    :param ActionJobApplyMessagesSummary apply_messages: The messages of apply jobs
           on the configuration.
-    :attr ActionJobDestroyMessagesSummary destroy_messages: The messages of destroy
+    :param ActionJobDestroyMessagesSummary destroy_messages: The messages of destroy
           jobs on the configuration.
     """
 
     def __init__(
         self,
         version: str,
         plan_summary: 'ActionJobPlanSummary',
@@ -2380,44 +2553,44 @@
         self.apply_messages = apply_messages
         self.destroy_messages = destroy_messages
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobSummary':
         """Initialize a ActionJobSummary object from a json dictionary."""
         args = {}
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ActionJobSummary JSON')
-        if 'plan_summary' in _dict:
-            args['plan_summary'] = ActionJobPlanSummary.from_dict(_dict.get('plan_summary'))
+        if (plan_summary := _dict.get('plan_summary')) is not None:
+            args['plan_summary'] = ActionJobPlanSummary.from_dict(plan_summary)
         else:
             raise ValueError('Required property \'plan_summary\' not present in ActionJobSummary JSON')
-        if 'apply_summary' in _dict:
-            args['apply_summary'] = ActionJobApplySummary.from_dict(_dict.get('apply_summary'))
+        if (apply_summary := _dict.get('apply_summary')) is not None:
+            args['apply_summary'] = ActionJobApplySummary.from_dict(apply_summary)
         else:
             raise ValueError('Required property \'apply_summary\' not present in ActionJobSummary JSON')
-        if 'destroy_summary' in _dict:
-            args['destroy_summary'] = ActionJobDestroySummary.from_dict(_dict.get('destroy_summary'))
+        if (destroy_summary := _dict.get('destroy_summary')) is not None:
+            args['destroy_summary'] = ActionJobDestroySummary.from_dict(destroy_summary)
         else:
             raise ValueError('Required property \'destroy_summary\' not present in ActionJobSummary JSON')
-        if 'message_summary' in _dict:
-            args['message_summary'] = ActionJobMessageSummary.from_dict(_dict.get('message_summary'))
+        if (message_summary := _dict.get('message_summary')) is not None:
+            args['message_summary'] = ActionJobMessageSummary.from_dict(message_summary)
         else:
             raise ValueError('Required property \'message_summary\' not present in ActionJobSummary JSON')
-        if 'plan_messages' in _dict:
-            args['plan_messages'] = ActionJobPlanMessagesSummary.from_dict(_dict.get('plan_messages'))
+        if (plan_messages := _dict.get('plan_messages')) is not None:
+            args['plan_messages'] = ActionJobPlanMessagesSummary.from_dict(plan_messages)
         else:
             raise ValueError('Required property \'plan_messages\' not present in ActionJobSummary JSON')
-        if 'apply_messages' in _dict:
-            args['apply_messages'] = ActionJobApplyMessagesSummary.from_dict(_dict.get('apply_messages'))
+        if (apply_messages := _dict.get('apply_messages')) is not None:
+            args['apply_messages'] = ActionJobApplyMessagesSummary.from_dict(apply_messages)
         else:
             raise ValueError('Required property \'apply_messages\' not present in ActionJobSummary JSON')
-        if 'destroy_messages' in _dict:
-            args['destroy_messages'] = ActionJobDestroyMessagesSummary.from_dict(_dict.get('destroy_messages'))
+        if (destroy_messages := _dict.get('destroy_messages')) is not None:
+            args['destroy_messages'] = ActionJobDestroyMessagesSummary.from_dict(destroy_messages)
         else:
             raise ValueError('Required property \'destroy_messages\' not present in ActionJobSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobSummary object from a json dictionary."""
@@ -2484,17 +2657,17 @@
         return not self == other
 
 
 class ActionJobWithIdAndSummary:
     """
     A brief summary of an action.
 
-    :attr str id: The unique ID.
-    :attr ActionJobSummary summary: The summaries of jobs that were performed on the
-          configuration.
+    :param str id: The unique ID.
+    :param ActionJobSummary summary: The summaries of jobs that were performed on
+          the configuration.
     """
 
     def __init__(
         self,
         id: str,
         summary: 'ActionJobSummary',
     ) -> None:
@@ -2508,20 +2681,20 @@
         self.id = id
         self.summary = summary
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ActionJobWithIdAndSummary':
         """Initialize a ActionJobWithIdAndSummary object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ActionJobWithIdAndSummary JSON')
-        if 'summary' in _dict:
-            args['summary'] = ActionJobSummary.from_dict(_dict.get('summary'))
+        if (summary := _dict.get('summary')) is not None:
+            args['summary'] = ActionJobSummary.from_dict(summary)
         else:
             raise ValueError('Required property \'summary\' not present in ActionJobWithIdAndSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ActionJobWithIdAndSummary object from a json dictionary."""
@@ -2558,31 +2731,31 @@
         return not self == other
 
 
 class CodeRiskAnalyzerLogsSummary:
     """
     The Code Risk Analyzer logs a summary of the configuration.
 
-    :attr str total: (optional) The total number of Code Risk Analyzer rules that
+    :param str total: (optional) The total number of Code Risk Analyzer rules that
           were applied in the scan.
-    :attr str passed: (optional) The number of Code Risk Analyzer rules that passed
+    :param str passed: (optional) The number of Code Risk Analyzer rules that passed
           in the scan.
-    :attr str failed: (optional) The number of Code Risk Analyzer rules that failed
+    :param str failed: (optional) The number of Code Risk Analyzer rules that failed
           in the scan.
-    :attr str skipped: (optional) The number of Code Risk Analyzer rules that were
+    :param str skipped: (optional) The number of Code Risk Analyzer rules that were
           skipped in the scan.
     """
 
     def __init__(
         self,
         *,
-        total: str = None,
-        passed: str = None,
-        failed: str = None,
-        skipped: str = None,
+        total: Optional[str] = None,
+        passed: Optional[str] = None,
+        failed: Optional[str] = None,
+        skipped: Optional[str] = None,
     ) -> None:
         """
         Initialize a CodeRiskAnalyzerLogsSummary object.
 
         :param str total: (optional) The total number of Code Risk Analyzer rules
                that were applied in the scan.
         :param str passed: (optional) The number of Code Risk Analyzer rules that
@@ -2597,22 +2770,22 @@
         self.failed = failed
         self.skipped = skipped
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'CodeRiskAnalyzerLogsSummary':
         """Initialize a CodeRiskAnalyzerLogsSummary object from a json dictionary."""
         args = {}
-        if 'total' in _dict:
-            args['total'] = _dict.get('total')
-        if 'passed' in _dict:
-            args['passed'] = _dict.get('passed')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'skipped' in _dict:
-            args['skipped'] = _dict.get('skipped')
+        if (total := _dict.get('total')) is not None:
+            args['total'] = total
+        if (passed := _dict.get('passed')) is not None:
+            args['passed'] = passed
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (skipped := _dict.get('skipped')) is not None:
+            args['skipped'] = skipped
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a CodeRiskAnalyzerLogsSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2644,31 +2817,90 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'CodeRiskAnalyzerLogsSummary') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ConfigDefinitionReference:
+    """
+    The definition of the config reference.
+
+    :param str name: The name of the configuration.
+    """
+
+    def __init__(
+        self,
+        name: str,
+    ) -> None:
+        """
+        Initialize a ConfigDefinitionReference object.
+
+        :param str name: The name of the configuration.
+        """
+        self.name = name
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ConfigDefinitionReference':
+        """Initialize a ConfigDefinitionReference object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in ConfigDefinitionReference JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ConfigDefinitionReference object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ConfigDefinitionReference object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ConfigDefinitionReference') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ConfigDefinitionReference') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class CumulativeNeedsAttention:
     """
     CumulativeNeedsAttention.
 
-    :attr str event: (optional) The event name.
-    :attr str event_id: (optional) A unique ID for this individual event.
-    :attr str config_id: (optional) A unique ID for the configuration.
-    :attr int config_version: (optional) The version number of the configuration.
+    :param str event: (optional) The event name.
+    :param str event_id: (optional) A unique ID for this individual event.
+    :param str config_id: (optional) A unique ID for the configuration.
+    :param int config_version: (optional) The version number of the configuration.
     """
 
     def __init__(
         self,
         *,
-        event: str = None,
-        event_id: str = None,
-        config_id: str = None,
-        config_version: int = None,
+        event: Optional[str] = None,
+        event_id: Optional[str] = None,
+        config_id: Optional[str] = None,
+        config_version: Optional[int] = None,
     ) -> None:
         """
         Initialize a CumulativeNeedsAttention object.
 
         :param str event: (optional) The event name.
         :param str event_id: (optional) A unique ID for this individual event.
         :param str config_id: (optional) A unique ID for the configuration.
@@ -2680,22 +2912,22 @@
         self.config_id = config_id
         self.config_version = config_version
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'CumulativeNeedsAttention':
         """Initialize a CumulativeNeedsAttention object from a json dictionary."""
         args = {}
-        if 'event' in _dict:
-            args['event'] = _dict.get('event')
-        if 'event_id' in _dict:
-            args['event_id'] = _dict.get('event_id')
-        if 'config_id' in _dict:
-            args['config_id'] = _dict.get('config_id')
-        if 'config_version' in _dict:
-            args['config_version'] = _dict.get('config_version')
+        if (event := _dict.get('event')) is not None:
+            args['event'] = event
+        if (event_id := _dict.get('event_id')) is not None:
+            args['event_id'] = event_id
+        if (config_id := _dict.get('config_id')) is not None:
+            args['config_id'] = config_id
+        if (config_version := _dict.get('config_version')) is not None:
+            args['config_version'] = config_version
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a CumulativeNeedsAttention object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2731,40 +2963,41 @@
         return not self == other
 
 
 class Environment:
     """
     The definition of a project environment.
 
-    :attr str id: The environment ID as a friendly name.
-    :attr ProjectReference project: The project that is referenced by this resource.
-    :attr datetime created_at: A date and time value in the format
+    :param str id: The environment ID as a friendly name.
+    :param ProjectReference project: The project that is referenced by this
+          resource.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str target_account: (optional) The target account ID derived from the
+    :param str target_account: (optional) The target account ID derived from the
           authentication block values. The target account exists only if the environment
           currently has an authorization block.
-    :attr datetime modified_at: A date and time value in the format
+    :param datetime modified_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str href: A URL.
-    :attr EnvironmentDefinitionRequiredPropertiesResponse definition: The
+    :param str href: A URL.
+    :param EnvironmentDefinitionRequiredPropertiesResponse definition: The
           environment definition.
     """
 
     def __init__(
         self,
         id: str,
         project: 'ProjectReference',
         created_at: datetime,
         modified_at: datetime,
         href: str,
         definition: 'EnvironmentDefinitionRequiredPropertiesResponse',
         *,
-        target_account: str = None,
+        target_account: Optional[str] = None,
     ) -> None:
         """
         Initialize a Environment object.
 
         :param str id: The environment ID as a friendly name.
         :param ProjectReference project: The project that is referenced by this
                resource.
@@ -2789,38 +3022,38 @@
         self.href = href
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'Environment':
         """Initialize a Environment object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in Environment JSON')
-        if 'project' in _dict:
-            args['project'] = ProjectReference.from_dict(_dict.get('project'))
+        if (project := _dict.get('project')) is not None:
+            args['project'] = ProjectReference.from_dict(project)
         else:
             raise ValueError('Required property \'project\' not present in Environment JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in Environment JSON')
-        if 'target_account' in _dict:
-            args['target_account'] = _dict.get('target_account')
-        if 'modified_at' in _dict:
-            args['modified_at'] = string_to_datetime(_dict.get('modified_at'))
+        if (target_account := _dict.get('target_account')) is not None:
+            args['target_account'] = target_account
+        if (modified_at := _dict.get('modified_at')) is not None:
+            args['modified_at'] = string_to_datetime(modified_at)
         else:
             raise ValueError('Required property \'modified_at\' not present in Environment JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in Environment JSON')
-        if 'definition' in _dict:
-            args['definition'] = EnvironmentDefinitionRequiredPropertiesResponse.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = EnvironmentDefinitionRequiredPropertiesResponse.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in Environment JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Environment object from a json dictionary."""
@@ -2870,27 +3103,27 @@
         return not self == other
 
 
 class EnvironmentCollection:
     """
     The list environment response.
 
-    :attr int limit: A pagination limit.
-    :attr PaginationLink first: A pagination link.
-    :attr PaginationLink next: (optional) A pagination link.
-    :attr List[Environment] environments: (optional) The environment.
+    :param int limit: A pagination limit.
+    :param PaginationLink first: A pagination link.
+    :param PaginationLink next: (optional) A pagination link.
+    :param List[Environment] environments: (optional) The environment.
     """
 
     def __init__(
         self,
         limit: int,
         first: 'PaginationLink',
         *,
-        next: 'PaginationLink' = None,
-        environments: List['Environment'] = None,
+        next: Optional['PaginationLink'] = None,
+        environments: Optional[List['Environment']] = None,
     ) -> None:
         """
         Initialize a EnvironmentCollection object.
 
         :param int limit: A pagination limit.
         :param PaginationLink first: A pagination link.
         :param PaginationLink next: (optional) A pagination link.
@@ -2901,26 +3134,26 @@
         self.next = next
         self.environments = environments
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentCollection':
         """Initialize a EnvironmentCollection object from a json dictionary."""
         args = {}
-        if 'limit' in _dict:
-            args['limit'] = _dict.get('limit')
+        if (limit := _dict.get('limit')) is not None:
+            args['limit'] = limit
         else:
             raise ValueError('Required property \'limit\' not present in EnvironmentCollection JSON')
-        if 'first' in _dict:
-            args['first'] = PaginationLink.from_dict(_dict.get('first'))
+        if (first := _dict.get('first')) is not None:
+            args['first'] = PaginationLink.from_dict(first)
         else:
             raise ValueError('Required property \'first\' not present in EnvironmentCollection JSON')
-        if 'next' in _dict:
-            args['next'] = PaginationLink.from_dict(_dict.get('next'))
-        if 'environments' in _dict:
-            args['environments'] = [Environment.from_dict(v) for v in _dict.get('environments')]
+        if (next := _dict.get('next')) is not None:
+            args['next'] = PaginationLink.from_dict(next)
+        if (environments := _dict.get('environments')) is not None:
+            args['environments'] = [Environment.from_dict(v) for v in environments]
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentCollection object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -2968,33 +3201,33 @@
         return not self == other
 
 
 class EnvironmentDefinitionPropertiesPatch:
     """
     The environment definition that is used for updates.
 
-    :attr str description: (optional) The description of the environment.
-    :attr str name: (optional) The name of the environment. It's unique within the
+    :param str description: (optional) The description of the environment.
+    :param str name: (optional) The name of the environment. It's unique within the
           account across projects and regions.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
     """
 
     def __init__(
         self,
         *,
-        description: str = None,
-        name: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        compliance_profile: 'ProjectComplianceProfile' = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
     ) -> None:
         """
         Initialize a EnvironmentDefinitionPropertiesPatch object.
 
         :param str description: (optional) The description of the environment.
         :param str name: (optional) The name of the environment. It's unique within
                the account across projects and regions.
@@ -3012,24 +3245,24 @@
         self.inputs = inputs
         self.compliance_profile = compliance_profile
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentDefinitionPropertiesPatch':
         """Initialize a EnvironmentDefinitionPropertiesPatch object from a json dictionary."""
         args = {}
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentDefinitionPropertiesPatch object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3073,33 +3306,33 @@
         return not self == other
 
 
 class EnvironmentDefinitionRequiredProperties:
     """
     The environment definition.
 
-    :attr str description: (optional) The description of the environment.
-    :attr str name: The name of the environment. It's unique within the account
+    :param str description: (optional) The description of the environment.
+    :param str name: The name of the environment. It's unique within the account
           across projects and regions.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
     """
 
     def __init__(
         self,
         name: str,
         *,
-        description: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        compliance_profile: 'ProjectComplianceProfile' = None,
+        description: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
     ) -> None:
         """
         Initialize a EnvironmentDefinitionRequiredProperties object.
 
         :param str name: The name of the environment. It's unique within the
                account across projects and regions.
         :param str description: (optional) The description of the environment.
@@ -3117,26 +3350,26 @@
         self.inputs = inputs
         self.compliance_profile = compliance_profile
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentDefinitionRequiredProperties':
         """Initialize a EnvironmentDefinitionRequiredProperties object from a json dictionary."""
         args = {}
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in EnvironmentDefinitionRequiredProperties JSON')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentDefinitionRequiredProperties object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3180,33 +3413,33 @@
         return not self == other
 
 
 class EnvironmentDefinitionRequiredPropertiesResponse:
     """
     The environment definition.
 
-    :attr str description: The description of the environment.
-    :attr str name: The name of the environment. It's unique within the account
+    :param str description: The description of the environment.
+    :param str name: The name of the environment. It's unique within the account
           across projects and regions.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
     """
 
     def __init__(
         self,
         description: str,
         name: str,
         *,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        compliance_profile: 'ProjectComplianceProfile' = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
     ) -> None:
         """
         Initialize a EnvironmentDefinitionRequiredPropertiesResponse object.
 
         :param str description: The description of the environment.
         :param str name: The name of the environment. It's unique within the
                account across projects and regions.
@@ -3224,32 +3457,32 @@
         self.inputs = inputs
         self.compliance_profile = compliance_profile
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentDefinitionRequiredPropertiesResponse':
         """Initialize a EnvironmentDefinitionRequiredPropertiesResponse object from a json dictionary."""
         args = {}
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError(
                 'Required property \'description\' not present in EnvironmentDefinitionRequiredPropertiesResponse JSON'
             )
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError(
                 'Required property \'name\' not present in EnvironmentDefinitionRequiredPropertiesResponse JSON'
             )
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentDefinitionRequiredPropertiesResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3293,15 +3526,15 @@
         return not self == other
 
 
 class EnvironmentDeleteResponse:
     """
     The response to a request to delete an environment.
 
-    :attr str id: The environment ID as a friendly name.
+    :param str id: The environment ID as a friendly name.
     """
 
     def __init__(
         self,
         id: str,
     ) -> None:
         """
@@ -3311,16 +3544,16 @@
         """
         self.id = id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentDeleteResponse':
         """Initialize a EnvironmentDeleteResponse object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in EnvironmentDeleteResponse JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentDeleteResponse object from a json dictionary."""
@@ -3352,15 +3585,15 @@
         return not self == other
 
 
 class EnvironmentPrototype:
     """
     The definition of a project environment.
 
-    :attr EnvironmentDefinitionRequiredProperties definition: The environment
+    :param EnvironmentDefinitionRequiredProperties definition: The environment
           definition.
     """
 
     def __init__(
         self,
         definition: 'EnvironmentDefinitionRequiredProperties',
     ) -> None:
@@ -3372,16 +3605,16 @@
         """
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'EnvironmentPrototype':
         """Initialize a EnvironmentPrototype object from a json dictionary."""
         args = {}
-        if 'definition' in _dict:
-            args['definition'] = EnvironmentDefinitionRequiredProperties.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = EnvironmentDefinitionRequiredProperties.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in EnvironmentPrototype JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a EnvironmentPrototype object from a json dictionary."""
@@ -3417,31 +3650,31 @@
 
 
 class LastActionWithSummary:
     """
     The href and results from the last action job that is performed on the project
     configuration.
 
-    :attr str href: A URL.
-    :attr str result: (optional) The result of the last action.
-    :attr ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
-    :attr PrePostActionJobWithIdAndSummary pre_job: (optional) A brief summary of a
-          pre- and post-action.
-    :attr PrePostActionJobWithIdAndSummary post_job: (optional) A brief summary of a
+    :param str href: A URL.
+    :param str result: (optional) The result of the last action.
+    :param ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
+    :param PrePostActionJobWithIdAndSummary pre_job: (optional) A brief summary of a
           pre- and post-action.
+    :param PrePostActionJobWithIdAndSummary post_job: (optional) A brief summary of
+          a pre- and post-action.
     """
 
     def __init__(
         self,
         href: str,
         *,
-        result: str = None,
-        job: 'ActionJobWithIdAndSummary' = None,
-        pre_job: 'PrePostActionJobWithIdAndSummary' = None,
-        post_job: 'PrePostActionJobWithIdAndSummary' = None,
+        result: Optional[str] = None,
+        job: Optional['ActionJobWithIdAndSummary'] = None,
+        pre_job: Optional['PrePostActionJobWithIdAndSummary'] = None,
+        post_job: Optional['PrePostActionJobWithIdAndSummary'] = None,
     ) -> None:
         """
         Initialize a LastActionWithSummary object.
 
         :param str href: A URL.
         :param str result: (optional) The result of the last action.
         :param ActionJobWithIdAndSummary job: (optional) A brief summary of an
@@ -3457,26 +3690,26 @@
         self.pre_job = pre_job
         self.post_job = post_job
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'LastActionWithSummary':
         """Initialize a LastActionWithSummary object from a json dictionary."""
         args = {}
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in LastActionWithSummary JSON')
-        if 'result' in _dict:
-            args['result'] = _dict.get('result')
-        if 'job' in _dict:
-            args['job'] = ActionJobWithIdAndSummary.from_dict(_dict.get('job'))
-        if 'pre_job' in _dict:
-            args['pre_job'] = PrePostActionJobWithIdAndSummary.from_dict(_dict.get('pre_job'))
-        if 'post_job' in _dict:
-            args['post_job'] = PrePostActionJobWithIdAndSummary.from_dict(_dict.get('post_job'))
+        if (result := _dict.get('result')) is not None:
+            args['result'] = result
+        if (job := _dict.get('job')) is not None:
+            args['job'] = ActionJobWithIdAndSummary.from_dict(job)
+        if (pre_job := _dict.get('pre_job')) is not None:
+            args['pre_job'] = PrePostActionJobWithIdAndSummary.from_dict(pre_job)
+        if (post_job := _dict.get('post_job')) is not None:
+            args['post_job'] = PrePostActionJobWithIdAndSummary.from_dict(post_job)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LastActionWithSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3532,36 +3765,36 @@
 
 
 class LastDriftDetectionJobSummary:
     """
     The summary for drift detection jobs that are performed as part of the last monitoring
     action.
 
-    :attr ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
+    :param ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
     """
 
     def __init__(
         self,
         *,
-        job: 'ActionJobWithIdAndSummary' = None,
+        job: Optional['ActionJobWithIdAndSummary'] = None,
     ) -> None:
         """
         Initialize a LastDriftDetectionJobSummary object.
 
         :param ActionJobWithIdAndSummary job: (optional) A brief summary of an
                action.
         """
         self.job = job
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'LastDriftDetectionJobSummary':
         """Initialize a LastDriftDetectionJobSummary object from a json dictionary."""
         args = {}
-        if 'job' in _dict:
-            args['job'] = ActionJobWithIdAndSummary.from_dict(_dict.get('job'))
+        if (job := _dict.get('job')) is not None:
+            args['job'] = ActionJobWithIdAndSummary.from_dict(job)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LastDriftDetectionJobSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3595,26 +3828,26 @@
 
 
 class LastMonitoringActionWithSummary:
     """
     The summary from the last monitoring action job that is performed on the project
     configuration.
 
-    :attr str href: A URL.
-    :attr str result: (optional) The result of the last action.
-    :attr LastDriftDetectionJobSummary drift_detection: (optional) The summary for
+    :param str href: A URL.
+    :param str result: (optional) The result of the last action.
+    :param LastDriftDetectionJobSummary drift_detection: (optional) The summary for
           drift detection jobs that are performed as part of the last monitoring action.
     """
 
     def __init__(
         self,
         href: str,
         *,
-        result: str = None,
-        drift_detection: 'LastDriftDetectionJobSummary' = None,
+        result: Optional[str] = None,
+        drift_detection: Optional['LastDriftDetectionJobSummary'] = None,
     ) -> None:
         """
         Initialize a LastMonitoringActionWithSummary object.
 
         :param str href: A URL.
         :param str result: (optional) The result of the last action.
         :param LastDriftDetectionJobSummary drift_detection: (optional) The summary
@@ -3625,22 +3858,22 @@
         self.result = result
         self.drift_detection = drift_detection
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'LastMonitoringActionWithSummary':
         """Initialize a LastMonitoringActionWithSummary object from a json dictionary."""
         args = {}
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in LastMonitoringActionWithSummary JSON')
-        if 'result' in _dict:
-            args['result'] = _dict.get('result')
-        if 'drift_detection' in _dict:
-            args['drift_detection'] = LastDriftDetectionJobSummary.from_dict(_dict.get('drift_detection'))
+        if (result := _dict.get('result')) is not None:
+            args['result'] = result
+        if (drift_detection := _dict.get('drift_detection')) is not None:
+            args['drift_detection'] = LastDriftDetectionJobSummary.from_dict(drift_detection)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LastMonitoringActionWithSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3686,40 +3919,40 @@
 
 
 class LastValidatedActionWithSummary:
     """
     The href and results from the last action job that is performed on the project
     configuration.
 
-    :attr str href: A URL.
-    :attr str result: (optional) The result of the last action.
-    :attr ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
-    :attr PrePostActionJobWithIdAndSummary pre_job: (optional) A brief summary of a
-          pre- and post-action.
-    :attr PrePostActionJobWithIdAndSummary post_job: (optional) A brief summary of a
+    :param str href: A URL.
+    :param str result: (optional) The result of the last action.
+    :param ActionJobWithIdAndSummary job: (optional) A brief summary of an action.
+    :param PrePostActionJobWithIdAndSummary pre_job: (optional) A brief summary of a
           pre- and post-action.
-    :attr ProjectConfigMetadataCostEstimate cost_estimate: (optional) The cost
+    :param PrePostActionJobWithIdAndSummary post_job: (optional) A brief summary of
+          a pre- and post-action.
+    :param ProjectConfigMetadataCostEstimate cost_estimate: (optional) The cost
           estimate of the configuration.
           This property exists only after the first configuration validation.
-    :attr ProjectConfigMetadataCodeRiskAnalyzerLogs cra_logs: (optional) The Code
+    :param ProjectConfigMetadataCodeRiskAnalyzerLogs cra_logs: (optional) The Code
           Risk Analyzer logs of the configuration. This property is populated only after
           the validation step when the Code Risk Analyzer is run. Note: `cra` is the
           abbreviated form of Code Risk Analyzer.
     """
 
     def __init__(
         self,
         href: str,
         *,
-        result: str = None,
-        job: 'ActionJobWithIdAndSummary' = None,
-        pre_job: 'PrePostActionJobWithIdAndSummary' = None,
-        post_job: 'PrePostActionJobWithIdAndSummary' = None,
-        cost_estimate: 'ProjectConfigMetadataCostEstimate' = None,
-        cra_logs: 'ProjectConfigMetadataCodeRiskAnalyzerLogs' = None,
+        result: Optional[str] = None,
+        job: Optional['ActionJobWithIdAndSummary'] = None,
+        pre_job: Optional['PrePostActionJobWithIdAndSummary'] = None,
+        post_job: Optional['PrePostActionJobWithIdAndSummary'] = None,
+        cost_estimate: Optional['ProjectConfigMetadataCostEstimate'] = None,
+        cra_logs: Optional['ProjectConfigMetadataCodeRiskAnalyzerLogs'] = None,
     ) -> None:
         """
         Initialize a LastValidatedActionWithSummary object.
 
         :param str href: A URL.
         :param str result: (optional) The result of the last action.
         :param ActionJobWithIdAndSummary job: (optional) A brief summary of an
@@ -3744,30 +3977,30 @@
         self.cost_estimate = cost_estimate
         self.cra_logs = cra_logs
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'LastValidatedActionWithSummary':
         """Initialize a LastValidatedActionWithSummary object from a json dictionary."""
         args = {}
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in LastValidatedActionWithSummary JSON')
-        if 'result' in _dict:
-            args['result'] = _dict.get('result')
-        if 'job' in _dict:
-            args['job'] = ActionJobWithIdAndSummary.from_dict(_dict.get('job'))
-        if 'pre_job' in _dict:
-            args['pre_job'] = PrePostActionJobWithIdAndSummary.from_dict(_dict.get('pre_job'))
-        if 'post_job' in _dict:
-            args['post_job'] = PrePostActionJobWithIdAndSummary.from_dict(_dict.get('post_job'))
-        if 'cost_estimate' in _dict:
-            args['cost_estimate'] = ProjectConfigMetadataCostEstimate.from_dict(_dict.get('cost_estimate'))
-        if 'cra_logs' in _dict:
-            args['cra_logs'] = _dict.get('cra_logs')
+        if (result := _dict.get('result')) is not None:
+            args['result'] = result
+        if (job := _dict.get('job')) is not None:
+            args['job'] = ActionJobWithIdAndSummary.from_dict(job)
+        if (pre_job := _dict.get('pre_job')) is not None:
+            args['pre_job'] = PrePostActionJobWithIdAndSummary.from_dict(pre_job)
+        if (post_job := _dict.get('post_job')) is not None:
+            args['post_job'] = PrePostActionJobWithIdAndSummary.from_dict(post_job)
+        if (cost_estimate := _dict.get('cost_estimate')) is not None:
+            args['cost_estimate'] = ProjectConfigMetadataCostEstimate.from_dict(cost_estimate)
+        if (cra_logs := _dict.get('cra_logs')) is not None:
+            args['cra_logs'] = cra_logs
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a LastValidatedActionWithSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3832,26 +4065,26 @@
         PASSED = 'passed'
 
 
 class OutputValue:
     """
     OutputValue.
 
-    :attr str name: The variable name.
-    :attr str description: (optional) A short explanation of the output value.
-    :attr object value: (optional) This property can be any value - a string,
+    :param str name: The variable name.
+    :param str description: (optional) A short explanation of the output value.
+    :param object value: (optional) This property can be any value - a string,
           number, boolean, array, or object.
     """
 
     def __init__(
         self,
         name: str,
         *,
-        description: str = None,
-        value: object = None,
+        description: Optional[str] = None,
+        value: Optional[object] = None,
     ) -> None:
         """
         Initialize a OutputValue object.
 
         :param str name: The variable name.
         :param str description: (optional) A short explanation of the output value.
         :param object value: (optional) This property can be any value - a string,
@@ -3861,22 +4094,22 @@
         self.description = description
         self.value = value
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'OutputValue':
         """Initialize a OutputValue object from a json dictionary."""
         args = {}
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in OutputValue JSON')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'value' in _dict:
-            args['value'] = _dict.get('value')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (value := _dict.get('value')) is not None:
+            args['value'] = value
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a OutputValue object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -3910,15 +4143,15 @@
         return not self == other
 
 
 class PaginationLink:
     """
     A pagination link.
 
-    :attr str href: A URL.
+    :param str href: A URL.
     """
 
     def __init__(
         self,
         href: str,
     ) -> None:
         """
@@ -3928,16 +4161,16 @@
         """
         self.href = href
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'PaginationLink':
         """Initialize a PaginationLink object from a json dictionary."""
         args = {}
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in PaginationLink JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a PaginationLink object from a json dictionary."""
@@ -3970,43 +4203,43 @@
 
 
 class PrePostActionJobSummary:
     """
     A brief summary of a pre- and post-action job. This property is populated only after
     an action is run as part of a validation, deployment, or undeployment.
 
-    :attr str job_id: The ID of the Schematics action job that ran as part of the
+    :param str job_id: The ID of the Schematics action job that ran as part of the
           pre- and post-job.
-    :attr datetime start_time: (optional) A date and time value in the format
+    :param datetime start_time: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr datetime end_time: (optional) A date and time value in the format
+    :param datetime end_time: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr int tasks: (optional) The number of tasks that were run in the job.
-    :attr int ok: (optional) The number of tasks that successfully ran in the job.
-    :attr int failed: (optional) The number of tasks that failed in the job.
-    :attr int skipped: (optional) The number of tasks that were skipped in the job.
-    :attr int changed: (optional) The number of tasks that were changed in the job.
-    :attr PrePostActionJobSystemError project_error: (optional) A system-level error
-          from the pipeline that ran for this specific pre- and post-job.
+    :param int tasks: (optional) The number of tasks that were run in the job.
+    :param int ok: (optional) The number of tasks that successfully ran in the job.
+    :param int failed: (optional) The number of tasks that failed in the job.
+    :param int skipped: (optional) The number of tasks that were skipped in the job.
+    :param int changed: (optional) The number of tasks that were changed in the job.
+    :param PrePostActionJobSystemError project_error: (optional) A system-level
+          error from the pipeline that ran for this specific pre- and post-job.
     """
 
     def __init__(
         self,
         job_id: str,
         *,
-        start_time: datetime = None,
-        end_time: datetime = None,
-        tasks: int = None,
-        ok: int = None,
-        failed: int = None,
-        skipped: int = None,
-        changed: int = None,
-        project_error: 'PrePostActionJobSystemError' = None,
+        start_time: Optional[datetime] = None,
+        end_time: Optional[datetime] = None,
+        tasks: Optional[int] = None,
+        ok: Optional[int] = None,
+        failed: Optional[int] = None,
+        skipped: Optional[int] = None,
+        changed: Optional[int] = None,
+        project_error: Optional['PrePostActionJobSystemError'] = None,
     ) -> None:
         """
         Initialize a PrePostActionJobSummary object.
 
         :param str job_id: The ID of the Schematics action job that ran as part of
                the pre- and post-job.
         :param datetime start_time: (optional) A date and time value in the format
@@ -4036,34 +4269,34 @@
         self.changed = changed
         self.project_error = project_error
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'PrePostActionJobSummary':
         """Initialize a PrePostActionJobSummary object from a json dictionary."""
         args = {}
-        if 'job_id' in _dict:
-            args['job_id'] = _dict.get('job_id')
+        if (job_id := _dict.get('job_id')) is not None:
+            args['job_id'] = job_id
         else:
             raise ValueError('Required property \'job_id\' not present in PrePostActionJobSummary JSON')
-        if 'start_time' in _dict:
-            args['start_time'] = string_to_datetime(_dict.get('start_time'))
-        if 'end_time' in _dict:
-            args['end_time'] = string_to_datetime(_dict.get('end_time'))
-        if 'tasks' in _dict:
-            args['tasks'] = _dict.get('tasks')
-        if 'ok' in _dict:
-            args['ok'] = _dict.get('ok')
-        if 'failed' in _dict:
-            args['failed'] = _dict.get('failed')
-        if 'skipped' in _dict:
-            args['skipped'] = _dict.get('skipped')
-        if 'changed' in _dict:
-            args['changed'] = _dict.get('changed')
-        if 'project_error' in _dict:
-            args['project_error'] = PrePostActionJobSystemError.from_dict(_dict.get('project_error'))
+        if (start_time := _dict.get('start_time')) is not None:
+            args['start_time'] = string_to_datetime(start_time)
+        if (end_time := _dict.get('end_time')) is not None:
+            args['end_time'] = string_to_datetime(end_time)
+        if (tasks := _dict.get('tasks')) is not None:
+            args['tasks'] = tasks
+        if (ok := _dict.get('ok')) is not None:
+            args['ok'] = ok
+        if (failed := _dict.get('failed')) is not None:
+            args['failed'] = failed
+        if (skipped := _dict.get('skipped')) is not None:
+            args['skipped'] = skipped
+        if (changed := _dict.get('changed')) is not None:
+            args['changed'] = changed
+        if (project_error := _dict.get('project_error')) is not None:
+            args['project_error'] = PrePostActionJobSystemError.from_dict(project_error)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a PrePostActionJobSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -4113,32 +4346,33 @@
 
 
 class PrePostActionJobSystemError:
     """
     The system-level error that OS captured in the project pipelines for the pre- and
     post-job.
 
-    :attr datetime timestamp: A date and time value in the format
+    :param datetime timestamp: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str user_id: The ID of the user that triggered the pipeline that ran the
+    :param str user_id: The ID of the user that triggered the pipeline that ran the
           pre- and post-job.
-    :attr str status_code: The HTTP status code for the error.
-    :attr str description: The summary description of the error.
-    :attr str error_response: (optional) The detailed message from the source error.
+    :param str status_code: The HTTP status code for the error.
+    :param str description: The summary description of the error.
+    :param str error_response: (optional) The detailed message from the source
+          error.
     """
 
     def __init__(
         self,
         timestamp: datetime,
         user_id: str,
         status_code: str,
         description: str,
         *,
-        error_response: str = None,
+        error_response: Optional[str] = None,
     ) -> None:
         """
         Initialize a PrePostActionJobSystemError object.
 
         :param datetime timestamp: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
@@ -4155,32 +4389,32 @@
         self.description = description
         self.error_response = error_response
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'PrePostActionJobSystemError':
         """Initialize a PrePostActionJobSystemError object from a json dictionary."""
         args = {}
-        if 'timestamp' in _dict:
-            args['timestamp'] = string_to_datetime(_dict.get('timestamp'))
+        if (timestamp := _dict.get('timestamp')) is not None:
+            args['timestamp'] = string_to_datetime(timestamp)
         else:
             raise ValueError('Required property \'timestamp\' not present in PrePostActionJobSystemError JSON')
-        if 'user_id' in _dict:
-            args['user_id'] = _dict.get('user_id')
+        if (user_id := _dict.get('user_id')) is not None:
+            args['user_id'] = user_id
         else:
             raise ValueError('Required property \'user_id\' not present in PrePostActionJobSystemError JSON')
-        if 'status_code' in _dict:
-            args['status_code'] = _dict.get('status_code')
+        if (status_code := _dict.get('status_code')) is not None:
+            args['status_code'] = status_code
         else:
             raise ValueError('Required property \'status_code\' not present in PrePostActionJobSystemError JSON')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError('Required property \'description\' not present in PrePostActionJobSystemError JSON')
-        if 'error_response' in _dict:
-            args['error_response'] = _dict.get('error_response')
+        if (error_response := _dict.get('error_response')) is not None:
+            args['error_response'] = error_response
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a PrePostActionJobSystemError object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -4218,18 +4452,18 @@
         return not self == other
 
 
 class PrePostActionJobWithIdAndSummary:
     """
     A brief summary of a pre- and post-action.
 
-    :attr str id: The unique ID.
-    :attr PrePostActionJobSummary summary: A brief summary of a pre- and post-action
-          job. This property is populated only after an action is run as part of a
-          validation, deployment, or undeployment.
+    :param str id: The unique ID.
+    :param PrePostActionJobSummary summary: A brief summary of a pre- and
+          post-action job. This property is populated only after an action is run as part
+          of a validation, deployment, or undeployment.
     """
 
     def __init__(
         self,
         id: str,
         summary: 'PrePostActionJobSummary',
     ) -> None:
@@ -4244,20 +4478,20 @@
         self.id = id
         self.summary = summary
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'PrePostActionJobWithIdAndSummary':
         """Initialize a PrePostActionJobWithIdAndSummary object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in PrePostActionJobWithIdAndSummary JSON')
-        if 'summary' in _dict:
-            args['summary'] = PrePostActionJobSummary.from_dict(_dict.get('summary'))
+        if (summary := _dict.get('summary')) is not None:
+            args['summary'] = PrePostActionJobSummary.from_dict(summary)
         else:
             raise ValueError('Required property \'summary\' not present in PrePostActionJobWithIdAndSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a PrePostActionJobWithIdAndSummary object from a json dictionary."""
@@ -4294,42 +4528,42 @@
         return not self == other
 
 
 class Project:
     """
     The standard schema of a project.
 
-    :attr str crn: An IBM Cloud resource name that uniquely identifies a resource.
-    :attr datetime created_at: A date and time value in the format
+    :param str crn: An IBM Cloud resource name that uniquely identifies a resource.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr List[CumulativeNeedsAttention] cumulative_needs_attention_view: The
+    :param List[CumulativeNeedsAttention] cumulative_needs_attention_view: The
           cumulative list of needs attention items for a project. If the view is
           successfully retrieved, an empty or nonempty array is returned.
-    :attr bool cumulative_needs_attention_view_error: (optional) A value of `true`
+    :param bool cumulative_needs_attention_view_error: (optional) A value of `true`
           indicates that the fetch of the needs attention items failed. This property only
           exists if there was an error when you retrieved the cumulative needs attention
           view.
-    :attr str id: The unique project ID.
-    :attr str location: The IBM Cloud location where a resource is deployed.
-    :attr str resource_group_id: The resource group ID where the project's data and
+    :param str id: The unique project ID.
+    :param str location: The IBM Cloud location where a resource is deployed.
+    :param str resource_group_id: The resource group ID where the project's data and
           tools are created.
-    :attr str state: The project status value.
-    :attr str href: A URL.
-    :attr str resource_group: The resource group name where the project's data and
+    :param str state: The project status value.
+    :param str href: A URL.
+    :param str resource_group: The resource group name where the project's data and
           tools are created.
-    :attr str event_notifications_crn: (optional) The CRN of the Event Notifications
-          instance if one is connected to this project.
-    :attr List[ProjectConfigSummary] configs: The project configurations. These
+    :param str event_notifications_crn: (optional) The CRN of the Event
+          Notifications instance if one is connected to this project.
+    :param List[ProjectConfigSummary] configs: The project configurations. These
           configurations are only included in the response of creating a project if a
           configuration array is specified in the request payload.
-    :attr List[ProjectEnvironmentSummary] environments: The project environment.
+    :param List[ProjectEnvironmentSummary] environments: The project environment.
           These environments are only included in the response if project environments
           were created on the project.
-    :attr ProjectDefinitionProperties definition: The definition of the project.
+    :param ProjectDefinitionProperties definition: The definition of the project.
     """
 
     def __init__(
         self,
         crn: str,
         created_at: datetime,
         cumulative_needs_attention_view: List['CumulativeNeedsAttention'],
@@ -4339,16 +4573,16 @@
         state: str,
         href: str,
         resource_group: str,
         configs: List['ProjectConfigSummary'],
         environments: List['ProjectEnvironmentSummary'],
         definition: 'ProjectDefinitionProperties',
         *,
-        cumulative_needs_attention_view_error: bool = None,
-        event_notifications_crn: str = None,
+        cumulative_needs_attention_view_error: Optional[bool] = None,
+        event_notifications_crn: Optional[str] = None,
     ) -> None:
         """
         Initialize a Project object.
 
         :param str crn: An IBM Cloud resource name that uniquely identifies a
                resource.
         :param datetime created_at: A date and time value in the format
@@ -4395,66 +4629,66 @@
         self.environments = environments
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'Project':
         """Initialize a Project object from a json dictionary."""
         args = {}
-        if 'crn' in _dict:
-            args['crn'] = _dict.get('crn')
+        if (crn := _dict.get('crn')) is not None:
+            args['crn'] = crn
         else:
             raise ValueError('Required property \'crn\' not present in Project JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in Project JSON')
-        if 'cumulative_needs_attention_view' in _dict:
+        if (cumulative_needs_attention_view := _dict.get('cumulative_needs_attention_view')) is not None:
             args['cumulative_needs_attention_view'] = [
-                CumulativeNeedsAttention.from_dict(v) for v in _dict.get('cumulative_needs_attention_view')
+                CumulativeNeedsAttention.from_dict(v) for v in cumulative_needs_attention_view
             ]
         else:
             raise ValueError('Required property \'cumulative_needs_attention_view\' not present in Project JSON')
-        if 'cumulative_needs_attention_view_error' in _dict:
-            args['cumulative_needs_attention_view_error'] = _dict.get('cumulative_needs_attention_view_error')
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (cumulative_needs_attention_view_error := _dict.get('cumulative_needs_attention_view_error')) is not None:
+            args['cumulative_needs_attention_view_error'] = cumulative_needs_attention_view_error
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in Project JSON')
-        if 'location' in _dict:
-            args['location'] = _dict.get('location')
+        if (location := _dict.get('location')) is not None:
+            args['location'] = location
         else:
             raise ValueError('Required property \'location\' not present in Project JSON')
-        if 'resource_group_id' in _dict:
-            args['resource_group_id'] = _dict.get('resource_group_id')
+        if (resource_group_id := _dict.get('resource_group_id')) is not None:
+            args['resource_group_id'] = resource_group_id
         else:
             raise ValueError('Required property \'resource_group_id\' not present in Project JSON')
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in Project JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in Project JSON')
-        if 'resource_group' in _dict:
-            args['resource_group'] = _dict.get('resource_group')
+        if (resource_group := _dict.get('resource_group')) is not None:
+            args['resource_group'] = resource_group
         else:
             raise ValueError('Required property \'resource_group\' not present in Project JSON')
-        if 'event_notifications_crn' in _dict:
-            args['event_notifications_crn'] = _dict.get('event_notifications_crn')
-        if 'configs' in _dict:
-            args['configs'] = [ProjectConfigSummary.from_dict(v) for v in _dict.get('configs')]
+        if (event_notifications_crn := _dict.get('event_notifications_crn')) is not None:
+            args['event_notifications_crn'] = event_notifications_crn
+        if (configs := _dict.get('configs')) is not None:
+            args['configs'] = [ProjectConfigSummary.from_dict(v) for v in configs]
         else:
             raise ValueError('Required property \'configs\' not present in Project JSON')
-        if 'environments' in _dict:
-            args['environments'] = [ProjectEnvironmentSummary.from_dict(v) for v in _dict.get('environments')]
+        if (environments := _dict.get('environments')) is not None:
+            args['environments'] = [ProjectEnvironmentSummary.from_dict(v) for v in environments]
         else:
             raise ValueError('Required property \'environments\' not present in Project JSON')
-        if 'definition' in _dict:
-            args['definition'] = ProjectDefinitionProperties.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectDefinitionProperties.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in Project JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Project object from a json dictionary."""
@@ -4545,27 +4779,27 @@
         DELETING_FAILED = 'deleting_failed'
 
 
 class ProjectCollection:
     """
     Projects list.
 
-    :attr int limit: A pagination limit.
-    :attr PaginationLink first: A pagination link.
-    :attr PaginationLink next: (optional) A pagination link.
-    :attr List[ProjectSummary] projects: (optional) An array of projects.
+    :param int limit: A pagination limit.
+    :param PaginationLink first: A pagination link.
+    :param PaginationLink next: (optional) A pagination link.
+    :param List[ProjectSummary] projects: (optional) An array of projects.
     """
 
     def __init__(
         self,
         limit: int,
         first: 'PaginationLink',
         *,
-        next: 'PaginationLink' = None,
-        projects: List['ProjectSummary'] = None,
+        next: Optional['PaginationLink'] = None,
+        projects: Optional[List['ProjectSummary']] = None,
     ) -> None:
         """
         Initialize a ProjectCollection object.
 
         :param int limit: A pagination limit.
         :param PaginationLink first: A pagination link.
         :param PaginationLink next: (optional) A pagination link.
@@ -4576,26 +4810,26 @@
         self.next = next
         self.projects = projects
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectCollection':
         """Initialize a ProjectCollection object from a json dictionary."""
         args = {}
-        if 'limit' in _dict:
-            args['limit'] = _dict.get('limit')
+        if (limit := _dict.get('limit')) is not None:
+            args['limit'] = limit
         else:
             raise ValueError('Required property \'limit\' not present in ProjectCollection JSON')
-        if 'first' in _dict:
-            args['first'] = PaginationLink.from_dict(_dict.get('first'))
+        if (first := _dict.get('first')) is not None:
+            args['first'] = PaginationLink.from_dict(first)
         else:
             raise ValueError('Required property \'first\' not present in ProjectCollection JSON')
-        if 'next' in _dict:
-            args['next'] = PaginationLink.from_dict(_dict.get('next'))
-        if 'projects' in _dict:
-            args['projects'] = [ProjectSummary.from_dict(v) for v in _dict.get('projects')]
+        if (next := _dict.get('next')) is not None:
+            args['next'] = PaginationLink.from_dict(next)
+        if (projects := _dict.get('projects')) is not None:
+            args['projects'] = [ProjectSummary.from_dict(v) for v in projects]
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectCollection object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -4643,31 +4877,32 @@
         return not self == other
 
 
 class ProjectComplianceProfile:
     """
     The profile that is required for compliance.
 
-    :attr str id: (optional) The unique ID for the compliance profile.
-    :attr str instance_id: (optional) A unique ID for the instance of a compliance
+    :param str id: (optional) The unique ID for the compliance profile.
+    :param str instance_id: (optional) A unique ID for the instance of a compliance
           profile.
-    :attr str instance_location: (optional) The location of the compliance instance.
-    :attr str attachment_id: (optional) A unique ID for the attachment to a
+    :param str instance_location: (optional) The location of the compliance
+          instance.
+    :param str attachment_id: (optional) A unique ID for the attachment to a
           compliance profile.
-    :attr str profile_name: (optional) The name of the compliance profile.
+    :param str profile_name: (optional) The name of the compliance profile.
     """
 
     def __init__(
         self,
         *,
-        id: str = None,
-        instance_id: str = None,
-        instance_location: str = None,
-        attachment_id: str = None,
-        profile_name: str = None,
+        id: Optional[str] = None,
+        instance_id: Optional[str] = None,
+        instance_location: Optional[str] = None,
+        attachment_id: Optional[str] = None,
+        profile_name: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectComplianceProfile object.
 
         :param str id: (optional) The unique ID for the compliance profile.
         :param str instance_id: (optional) A unique ID for the instance of a
                compliance profile.
@@ -4683,24 +4918,24 @@
         self.attachment_id = attachment_id
         self.profile_name = profile_name
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectComplianceProfile':
         """Initialize a ProjectComplianceProfile object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
-        if 'instance_id' in _dict:
-            args['instance_id'] = _dict.get('instance_id')
-        if 'instance_location' in _dict:
-            args['instance_location'] = _dict.get('instance_location')
-        if 'attachment_id' in _dict:
-            args['attachment_id'] = _dict.get('attachment_id')
-        if 'profile_name' in _dict:
-            args['profile_name'] = _dict.get('profile_name')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
+        if (instance_id := _dict.get('instance_id')) is not None:
+            args['instance_id'] = instance_id
+        if (instance_location := _dict.get('instance_location')) is not None:
+            args['instance_location'] = instance_location
+        if (attachment_id := _dict.get('attachment_id')) is not None:
+            args['attachment_id'] = attachment_id
+        if (profile_name := _dict.get('profile_name')) is not None:
+            args['profile_name'] = profile_name
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectComplianceProfile object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -4738,94 +4973,97 @@
         return not self == other
 
 
 class ProjectConfig:
     """
     The standard schema of a project configuration.
 
-    :attr str id: The ID of the configuration. If this parameter is empty, an ID is
+    :param str id: The ID of the configuration. If this parameter is empty, an ID is
           automatically created for the configuration.
-    :attr int version: The version of the configuration.
-    :attr bool is_draft: The flag that indicates whether the version of the
+    :param int version: The version of the configuration.
+    :param bool is_draft: The flag that indicates whether the version of the
           configuration is draft, or active.
-    :attr List[object] needs_attention_state: The needs attention state of a
-          configuration.
-    :attr datetime created_at: A date and time value in the format
+    :param List[ProjectConfigNeedsAttentionState] needs_attention_state: The needs
+          attention state of a configuration.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr datetime modified_at: A date and time value in the format
+    :param datetime modified_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr ProjectConfigMetadataLastApproved last_approved: (optional) The last
+    :param ProjectConfigMetadataLastApproved last_approved: (optional) The last
           approved metadata of the configuration.
-    :attr datetime last_saved_at: (optional) A date and time value in the format
+    :param datetime last_saved_at: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr LastValidatedActionWithSummary last_validated: (optional) The href and
+    :param LastValidatedActionWithSummary last_validated: (optional) The href and
           results from the last action job that is performed on the project configuration.
-    :attr LastActionWithSummary last_deployed: (optional) The href and results from
+    :param LastActionWithSummary last_deployed: (optional) The href and results from
           the last action job that is performed on the project configuration.
-    :attr LastActionWithSummary last_undeployed: (optional) The href and results
+    :param LastActionWithSummary last_undeployed: (optional) The href and results
           from the last action job that is performed on the project configuration.
-    :attr LastMonitoringActionWithSummary last_monitoring: (optional) The summary
+    :param LastMonitoringActionWithSummary last_monitoring: (optional) The summary
           from the last monitoring action job that is performed on the project
           configuration.
-    :attr List[OutputValue] outputs: The outputs of a Schematics template property.
-    :attr ProjectReference project: The project that is referenced by this resource.
-    :attr dict references: (optional) The references that are used in the
+    :param List[OutputValue] outputs: The outputs of a Schematics template property.
+    :param ProjectReference project: The project that is referenced by this
+          resource.
+    :param dict references: (optional) The references that are used in the
           configuration to resolve input values.
-    :attr SchematicsMetadata schematics: (optional) A Schematics workspace that is
+    :param SchematicsMetadata schematics: (optional) A Schematics workspace that is
           associated to a project configuration, with scripts.
-    :attr str state: The state of the configuration.
-    :attr bool update_available: (optional) The flag that indicates whether a
+    :param str state: The state of the configuration.
+    :param bool update_available: (optional) The flag that indicates whether a
           configuration update is available.
-    :attr str href: A URL.
-    :attr ProjectConfigDefinitionResponse definition:
-    :attr ProjectConfigVersionSummary approved_version: (optional) A summary of a
+    :param ProjectObjectReference template: (optional) The template reference.
+    :param str href: A URL.
+    :param ProjectConfigDefinitionResponse definition:
+    :param ProjectConfigVersionSummary approved_version: (optional) A summary of a
           project configuration version.
-    :attr ProjectConfigVersionSummary deployed_version: (optional) A summary of a
+    :param ProjectConfigVersionSummary deployed_version: (optional) A summary of a
           project configuration version.
     """
 
     def __init__(
         self,
         id: str,
         version: int,
         is_draft: bool,
-        needs_attention_state: List[object],
+        needs_attention_state: List['ProjectConfigNeedsAttentionState'],
         created_at: datetime,
         modified_at: datetime,
         outputs: List['OutputValue'],
         project: 'ProjectReference',
         state: str,
         href: str,
         definition: 'ProjectConfigDefinitionResponse',
         *,
-        last_approved: 'ProjectConfigMetadataLastApproved' = None,
-        last_saved_at: datetime = None,
-        last_validated: 'LastValidatedActionWithSummary' = None,
-        last_deployed: 'LastActionWithSummary' = None,
-        last_undeployed: 'LastActionWithSummary' = None,
-        last_monitoring: 'LastMonitoringActionWithSummary' = None,
-        references: dict = None,
-        schematics: 'SchematicsMetadata' = None,
-        update_available: bool = None,
-        approved_version: 'ProjectConfigVersionSummary' = None,
-        deployed_version: 'ProjectConfigVersionSummary' = None,
+        last_approved: Optional['ProjectConfigMetadataLastApproved'] = None,
+        last_saved_at: Optional[datetime] = None,
+        last_validated: Optional['LastValidatedActionWithSummary'] = None,
+        last_deployed: Optional['LastActionWithSummary'] = None,
+        last_undeployed: Optional['LastActionWithSummary'] = None,
+        last_monitoring: Optional['LastMonitoringActionWithSummary'] = None,
+        references: Optional[dict] = None,
+        schematics: Optional['SchematicsMetadata'] = None,
+        update_available: Optional[bool] = None,
+        template: Optional['ProjectObjectReference'] = None,
+        approved_version: Optional['ProjectConfigVersionSummary'] = None,
+        deployed_version: Optional['ProjectConfigVersionSummary'] = None,
     ) -> None:
         """
         Initialize a ProjectConfig object.
 
         :param str id: The ID of the configuration. If this parameter is empty, an
                ID is automatically created for the configuration.
         :param int version: The version of the configuration.
         :param bool is_draft: The flag that indicates whether the version of the
                configuration is draft, or active.
-        :param List[object] needs_attention_state: The needs attention state of a
-               configuration.
+        :param List[ProjectConfigNeedsAttentionState] needs_attention_state: The
+               needs attention state of a configuration.
         :param datetime created_at: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
         :param datetime modified_at: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
         :param List[OutputValue] outputs: The outputs of a Schematics template
@@ -4853,14 +5091,15 @@
                project configuration.
         :param dict references: (optional) The references that are used in the
                configuration to resolve input values.
         :param SchematicsMetadata schematics: (optional) A Schematics workspace
                that is associated to a project configuration, with scripts.
         :param bool update_available: (optional) The flag that indicates whether a
                configuration update is available.
+        :param ProjectObjectReference template: (optional) The template reference.
         :param ProjectConfigVersionSummary approved_version: (optional) A summary
                of a project configuration version.
         :param ProjectConfigVersionSummary deployed_version: (optional) A summary
                of a project configuration version.
         """
         self.id = id
         self.version = version
@@ -4876,89 +5115,94 @@
         self.last_monitoring = last_monitoring
         self.outputs = outputs
         self.project = project
         self.references = references
         self.schematics = schematics
         self.state = state
         self.update_available = update_available
+        self.template = template
         self.href = href
         self.definition = definition
         self.approved_version = approved_version
         self.deployed_version = deployed_version
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfig':
         """Initialize a ProjectConfig object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectConfig JSON')
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ProjectConfig JSON')
-        if 'is_draft' in _dict:
-            args['is_draft'] = _dict.get('is_draft')
+        if (is_draft := _dict.get('is_draft')) is not None:
+            args['is_draft'] = is_draft
         else:
             raise ValueError('Required property \'is_draft\' not present in ProjectConfig JSON')
-        if 'needs_attention_state' in _dict:
-            args['needs_attention_state'] = _dict.get('needs_attention_state')
+        if (needs_attention_state := _dict.get('needs_attention_state')) is not None:
+            args['needs_attention_state'] = [
+                ProjectConfigNeedsAttentionState.from_dict(v) for v in needs_attention_state
+            ]
         else:
             raise ValueError('Required property \'needs_attention_state\' not present in ProjectConfig JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in ProjectConfig JSON')
-        if 'modified_at' in _dict:
-            args['modified_at'] = string_to_datetime(_dict.get('modified_at'))
+        if (modified_at := _dict.get('modified_at')) is not None:
+            args['modified_at'] = string_to_datetime(modified_at)
         else:
             raise ValueError('Required property \'modified_at\' not present in ProjectConfig JSON')
-        if 'last_approved' in _dict:
-            args['last_approved'] = ProjectConfigMetadataLastApproved.from_dict(_dict.get('last_approved'))
-        if 'last_saved_at' in _dict:
-            args['last_saved_at'] = string_to_datetime(_dict.get('last_saved_at'))
-        if 'last_validated' in _dict:
-            args['last_validated'] = LastValidatedActionWithSummary.from_dict(_dict.get('last_validated'))
-        if 'last_deployed' in _dict:
-            args['last_deployed'] = LastActionWithSummary.from_dict(_dict.get('last_deployed'))
-        if 'last_undeployed' in _dict:
-            args['last_undeployed'] = LastActionWithSummary.from_dict(_dict.get('last_undeployed'))
-        if 'last_monitoring' in _dict:
-            args['last_monitoring'] = LastMonitoringActionWithSummary.from_dict(_dict.get('last_monitoring'))
-        if 'outputs' in _dict:
-            args['outputs'] = [OutputValue.from_dict(v) for v in _dict.get('outputs')]
+        if (last_approved := _dict.get('last_approved')) is not None:
+            args['last_approved'] = ProjectConfigMetadataLastApproved.from_dict(last_approved)
+        if (last_saved_at := _dict.get('last_saved_at')) is not None:
+            args['last_saved_at'] = string_to_datetime(last_saved_at)
+        if (last_validated := _dict.get('last_validated')) is not None:
+            args['last_validated'] = LastValidatedActionWithSummary.from_dict(last_validated)
+        if (last_deployed := _dict.get('last_deployed')) is not None:
+            args['last_deployed'] = LastActionWithSummary.from_dict(last_deployed)
+        if (last_undeployed := _dict.get('last_undeployed')) is not None:
+            args['last_undeployed'] = LastActionWithSummary.from_dict(last_undeployed)
+        if (last_monitoring := _dict.get('last_monitoring')) is not None:
+            args['last_monitoring'] = LastMonitoringActionWithSummary.from_dict(last_monitoring)
+        if (outputs := _dict.get('outputs')) is not None:
+            args['outputs'] = [OutputValue.from_dict(v) for v in outputs]
         else:
             raise ValueError('Required property \'outputs\' not present in ProjectConfig JSON')
-        if 'project' in _dict:
-            args['project'] = ProjectReference.from_dict(_dict.get('project'))
+        if (project := _dict.get('project')) is not None:
+            args['project'] = ProjectReference.from_dict(project)
         else:
             raise ValueError('Required property \'project\' not present in ProjectConfig JSON')
-        if 'references' in _dict:
-            args['references'] = _dict.get('references')
-        if 'schematics' in _dict:
-            args['schematics'] = SchematicsMetadata.from_dict(_dict.get('schematics'))
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (references := _dict.get('references')) is not None:
+            args['references'] = references
+        if (schematics := _dict.get('schematics')) is not None:
+            args['schematics'] = SchematicsMetadata.from_dict(schematics)
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfig JSON')
-        if 'update_available' in _dict:
-            args['update_available'] = _dict.get('update_available')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (update_available := _dict.get('update_available')) is not None:
+            args['update_available'] = update_available
+        if (template := _dict.get('template')) is not None:
+            args['template'] = ProjectObjectReference.from_dict(template)
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfig JSON')
-        if 'definition' in _dict:
-            args['definition'] = _dict.get('definition')
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = definition
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfig JSON')
-        if 'approved_version' in _dict:
-            args['approved_version'] = ProjectConfigVersionSummary.from_dict(_dict.get('approved_version'))
-        if 'deployed_version' in _dict:
-            args['deployed_version'] = ProjectConfigVersionSummary.from_dict(_dict.get('deployed_version'))
+        if (approved_version := _dict.get('approved_version')) is not None:
+            args['approved_version'] = ProjectConfigVersionSummary.from_dict(approved_version)
+        if (deployed_version := _dict.get('deployed_version')) is not None:
+            args['deployed_version'] = ProjectConfigVersionSummary.from_dict(deployed_version)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfig object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -4968,15 +5212,21 @@
         if hasattr(self, 'id') and self.id is not None:
             _dict['id'] = self.id
         if hasattr(self, 'version') and self.version is not None:
             _dict['version'] = self.version
         if hasattr(self, 'is_draft') and self.is_draft is not None:
             _dict['is_draft'] = self.is_draft
         if hasattr(self, 'needs_attention_state') and self.needs_attention_state is not None:
-            _dict['needs_attention_state'] = self.needs_attention_state
+            needs_attention_state_list = []
+            for v in self.needs_attention_state:
+                if isinstance(v, dict):
+                    needs_attention_state_list.append(v)
+                else:
+                    needs_attention_state_list.append(v.to_dict())
+            _dict['needs_attention_state'] = needs_attention_state_list
         if hasattr(self, 'created_at') and self.created_at is not None:
             _dict['created_at'] = datetime_to_string(self.created_at)
         if hasattr(self, 'modified_at') and self.modified_at is not None:
             _dict['modified_at'] = datetime_to_string(self.modified_at)
         if hasattr(self, 'last_approved') and self.last_approved is not None:
             if isinstance(self.last_approved, dict):
                 _dict['last_approved'] = self.last_approved
@@ -5024,14 +5274,19 @@
                 _dict['schematics'] = self.schematics
             else:
                 _dict['schematics'] = self.schematics.to_dict()
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
         if hasattr(self, 'update_available') and self.update_available is not None:
             _dict['update_available'] = self.update_available
+        if hasattr(self, 'template') and self.template is not None:
+            if isinstance(self.template, dict):
+                _dict['template'] = self.template
+            else:
+                _dict['template'] = self.template.to_dict()
         if hasattr(self, 'href') and self.href is not None:
             _dict['href'] = self.href
         if hasattr(self, 'definition') and self.definition is not None:
             if isinstance(self.definition, dict):
                 _dict['definition'] = self.definition
             else:
                 _dict['definition'] = self.definition.to_dict()
@@ -5090,27 +5345,27 @@
 
 
 class ProjectConfigAuth:
     """
     The authorization details. You can authorize by using a trusted profile or an API key
     in Secrets Manager.
 
-    :attr str trusted_profile_id: (optional) The trusted profile ID.
-    :attr str method: (optional) The authorization method. You can authorize by
+    :param str trusted_profile_id: (optional) The trusted profile ID.
+    :param str method: (optional) The authorization method. You can authorize by
           using a trusted profile or an API key in Secrets Manager.
-    :attr str api_key: (optional) The IBM Cloud API Key. It can be either raw or
+    :param str api_key: (optional) The IBM Cloud API Key. It can be either raw or
           pulled from the catalog via a `CRN` or `JSON` blob.
     """
 
     def __init__(
         self,
         *,
-        trusted_profile_id: str = None,
-        method: str = None,
-        api_key: str = None,
+        trusted_profile_id: Optional[str] = None,
+        method: Optional[str] = None,
+        api_key: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigAuth object.
 
         :param str trusted_profile_id: (optional) The trusted profile ID.
         :param str method: (optional) The authorization method. You can authorize
                by using a trusted profile or an API key in Secrets Manager.
@@ -5121,20 +5376,20 @@
         self.method = method
         self.api_key = api_key
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigAuth':
         """Initialize a ProjectConfigAuth object from a json dictionary."""
         args = {}
-        if 'trusted_profile_id' in _dict:
-            args['trusted_profile_id'] = _dict.get('trusted_profile_id')
-        if 'method' in _dict:
-            args['method'] = _dict.get('method')
-        if 'api_key' in _dict:
-            args['api_key'] = _dict.get('api_key')
+        if (trusted_profile_id := _dict.get('trusted_profile_id')) is not None:
+            args['trusted_profile_id'] = trusted_profile_id
+        if (method := _dict.get('method')) is not None:
+            args['method'] = method
+        if (api_key := _dict.get('api_key')) is not None:
+            args['api_key'] = api_key
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigAuth object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5177,29 +5432,29 @@
         TRUSTED_PROFILE = 'trusted_profile'
 
 
 class ProjectConfigCollection:
     """
     The project configuration list.
 
-    :attr int limit: A pagination limit.
-    :attr PaginationLink first: A pagination link.
-    :attr PaginationLink next: (optional) A pagination link.
-    :attr List[ProjectConfigSummary] configs: (optional) The response schema of the
+    :param int limit: A pagination limit.
+    :param PaginationLink first: A pagination link.
+    :param PaginationLink next: (optional) A pagination link.
+    :param List[ProjectConfigSummary] configs: (optional) The response schema of the
           collection list operation that defines the array property with the name
           `configs`.
     """
 
     def __init__(
         self,
         limit: int,
         first: 'PaginationLink',
         *,
-        next: 'PaginationLink' = None,
-        configs: List['ProjectConfigSummary'] = None,
+        next: Optional['PaginationLink'] = None,
+        configs: Optional[List['ProjectConfigSummary']] = None,
     ) -> None:
         """
         Initialize a ProjectConfigCollection object.
 
         :param int limit: A pagination limit.
         :param PaginationLink first: A pagination link.
         :param PaginationLink next: (optional) A pagination link.
@@ -5212,26 +5467,26 @@
         self.next = next
         self.configs = configs
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigCollection':
         """Initialize a ProjectConfigCollection object from a json dictionary."""
         args = {}
-        if 'limit' in _dict:
-            args['limit'] = _dict.get('limit')
+        if (limit := _dict.get('limit')) is not None:
+            args['limit'] = limit
         else:
             raise ValueError('Required property \'limit\' not present in ProjectConfigCollection JSON')
-        if 'first' in _dict:
-            args['first'] = PaginationLink.from_dict(_dict.get('first'))
+        if (first := _dict.get('first')) is not None:
+            args['first'] = PaginationLink.from_dict(first)
         else:
             raise ValueError('Required property \'first\' not present in ProjectConfigCollection JSON')
-        if 'next' in _dict:
-            args['next'] = PaginationLink.from_dict(_dict.get('next'))
-        if 'configs' in _dict:
-            args['configs'] = [ProjectConfigSummary.from_dict(v) for v in _dict.get('configs')]
+        if (next := _dict.get('next')) is not None:
+            args['next'] = PaginationLink.from_dict(next)
+        if (configs := _dict.get('configs')) is not None:
+            args['configs'] = [ProjectConfigSummary.from_dict(v) for v in configs]
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigCollection object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5316,14 +5571,15 @@
         Initialize a ProjectConfigDefinitionPrototype object.
 
         """
         msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
             ", ".join(
                 [
                     'ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype',
+                    'ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties',
                     'ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype',
                 ]
             )
         )
         raise Exception(msg)
 
 
@@ -5341,25 +5597,26 @@
 
         """
         msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
             ", ".join(
                 [
                     'ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse',
                     'ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse',
+                    'ProjectConfigDefinitionResponseStackConfigDefinitionProperties',
                 ]
             )
         )
         raise Exception(msg)
 
 
 class ProjectConfigDelete:
     """
     The ID of the deleted configuration.
 
-    :attr str id: The ID of the deleted project or configuration.
+    :param str id: The ID of the deleted project or configuration.
     """
 
     def __init__(
         self,
         id: str,
     ) -> None:
         """
@@ -5369,16 +5626,16 @@
         """
         self.id = id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDelete':
         """Initialize a ProjectConfigDelete object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectConfigDelete JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDelete object from a json dictionary."""
@@ -5432,49 +5689,49 @@
 
 
 class ProjectConfigMetadataCostEstimate:
     """
     The cost estimate of the configuration. This property exists only after the first
     configuration validation.
 
-    :attr str version: (optional) The version of the cost estimate of the
+    :param str version: (optional) The version of the cost estimate of the
           configuration.
-    :attr str currency: (optional) The currency of the cost estimate of the
+    :param str currency: (optional) The currency of the cost estimate of the
           configuration.
-    :attr str total_hourly_cost: (optional) The total hourly cost estimate of the
+    :param str total_hourly_cost: (optional) The total hourly cost estimate of the
           configuration.
-    :attr str total_monthly_cost: (optional) The total monthly cost estimate of the
+    :param str total_monthly_cost: (optional) The total monthly cost estimate of the
           configuration.
-    :attr str past_total_hourly_cost: (optional) The past total hourly cost estimate
-          of the configuration.
-    :attr str past_total_monthly_cost: (optional) The past total monthly cost
+    :param str past_total_hourly_cost: (optional) The past total hourly cost
+          estimate of the configuration.
+    :param str past_total_monthly_cost: (optional) The past total monthly cost
           estimate of the configuration.
-    :attr str diff_total_hourly_cost: (optional) The difference between the current
+    :param str diff_total_hourly_cost: (optional) The difference between the current
           and past total hourly cost estimates of the configuration.
-    :attr str diff_total_monthly_cost: (optional) The difference between the current
-          and past total monthly cost estimates of the configuration.
-    :attr datetime time_generated: (optional) A date and time value in the format
+    :param str diff_total_monthly_cost: (optional) The difference between the
+          current and past total monthly cost estimates of the configuration.
+    :param datetime time_generated: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str user_id: (optional) The unique ID.
+    :param str user_id: (optional) The unique ID.
     """
 
     def __init__(
         self,
         *,
-        version: str = None,
-        currency: str = None,
-        total_hourly_cost: str = None,
-        total_monthly_cost: str = None,
-        past_total_hourly_cost: str = None,
-        past_total_monthly_cost: str = None,
-        diff_total_hourly_cost: str = None,
-        diff_total_monthly_cost: str = None,
-        time_generated: datetime = None,
-        user_id: str = None,
+        version: Optional[str] = None,
+        currency: Optional[str] = None,
+        total_hourly_cost: Optional[str] = None,
+        total_monthly_cost: Optional[str] = None,
+        past_total_hourly_cost: Optional[str] = None,
+        past_total_monthly_cost: Optional[str] = None,
+        diff_total_hourly_cost: Optional[str] = None,
+        diff_total_monthly_cost: Optional[str] = None,
+        time_generated: Optional[datetime] = None,
+        user_id: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigMetadataCostEstimate object.
 
         :param str version: (optional) The version of the cost estimate of the
                configuration.
         :param str currency: (optional) The currency of the cost estimate of the
@@ -5507,34 +5764,34 @@
         self.time_generated = time_generated
         self.user_id = user_id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigMetadataCostEstimate':
         """Initialize a ProjectConfigMetadataCostEstimate object from a json dictionary."""
         args = {}
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
-        if 'currency' in _dict:
-            args['currency'] = _dict.get('currency')
-        if 'totalHourlyCost' in _dict:
-            args['total_hourly_cost'] = _dict.get('totalHourlyCost')
-        if 'totalMonthlyCost' in _dict:
-            args['total_monthly_cost'] = _dict.get('totalMonthlyCost')
-        if 'pastTotalHourlyCost' in _dict:
-            args['past_total_hourly_cost'] = _dict.get('pastTotalHourlyCost')
-        if 'pastTotalMonthlyCost' in _dict:
-            args['past_total_monthly_cost'] = _dict.get('pastTotalMonthlyCost')
-        if 'diffTotalHourlyCost' in _dict:
-            args['diff_total_hourly_cost'] = _dict.get('diffTotalHourlyCost')
-        if 'diffTotalMonthlyCost' in _dict:
-            args['diff_total_monthly_cost'] = _dict.get('diffTotalMonthlyCost')
-        if 'timeGenerated' in _dict:
-            args['time_generated'] = string_to_datetime(_dict.get('timeGenerated'))
-        if 'user_id' in _dict:
-            args['user_id'] = _dict.get('user_id')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
+        if (currency := _dict.get('currency')) is not None:
+            args['currency'] = currency
+        if (total_hourly_cost := _dict.get('totalHourlyCost')) is not None:
+            args['total_hourly_cost'] = total_hourly_cost
+        if (total_monthly_cost := _dict.get('totalMonthlyCost')) is not None:
+            args['total_monthly_cost'] = total_monthly_cost
+        if (past_total_hourly_cost := _dict.get('pastTotalHourlyCost')) is not None:
+            args['past_total_hourly_cost'] = past_total_hourly_cost
+        if (past_total_monthly_cost := _dict.get('pastTotalMonthlyCost')) is not None:
+            args['past_total_monthly_cost'] = past_total_monthly_cost
+        if (diff_total_hourly_cost := _dict.get('diffTotalHourlyCost')) is not None:
+            args['diff_total_hourly_cost'] = diff_total_hourly_cost
+        if (diff_total_monthly_cost := _dict.get('diffTotalMonthlyCost')) is not None:
+            args['diff_total_monthly_cost'] = diff_total_monthly_cost
+        if (time_generated := _dict.get('timeGenerated')) is not None:
+            args['time_generated'] = string_to_datetime(time_generated)
+        if (user_id := _dict.get('user_id')) is not None:
+            args['user_id'] = user_id
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigMetadataCostEstimate object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5582,31 +5839,31 @@
         return not self == other
 
 
 class ProjectConfigMetadataLastApproved:
     """
     The last approved metadata of the configuration.
 
-    :attr datetime at: A date and time value in the format YYYY-MM-DDTHH:mm:ssZ or
+    :param datetime at: A date and time value in the format YYYY-MM-DDTHH:mm:ssZ or
           YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time format as specified by RFC
           3339.
-    :attr str comment: (optional) The comment that is left by the user who approved
+    :param str comment: (optional) The comment that is left by the user who approved
           the configuration.
-    :attr bool is_forced: The flag that indicates whether the approval was forced
+    :param bool is_forced: The flag that indicates whether the approval was forced
           approved.
-    :attr str user_id: The unique ID.
+    :param str user_id: The unique ID.
     """
 
     def __init__(
         self,
         at: datetime,
         is_forced: bool,
         user_id: str,
         *,
-        comment: str = None,
+        comment: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigMetadataLastApproved object.
 
         :param datetime at: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
@@ -5621,26 +5878,26 @@
         self.is_forced = is_forced
         self.user_id = user_id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigMetadataLastApproved':
         """Initialize a ProjectConfigMetadataLastApproved object from a json dictionary."""
         args = {}
-        if 'at' in _dict:
-            args['at'] = string_to_datetime(_dict.get('at'))
+        if (at := _dict.get('at')) is not None:
+            args['at'] = string_to_datetime(at)
         else:
             raise ValueError('Required property \'at\' not present in ProjectConfigMetadataLastApproved JSON')
-        if 'comment' in _dict:
-            args['comment'] = _dict.get('comment')
-        if 'is_forced' in _dict:
-            args['is_forced'] = _dict.get('is_forced')
+        if (comment := _dict.get('comment')) is not None:
+            args['comment'] = comment
+        if (is_forced := _dict.get('is_forced')) is not None:
+            args['is_forced'] = is_forced
         else:
             raise ValueError('Required property \'is_forced\' not present in ProjectConfigMetadataLastApproved JSON')
-        if 'user_id' in _dict:
-            args['user_id'] = _dict.get('user_id')
+        if (user_id := _dict.get('user_id')) is not None:
+            args['user_id'] = user_id
         else:
             raise ValueError('Required property \'user_id\' not present in ProjectConfigMetadataLastApproved JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigMetadataLastApproved object from a json dictionary."""
@@ -5674,20 +5931,157 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectConfigMetadataLastApproved') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ProjectConfigNeedsAttentionState:
+    """
+    A needs attention state item shown to users is a specific actionable event that occurs
+    during the lifecycle of a configuration.
+
+    :param str event_id: The id of the event.
+    :param str event: The name of the event.
+    :param str severity: (optional) The severity of the event. This is a system
+          generated field. For user triggered events the field is not present.
+    :param str action_url: (optional) An actionable URL that users can access in
+          response to the event. This is a system generated field. For user triggered
+          events the field is not present.
+    :param str target: (optional) The configuration id and version for which the
+          event occurred. This field is only available for user generated events. For
+          system triggered events the field is not present.
+    :param str triggered_by: (optional) The IAM id of the user that triggered the
+          event. This field is only available for user generated events. For system
+          triggered events the field is not present.
+    :param str timestamp: The timestamp of the event.
+    """
+
+    def __init__(
+        self,
+        event_id: str,
+        event: str,
+        timestamp: str,
+        *,
+        severity: Optional[str] = None,
+        action_url: Optional[str] = None,
+        target: Optional[str] = None,
+        triggered_by: Optional[str] = None,
+    ) -> None:
+        """
+        Initialize a ProjectConfigNeedsAttentionState object.
+
+        :param str event_id: The id of the event.
+        :param str event: The name of the event.
+        :param str timestamp: The timestamp of the event.
+        :param str severity: (optional) The severity of the event. This is a system
+               generated field. For user triggered events the field is not present.
+        :param str action_url: (optional) An actionable URL that users can access
+               in response to the event. This is a system generated field. For user
+               triggered events the field is not present.
+        :param str target: (optional) The configuration id and version for which
+               the event occurred. This field is only available for user generated events.
+               For system triggered events the field is not present.
+        :param str triggered_by: (optional) The IAM id of the user that triggered
+               the event. This field is only available for user generated events. For
+               system triggered events the field is not present.
+        """
+        self.event_id = event_id
+        self.event = event
+        self.severity = severity
+        self.action_url = action_url
+        self.target = target
+        self.triggered_by = triggered_by
+        self.timestamp = timestamp
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ProjectConfigNeedsAttentionState':
+        """Initialize a ProjectConfigNeedsAttentionState object from a json dictionary."""
+        args = {}
+        if (event_id := _dict.get('event_id')) is not None:
+            args['event_id'] = event_id
+        else:
+            raise ValueError('Required property \'event_id\' not present in ProjectConfigNeedsAttentionState JSON')
+        if (event := _dict.get('event')) is not None:
+            args['event'] = event
+        else:
+            raise ValueError('Required property \'event\' not present in ProjectConfigNeedsAttentionState JSON')
+        if (severity := _dict.get('severity')) is not None:
+            args['severity'] = severity
+        if (action_url := _dict.get('action_url')) is not None:
+            args['action_url'] = action_url
+        if (target := _dict.get('target')) is not None:
+            args['target'] = target
+        if (triggered_by := _dict.get('triggered_by')) is not None:
+            args['triggered_by'] = triggered_by
+        if (timestamp := _dict.get('timestamp')) is not None:
+            args['timestamp'] = timestamp
+        else:
+            raise ValueError('Required property \'timestamp\' not present in ProjectConfigNeedsAttentionState JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ProjectConfigNeedsAttentionState object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'event_id') and self.event_id is not None:
+            _dict['event_id'] = self.event_id
+        if hasattr(self, 'event') and self.event is not None:
+            _dict['event'] = self.event
+        if hasattr(self, 'severity') and self.severity is not None:
+            _dict['severity'] = self.severity
+        if hasattr(self, 'action_url') and self.action_url is not None:
+            _dict['action_url'] = self.action_url
+        if hasattr(self, 'target') and self.target is not None:
+            _dict['target'] = self.target
+        if hasattr(self, 'triggered_by') and self.triggered_by is not None:
+            _dict['triggered_by'] = self.triggered_by
+        if hasattr(self, 'timestamp') and self.timestamp is not None:
+            _dict['timestamp'] = self.timestamp
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ProjectConfigNeedsAttentionState object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ProjectConfigNeedsAttentionState') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ProjectConfigNeedsAttentionState') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+    class SeverityEnum(str, Enum):
+        """
+        The severity of the event. This is a system generated field. For user triggered
+        events the field is not present.
+        """
+
+        INFO = 'INFO'
+        WARNING = 'WARNING'
+        ERROR = 'ERROR'
+
+
 class ProjectConfigPrototype:
     """
     The input of a project configuration.
 
-    :attr ProjectConfigDefinitionPrototype definition:
-    :attr SchematicsWorkspace schematics: (optional) A Schematics workspace to use
+    :param ProjectConfigDefinitionPrototype definition:
+    :param SchematicsWorkspace schematics: (optional) A Schematics workspace to use
           for deploying this deployable architecture.
           > If you are importing data from an existing Schematics workspace that is not
           backed by cart, then you must provide a `locator_id`. If you are using a
           Schematics workspace that is backed by cart, a `locator_id` is not required
           because the Schematics workspace has one.
           >
           There are 3 scenarios:
@@ -5703,15 +6097,15 @@
           template](/docs/schematics?topic=schematics-sch-create-wks).
     """
 
     def __init__(
         self,
         definition: 'ProjectConfigDefinitionPrototype',
         *,
-        schematics: 'SchematicsWorkspace' = None,
+        schematics: Optional['SchematicsWorkspace'] = None,
     ) -> None:
         """
         Initialize a ProjectConfigPrototype object.
 
         :param ProjectConfigDefinitionPrototype definition:
         :param SchematicsWorkspace schematics: (optional) A Schematics workspace to
                use for deploying this deployable architecture.
@@ -5735,20 +6129,20 @@
         self.definition = definition
         self.schematics = schematics
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigPrototype':
         """Initialize a ProjectConfigPrototype object from a json dictionary."""
         args = {}
-        if 'definition' in _dict:
-            args['definition'] = _dict.get('definition')
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = definition
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigPrototype JSON')
-        if 'schematics' in _dict:
-            args['schematics'] = SchematicsWorkspace.from_dict(_dict.get('schematics'))
+        if (schematics := _dict.get('schematics')) is not None:
+            args['schematics'] = SchematicsWorkspace.from_dict(schematics)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigPrototype object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5786,31 +6180,31 @@
         return not self == other
 
 
 class ProjectConfigResource:
     """
     ProjectConfigResource.
 
-    :attr str resource_crn: (optional) An IBM Cloud resource name that uniquely
+    :param str resource_crn: (optional) An IBM Cloud resource name that uniquely
           identifies a resource.
-    :attr str resource_name: (optional) The name of the resource.
-    :attr str resource_type: (optional) The resource type.
-    :attr bool resource_tainted: (optional) The flag that indicates whether the
+    :param str resource_name: (optional) The name of the resource.
+    :param str resource_type: (optional) The resource type.
+    :param bool resource_tainted: (optional) The flag that indicates whether the
           status of the resource is tainted.
-    :attr str resource_group_name: (optional) The resource group of the resource.
+    :param str resource_group_name: (optional) The resource group of the resource.
     """
 
     def __init__(
         self,
         *,
-        resource_crn: str = None,
-        resource_name: str = None,
-        resource_type: str = None,
-        resource_tainted: bool = None,
-        resource_group_name: str = None,
+        resource_crn: Optional[str] = None,
+        resource_name: Optional[str] = None,
+        resource_type: Optional[str] = None,
+        resource_tainted: Optional[bool] = None,
+        resource_group_name: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigResource object.
 
         :param str resource_crn: (optional) An IBM Cloud resource name that
                uniquely identifies a resource.
         :param str resource_name: (optional) The name of the resource.
@@ -5826,24 +6220,24 @@
         self.resource_tainted = resource_tainted
         self.resource_group_name = resource_group_name
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigResource':
         """Initialize a ProjectConfigResource object from a json dictionary."""
         args = {}
-        if 'resource_crn' in _dict:
-            args['resource_crn'] = _dict.get('resource_crn')
-        if 'resource_name' in _dict:
-            args['resource_name'] = _dict.get('resource_name')
-        if 'resource_type' in _dict:
-            args['resource_type'] = _dict.get('resource_type')
-        if 'resource_tainted' in _dict:
-            args['resource_tainted'] = _dict.get('resource_tainted')
-        if 'resource_group_name' in _dict:
-            args['resource_group_name'] = _dict.get('resource_group_name')
+        if (resource_crn := _dict.get('resource_crn')) is not None:
+            args['resource_crn'] = resource_crn
+        if (resource_name := _dict.get('resource_name')) is not None:
+            args['resource_name'] = resource_name
+        if (resource_type := _dict.get('resource_type')) is not None:
+            args['resource_type'] = resource_type
+        if (resource_tainted := _dict.get('resource_tainted')) is not None:
+            args['resource_tainted'] = resource_tainted
+        if (resource_group_name := _dict.get('resource_group_name')) is not None:
+            args['resource_group_name'] = resource_group_name
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigResource object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -5881,17 +6275,17 @@
         return not self == other
 
 
 class ProjectConfigResourceCollection:
     """
     The project configuration resource list.
 
-    :attr List[ProjectConfigResource] resources: The collection list operation
+    :param List[ProjectConfigResource] resources: The collection list operation
           response schema that defines the array property with the name `resources`.
-    :attr int resources_count: The total number of resources that are deployed by
+    :param int resources_count: The total number of resources that are deployed by
           the configuration.
     """
 
     def __init__(
         self,
         resources: List['ProjectConfigResource'],
         resources_count: int,
@@ -5907,20 +6301,20 @@
         self.resources = resources
         self.resources_count = resources_count
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigResourceCollection':
         """Initialize a ProjectConfigResourceCollection object from a json dictionary."""
         args = {}
-        if 'resources' in _dict:
-            args['resources'] = [ProjectConfigResource.from_dict(v) for v in _dict.get('resources')]
+        if (resources := _dict.get('resources')) is not None:
+            args['resources'] = [ProjectConfigResource.from_dict(v) for v in resources]
         else:
             raise ValueError('Required property \'resources\' not present in ProjectConfigResourceCollection JSON')
-        if 'resources_count' in _dict:
-            args['resources_count'] = _dict.get('resources_count')
+        if (resources_count := _dict.get('resources_count')) is not None:
+            args['resources_count'] = resources_count
         else:
             raise ValueError(
                 'Required property \'resources_count\' not present in ProjectConfigResourceCollection JSON'
             )
         return cls(**args)
 
     @classmethod
@@ -5962,49 +6356,50 @@
         return not self == other
 
 
 class ProjectConfigSummary:
     """
     ProjectConfigSummary.
 
-    :attr ProjectConfigVersionSummary approved_version: (optional) A summary of a
+    :param ProjectConfigVersionSummary approved_version: (optional) A summary of a
           project configuration version.
-    :attr ProjectConfigVersionSummary deployed_version: (optional) A summary of a
+    :param ProjectConfigVersionSummary deployed_version: (optional) A summary of a
           project configuration version.
-    :attr str id: The ID of the configuration. If this parameter is empty, an ID is
+    :param str id: The ID of the configuration. If this parameter is empty, an ID is
           automatically created for the configuration.
-    :attr int version: The version of the configuration.
-    :attr str state: The state of the configuration.
-    :attr datetime created_at: A date and time value in the format
+    :param int version: The version of the configuration.
+    :param str state: The state of the configuration.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr datetime modified_at: A date and time value in the format
+    :param datetime modified_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str href: A URL.
-    :attr ProjectConfigSummaryDefinition definition: The description of a project
+    :param str href: A URL.
+    :param ProjectConfigSummaryDefinition definition: The description of a project
           configuration.
-    :attr ProjectReference project: The project that is referenced by this resource.
-    :attr str deployment_model: (optional) The configuration type.
+    :param ProjectReference project: The project that is referenced by this
+          resource.
+    :param str deployment_model: (optional) The configuration type.
     """
 
     def __init__(
         self,
         id: str,
         version: int,
         state: str,
         created_at: datetime,
         modified_at: datetime,
         href: str,
         definition: 'ProjectConfigSummaryDefinition',
         project: 'ProjectReference',
         *,
-        approved_version: 'ProjectConfigVersionSummary' = None,
-        deployed_version: 'ProjectConfigVersionSummary' = None,
-        deployment_model: str = None,
+        approved_version: Optional['ProjectConfigVersionSummary'] = None,
+        deployed_version: Optional['ProjectConfigVersionSummary'] = None,
+        deployment_model: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigSummary object.
 
         :param str id: The ID of the configuration. If this parameter is empty, an
                ID is automatically created for the configuration.
         :param int version: The version of the configuration.
@@ -6038,52 +6433,52 @@
         self.project = project
         self.deployment_model = deployment_model
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigSummary':
         """Initialize a ProjectConfigSummary object from a json dictionary."""
         args = {}
-        if 'approved_version' in _dict:
-            args['approved_version'] = ProjectConfigVersionSummary.from_dict(_dict.get('approved_version'))
-        if 'deployed_version' in _dict:
-            args['deployed_version'] = ProjectConfigVersionSummary.from_dict(_dict.get('deployed_version'))
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (approved_version := _dict.get('approved_version')) is not None:
+            args['approved_version'] = ProjectConfigVersionSummary.from_dict(approved_version)
+        if (deployed_version := _dict.get('deployed_version')) is not None:
+            args['deployed_version'] = ProjectConfigVersionSummary.from_dict(deployed_version)
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectConfigSummary JSON')
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ProjectConfigSummary JSON')
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfigSummary JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in ProjectConfigSummary JSON')
-        if 'modified_at' in _dict:
-            args['modified_at'] = string_to_datetime(_dict.get('modified_at'))
+        if (modified_at := _dict.get('modified_at')) is not None:
+            args['modified_at'] = string_to_datetime(modified_at)
         else:
             raise ValueError('Required property \'modified_at\' not present in ProjectConfigSummary JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfigSummary JSON')
-        if 'definition' in _dict:
-            args['definition'] = ProjectConfigSummaryDefinition.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectConfigSummaryDefinition.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigSummary JSON')
-        if 'project' in _dict:
-            args['project'] = ProjectReference.from_dict(_dict.get('project'))
+        if (project := _dict.get('project')) is not None:
+            args['project'] = ProjectReference.from_dict(project)
         else:
             raise ValueError('Required property \'project\' not present in ProjectConfigSummary JSON')
-        if 'deployment_model' in _dict:
-            args['deployment_model'] = _dict.get('deployment_model')
+        if (deployment_model := _dict.get('deployment_model')) is not None:
+            args['deployment_model'] = deployment_model
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -6170,24 +6565,25 @@
     class DeploymentModelEnum(str, Enum):
         """
         The configuration type.
         """
 
         PROJECT_DEPLOYED = 'project_deployed'
         USER_DEPLOYED = 'user_deployed'
+        STACK = 'stack'
 
 
 class ProjectConfigSummaryDefinition:
     """
     The description of a project configuration.
 
-    :attr str description: A project configuration description.
-    :attr str name: The configuration name. It's unique within the account across
+    :param str description: A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
           projects and regions.
-    :attr str locator_id: (optional) A unique concatenation of the catalog ID and
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
           > 1. If only a `locator_id` is specified, a new Schematics workspace is
@@ -6203,15 +6599,15 @@
     """
 
     def __init__(
         self,
         description: str,
         name: str,
         *,
-        locator_id: str = None,
+        locator_id: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigSummaryDefinition object.
 
         :param str description: A project configuration description.
         :param str name: The configuration name. It's unique within the account
                across projects and regions.
@@ -6237,24 +6633,24 @@
         self.name = name
         self.locator_id = locator_id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigSummaryDefinition':
         """Initialize a ProjectConfigSummaryDefinition object from a json dictionary."""
         args = {}
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError('Required property \'description\' not present in ProjectConfigSummaryDefinition JSON')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in ProjectConfigSummaryDefinition JSON')
-        if 'locator_id' in _dict:
-            args['locator_id'] = _dict.get('locator_id')
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigSummaryDefinition object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -6288,88 +6684,91 @@
         return not self == other
 
 
 class ProjectConfigVersion:
     """
     A specific version of a project configuration.
 
-    :attr str id: The ID of the configuration. If this parameter is empty, an ID is
+    :param str id: The ID of the configuration. If this parameter is empty, an ID is
           automatically created for the configuration.
-    :attr int version: The version of the configuration.
-    :attr bool is_draft: The flag that indicates whether the version of the
+    :param int version: The version of the configuration.
+    :param bool is_draft: The flag that indicates whether the version of the
           configuration is draft, or active.
-    :attr List[object] needs_attention_state: The needs attention state of a
-          configuration.
-    :attr datetime created_at: A date and time value in the format
+    :param List[ProjectConfigNeedsAttentionState] needs_attention_state: The needs
+          attention state of a configuration.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr datetime modified_at: A date and time value in the format
+    :param datetime modified_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr ProjectConfigMetadataLastApproved last_approved: (optional) The last
+    :param ProjectConfigMetadataLastApproved last_approved: (optional) The last
           approved metadata of the configuration.
-    :attr datetime last_saved_at: (optional) A date and time value in the format
+    :param datetime last_saved_at: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr LastValidatedActionWithSummary last_validated: (optional) The href and
+    :param LastValidatedActionWithSummary last_validated: (optional) The href and
           results from the last action job that is performed on the project configuration.
-    :attr LastActionWithSummary last_deployed: (optional) The href and results from
+    :param LastActionWithSummary last_deployed: (optional) The href and results from
           the last action job that is performed on the project configuration.
-    :attr LastActionWithSummary last_undeployed: (optional) The href and results
+    :param LastActionWithSummary last_undeployed: (optional) The href and results
           from the last action job that is performed on the project configuration.
-    :attr LastMonitoringActionWithSummary last_monitoring: (optional) The summary
+    :param LastMonitoringActionWithSummary last_monitoring: (optional) The summary
           from the last monitoring action job that is performed on the project
           configuration.
-    :attr List[OutputValue] outputs: The outputs of a Schematics template property.
-    :attr ProjectReference project: The project that is referenced by this resource.
-    :attr dict references: (optional) The references that are used in the
+    :param List[OutputValue] outputs: The outputs of a Schematics template property.
+    :param ProjectReference project: The project that is referenced by this
+          resource.
+    :param dict references: (optional) The references that are used in the
           configuration to resolve input values.
-    :attr SchematicsMetadata schematics: (optional) A Schematics workspace that is
+    :param SchematicsMetadata schematics: (optional) A Schematics workspace that is
           associated to a project configuration, with scripts.
-    :attr str state: The state of the configuration.
-    :attr bool update_available: (optional) The flag that indicates whether a
+    :param str state: The state of the configuration.
+    :param bool update_available: (optional) The flag that indicates whether a
           configuration update is available.
-    :attr str href: A URL.
-    :attr ProjectConfigDefinitionResponse definition:
+    :param ProjectObjectReference template: (optional) The template reference.
+    :param str href: A URL.
+    :param ProjectConfigDefinitionResponse definition:
     """
 
     def __init__(
         self,
         id: str,
         version: int,
         is_draft: bool,
-        needs_attention_state: List[object],
+        needs_attention_state: List['ProjectConfigNeedsAttentionState'],
         created_at: datetime,
         modified_at: datetime,
         outputs: List['OutputValue'],
         project: 'ProjectReference',
         state: str,
         href: str,
         definition: 'ProjectConfigDefinitionResponse',
         *,
-        last_approved: 'ProjectConfigMetadataLastApproved' = None,
-        last_saved_at: datetime = None,
-        last_validated: 'LastValidatedActionWithSummary' = None,
-        last_deployed: 'LastActionWithSummary' = None,
-        last_undeployed: 'LastActionWithSummary' = None,
-        last_monitoring: 'LastMonitoringActionWithSummary' = None,
-        references: dict = None,
-        schematics: 'SchematicsMetadata' = None,
-        update_available: bool = None,
+        last_approved: Optional['ProjectConfigMetadataLastApproved'] = None,
+        last_saved_at: Optional[datetime] = None,
+        last_validated: Optional['LastValidatedActionWithSummary'] = None,
+        last_deployed: Optional['LastActionWithSummary'] = None,
+        last_undeployed: Optional['LastActionWithSummary'] = None,
+        last_monitoring: Optional['LastMonitoringActionWithSummary'] = None,
+        references: Optional[dict] = None,
+        schematics: Optional['SchematicsMetadata'] = None,
+        update_available: Optional[bool] = None,
+        template: Optional['ProjectObjectReference'] = None,
     ) -> None:
         """
         Initialize a ProjectConfigVersion object.
 
         :param str id: The ID of the configuration. If this parameter is empty, an
                ID is automatically created for the configuration.
         :param int version: The version of the configuration.
         :param bool is_draft: The flag that indicates whether the version of the
                configuration is draft, or active.
-        :param List[object] needs_attention_state: The needs attention state of a
-               configuration.
+        :param List[ProjectConfigNeedsAttentionState] needs_attention_state: The
+               needs attention state of a configuration.
         :param datetime created_at: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
         :param datetime modified_at: A date and time value in the format
                YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
                format as specified by RFC 3339.
         :param List[OutputValue] outputs: The outputs of a Schematics template
@@ -6397,14 +6796,15 @@
                project configuration.
         :param dict references: (optional) The references that are used in the
                configuration to resolve input values.
         :param SchematicsMetadata schematics: (optional) A Schematics workspace
                that is associated to a project configuration, with scripts.
         :param bool update_available: (optional) The flag that indicates whether a
                configuration update is available.
+        :param ProjectObjectReference template: (optional) The template reference.
         """
         self.id = id
         self.version = version
         self.is_draft = is_draft
         self.needs_attention_state = needs_attention_state
         self.created_at = created_at
         self.modified_at = modified_at
@@ -6416,81 +6816,86 @@
         self.last_monitoring = last_monitoring
         self.outputs = outputs
         self.project = project
         self.references = references
         self.schematics = schematics
         self.state = state
         self.update_available = update_available
+        self.template = template
         self.href = href
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersion':
         """Initialize a ProjectConfigVersion object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectConfigVersion JSON')
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ProjectConfigVersion JSON')
-        if 'is_draft' in _dict:
-            args['is_draft'] = _dict.get('is_draft')
+        if (is_draft := _dict.get('is_draft')) is not None:
+            args['is_draft'] = is_draft
         else:
             raise ValueError('Required property \'is_draft\' not present in ProjectConfigVersion JSON')
-        if 'needs_attention_state' in _dict:
-            args['needs_attention_state'] = _dict.get('needs_attention_state')
+        if (needs_attention_state := _dict.get('needs_attention_state')) is not None:
+            args['needs_attention_state'] = [
+                ProjectConfigNeedsAttentionState.from_dict(v) for v in needs_attention_state
+            ]
         else:
             raise ValueError('Required property \'needs_attention_state\' not present in ProjectConfigVersion JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in ProjectConfigVersion JSON')
-        if 'modified_at' in _dict:
-            args['modified_at'] = string_to_datetime(_dict.get('modified_at'))
+        if (modified_at := _dict.get('modified_at')) is not None:
+            args['modified_at'] = string_to_datetime(modified_at)
         else:
             raise ValueError('Required property \'modified_at\' not present in ProjectConfigVersion JSON')
-        if 'last_approved' in _dict:
-            args['last_approved'] = ProjectConfigMetadataLastApproved.from_dict(_dict.get('last_approved'))
-        if 'last_saved_at' in _dict:
-            args['last_saved_at'] = string_to_datetime(_dict.get('last_saved_at'))
-        if 'last_validated' in _dict:
-            args['last_validated'] = LastValidatedActionWithSummary.from_dict(_dict.get('last_validated'))
-        if 'last_deployed' in _dict:
-            args['last_deployed'] = LastActionWithSummary.from_dict(_dict.get('last_deployed'))
-        if 'last_undeployed' in _dict:
-            args['last_undeployed'] = LastActionWithSummary.from_dict(_dict.get('last_undeployed'))
-        if 'last_monitoring' in _dict:
-            args['last_monitoring'] = LastMonitoringActionWithSummary.from_dict(_dict.get('last_monitoring'))
-        if 'outputs' in _dict:
-            args['outputs'] = [OutputValue.from_dict(v) for v in _dict.get('outputs')]
+        if (last_approved := _dict.get('last_approved')) is not None:
+            args['last_approved'] = ProjectConfigMetadataLastApproved.from_dict(last_approved)
+        if (last_saved_at := _dict.get('last_saved_at')) is not None:
+            args['last_saved_at'] = string_to_datetime(last_saved_at)
+        if (last_validated := _dict.get('last_validated')) is not None:
+            args['last_validated'] = LastValidatedActionWithSummary.from_dict(last_validated)
+        if (last_deployed := _dict.get('last_deployed')) is not None:
+            args['last_deployed'] = LastActionWithSummary.from_dict(last_deployed)
+        if (last_undeployed := _dict.get('last_undeployed')) is not None:
+            args['last_undeployed'] = LastActionWithSummary.from_dict(last_undeployed)
+        if (last_monitoring := _dict.get('last_monitoring')) is not None:
+            args['last_monitoring'] = LastMonitoringActionWithSummary.from_dict(last_monitoring)
+        if (outputs := _dict.get('outputs')) is not None:
+            args['outputs'] = [OutputValue.from_dict(v) for v in outputs]
         else:
             raise ValueError('Required property \'outputs\' not present in ProjectConfigVersion JSON')
-        if 'project' in _dict:
-            args['project'] = ProjectReference.from_dict(_dict.get('project'))
+        if (project := _dict.get('project')) is not None:
+            args['project'] = ProjectReference.from_dict(project)
         else:
             raise ValueError('Required property \'project\' not present in ProjectConfigVersion JSON')
-        if 'references' in _dict:
-            args['references'] = _dict.get('references')
-        if 'schematics' in _dict:
-            args['schematics'] = SchematicsMetadata.from_dict(_dict.get('schematics'))
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (references := _dict.get('references')) is not None:
+            args['references'] = references
+        if (schematics := _dict.get('schematics')) is not None:
+            args['schematics'] = SchematicsMetadata.from_dict(schematics)
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfigVersion JSON')
-        if 'update_available' in _dict:
-            args['update_available'] = _dict.get('update_available')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (update_available := _dict.get('update_available')) is not None:
+            args['update_available'] = update_available
+        if (template := _dict.get('template')) is not None:
+            args['template'] = ProjectObjectReference.from_dict(template)
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfigVersion JSON')
-        if 'definition' in _dict:
-            args['definition'] = _dict.get('definition')
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = definition
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigVersion JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigVersion object from a json dictionary."""
@@ -6502,15 +6907,21 @@
         if hasattr(self, 'id') and self.id is not None:
             _dict['id'] = self.id
         if hasattr(self, 'version') and self.version is not None:
             _dict['version'] = self.version
         if hasattr(self, 'is_draft') and self.is_draft is not None:
             _dict['is_draft'] = self.is_draft
         if hasattr(self, 'needs_attention_state') and self.needs_attention_state is not None:
-            _dict['needs_attention_state'] = self.needs_attention_state
+            needs_attention_state_list = []
+            for v in self.needs_attention_state:
+                if isinstance(v, dict):
+                    needs_attention_state_list.append(v)
+                else:
+                    needs_attention_state_list.append(v.to_dict())
+            _dict['needs_attention_state'] = needs_attention_state_list
         if hasattr(self, 'created_at') and self.created_at is not None:
             _dict['created_at'] = datetime_to_string(self.created_at)
         if hasattr(self, 'modified_at') and self.modified_at is not None:
             _dict['modified_at'] = datetime_to_string(self.modified_at)
         if hasattr(self, 'last_approved') and self.last_approved is not None:
             if isinstance(self.last_approved, dict):
                 _dict['last_approved'] = self.last_approved
@@ -6558,14 +6969,19 @@
                 _dict['schematics'] = self.schematics
             else:
                 _dict['schematics'] = self.schematics.to_dict()
         if hasattr(self, 'state') and self.state is not None:
             _dict['state'] = self.state
         if hasattr(self, 'update_available') and self.update_available is not None:
             _dict['update_available'] = self.update_available
+        if hasattr(self, 'template') and self.template is not None:
+            if isinstance(self.template, dict):
+                _dict['template'] = self.template
+            else:
+                _dict['template'] = self.template.to_dict()
         if hasattr(self, 'href') and self.href is not None:
             _dict['href'] = self.href
         if hasattr(self, 'definition') and self.definition is not None:
             if isinstance(self.definition, dict):
                 _dict['definition'] = self.definition
             else:
                 _dict['definition'] = self.definition.to_dict()
@@ -6613,16 +7029,16 @@
         APPLY_FAILED = 'apply_failed'
 
 
 class ProjectConfigVersionDefinitionSummary:
     """
     A summary of the definition in a project configuration version.
 
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr str locator_id: (optional) A unique concatenation of the catalog ID and
+    :param str environment_id: (optional) The ID of the project environment.
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
           > 1. If only a `locator_id` is specified, a new Schematics workspace is
@@ -6636,16 +7052,16 @@
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
     """
 
     def __init__(
         self,
         *,
-        environment_id: str = None,
-        locator_id: str = None,
+        environment_id: Optional[str] = None,
+        locator_id: Optional[str] = None,
     ) -> None:
         """
         Initialize a ProjectConfigVersionDefinitionSummary object.
 
         :param str environment_id: (optional) The ID of the project environment.
         :param str locator_id: (optional) A unique concatenation of the catalog ID
                and the version ID that identify the deployable architecture in the
@@ -6668,18 +7084,18 @@
         self.environment_id = environment_id
         self.locator_id = locator_id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersionDefinitionSummary':
         """Initialize a ProjectConfigVersionDefinitionSummary object from a json dictionary."""
         args = {}
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'locator_id' in _dict:
-            args['locator_id'] = _dict.get('locator_id')
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigVersionDefinitionSummary object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -6711,19 +7127,19 @@
         return not self == other
 
 
 class ProjectConfigVersionSummary:
     """
     A summary of a project configuration version.
 
-    :attr ProjectConfigVersionDefinitionSummary definition: A summary of the
+    :param ProjectConfigVersionDefinitionSummary definition: A summary of the
           definition in a project configuration version.
-    :attr str state: The state of the configuration.
-    :attr int version: The version number of the configuration.
-    :attr str href: A URL.
+    :param str state: The state of the configuration.
+    :param int version: The version number of the configuration.
+    :param str href: A URL.
     """
 
     def __init__(
         self,
         definition: 'ProjectConfigVersionDefinitionSummary',
         state: str,
         version: int,
@@ -6743,28 +7159,28 @@
         self.version = version
         self.href = href
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersionSummary':
         """Initialize a ProjectConfigVersionSummary object from a json dictionary."""
         args = {}
-        if 'definition' in _dict:
-            args['definition'] = ProjectConfigVersionDefinitionSummary.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectConfigVersionDefinitionSummary.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectConfigVersionSummary JSON')
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectConfigVersionSummary JSON')
-        if 'version' in _dict:
-            args['version'] = _dict.get('version')
+        if (version := _dict.get('version')) is not None:
+            args['version'] = version
         else:
             raise ValueError('Required property \'version\' not present in ProjectConfigVersionSummary JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectConfigVersionSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigVersionSummary object from a json dictionary."""
@@ -6828,15 +7244,15 @@
         APPLY_FAILED = 'apply_failed'
 
 
 class ProjectConfigVersionSummaryCollection:
     """
     The project configuration version list.
 
-    :attr List[ProjectConfigVersionSummary] versions: The collection list operation
+    :param List[ProjectConfigVersionSummary] versions: The collection list operation
           response schema that defines the array property with the name `versions`.
     """
 
     def __init__(
         self,
         versions: List['ProjectConfigVersionSummary'],
     ) -> None:
@@ -6849,16 +7265,16 @@
         """
         self.versions = versions
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigVersionSummaryCollection':
         """Initialize a ProjectConfigVersionSummaryCollection object from a json dictionary."""
         args = {}
-        if 'versions' in _dict:
-            args['versions'] = [ProjectConfigVersionSummary.from_dict(v) for v in _dict.get('versions')]
+        if (versions := _dict.get('versions')) is not None:
+            args['versions'] = [ProjectConfigVersionSummary.from_dict(v) for v in versions]
         else:
             raise ValueError('Required property \'versions\' not present in ProjectConfigVersionSummaryCollection JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigVersionSummaryCollection object from a json dictionary."""
@@ -6896,33 +7312,33 @@
         return not self == other
 
 
 class ProjectDefinitionProperties:
     """
     The definition of the project.
 
-    :attr str name: The name of the project.  It's unique within the account across
+    :param str name: The name of the project.  It's unique within the account across
           regions.
-    :attr bool destroy_on_delete: The policy that indicates whether the resources
+    :param bool destroy_on_delete: The policy that indicates whether the resources
           are destroyed or not when a project is deleted.
-    :attr str description: A brief explanation of the project's use in the
+    :param str description: A brief explanation of the project's use in the
           configuration of a deployable architecture. You can create a project without
           providing a description.
-    :attr bool monitoring_enabled: (optional) A boolean flag to enable automatic
+    :param bool monitoring_enabled: (optional) A boolean flag to enable automatic
           drift detection. Use this field to run a daily check to compare your
           configurations to your deployed resources to detect any difference.
     """
 
     def __init__(
         self,
         name: str,
         destroy_on_delete: bool,
         description: str,
         *,
-        monitoring_enabled: bool = None,
+        monitoring_enabled: Optional[bool] = None,
     ) -> None:
         """
         Initialize a ProjectDefinitionProperties object.
 
         :param str name: The name of the project.  It's unique within the account
                across regions.
         :param bool destroy_on_delete: The policy that indicates whether the
@@ -6939,28 +7355,28 @@
         self.description = description
         self.monitoring_enabled = monitoring_enabled
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectDefinitionProperties':
         """Initialize a ProjectDefinitionProperties object from a json dictionary."""
         args = {}
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in ProjectDefinitionProperties JSON')
-        if 'destroy_on_delete' in _dict:
-            args['destroy_on_delete'] = _dict.get('destroy_on_delete')
+        if (destroy_on_delete := _dict.get('destroy_on_delete')) is not None:
+            args['destroy_on_delete'] = destroy_on_delete
         else:
             raise ValueError('Required property \'destroy_on_delete\' not present in ProjectDefinitionProperties JSON')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError('Required property \'description\' not present in ProjectDefinitionProperties JSON')
-        if 'monitoring_enabled' in _dict:
-            args['monitoring_enabled'] = _dict.get('monitoring_enabled')
+        if (monitoring_enabled := _dict.get('monitoring_enabled')) is not None:
+            args['monitoring_enabled'] = monitoring_enabled
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectDefinitionProperties object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -6996,15 +7412,15 @@
         return not self == other
 
 
 class ProjectDefinitionReference:
     """
     The definition of the project reference.
 
-    :attr str name: The name of the project.
+    :param str name: The name of the project.
     """
 
     def __init__(
         self,
         name: str,
     ) -> None:
         """
@@ -7014,16 +7430,16 @@
         """
         self.name = name
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectDefinitionReference':
         """Initialize a ProjectDefinitionReference object from a json dictionary."""
         args = {}
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in ProjectDefinitionReference JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectDefinitionReference object from a json dictionary."""
@@ -7055,15 +7471,15 @@
         return not self == other
 
 
 class ProjectDeleteResponse:
     """
     The ID of the deleted project.
 
-    :attr str id: The ID of the deleted project or configuration.
+    :param str id: The ID of the deleted project or configuration.
     """
 
     def __init__(
         self,
         id: str,
     ) -> None:
         """
@@ -7073,16 +7489,16 @@
         """
         self.id = id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectDeleteResponse':
         """Initialize a ProjectDeleteResponse object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectDeleteResponse JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectDeleteResponse object from a json dictionary."""
@@ -7114,22 +7530,23 @@
         return not self == other
 
 
 class ProjectEnvironmentSummary:
     """
     The environment metadata.
 
-    :attr str id: The environment ID as a friendly name.
-    :attr ProjectReference project: The project that is referenced by this resource.
-    :attr datetime created_at: A date and time value in the format
+    :param str id: The environment ID as a friendly name.
+    :param ProjectReference project: The project that is referenced by this
+          resource.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr str href: A URL.
-    :attr ProjectEnvironmentSummaryDefinition definition: The environment definition
-          that is used in the project collection.
+    :param str href: A URL.
+    :param ProjectEnvironmentSummaryDefinition definition: The environment
+          definition that is used in the project collection.
     """
 
     def __init__(
         self,
         id: str,
         project: 'ProjectReference',
         created_at: datetime,
@@ -7155,32 +7572,32 @@
         self.href = href
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectEnvironmentSummary':
         """Initialize a ProjectEnvironmentSummary object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectEnvironmentSummary JSON')
-        if 'project' in _dict:
-            args['project'] = ProjectReference.from_dict(_dict.get('project'))
+        if (project := _dict.get('project')) is not None:
+            args['project'] = ProjectReference.from_dict(project)
         else:
             raise ValueError('Required property \'project\' not present in ProjectEnvironmentSummary JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in ProjectEnvironmentSummary JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectEnvironmentSummary JSON')
-        if 'definition' in _dict:
-            args['definition'] = ProjectEnvironmentSummaryDefinition.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectEnvironmentSummaryDefinition.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectEnvironmentSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectEnvironmentSummary object from a json dictionary."""
@@ -7226,16 +7643,16 @@
         return not self == other
 
 
 class ProjectEnvironmentSummaryDefinition:
     """
     The environment definition that is used in the project collection.
 
-    :attr str description: The description of the environment.
-    :attr str name: The name of the environment. It's unique within the account
+    :param str description: The description of the environment.
+    :param str name: The name of the environment. It's unique within the account
           across projects and regions.
     """
 
     def __init__(
         self,
         description: str,
         name: str,
@@ -7250,22 +7667,22 @@
         self.description = description
         self.name = name
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectEnvironmentSummaryDefinition':
         """Initialize a ProjectEnvironmentSummaryDefinition object from a json dictionary."""
         args = {}
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError(
                 'Required property \'description\' not present in ProjectEnvironmentSummaryDefinition JSON'
             )
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in ProjectEnvironmentSummaryDefinition JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectEnvironmentSummaryDefinition object from a json dictionary."""
@@ -7295,37 +7712,106 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectEnvironmentSummaryDefinition') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ProjectObjectReference:
+    """
+    ProjectObjectReference.
+
+    :param str id: The unique ID.
+    :param str href: A URL.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        href: str,
+    ) -> None:
+        """
+        Initialize a ProjectObjectReference object.
+
+        :param str id: The unique ID.
+        :param str href: A URL.
+        """
+        self.id = id
+        self.href = href
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ProjectObjectReference':
+        """Initialize a ProjectObjectReference object from a json dictionary."""
+        args = {}
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
+        else:
+            raise ValueError('Required property \'id\' not present in ProjectObjectReference JSON')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
+        else:
+            raise ValueError('Required property \'href\' not present in ProjectObjectReference JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ProjectObjectReference object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ProjectObjectReference object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ProjectObjectReference') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ProjectObjectReference') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class ProjectPatchDefinitionBlock:
     """
     The definition of the project.
 
-    :attr str name: (optional) The name of the project.  It's unique within the
+    :param str name: (optional) The name of the project.  It's unique within the
           account across regions.
-    :attr bool destroy_on_delete: (optional) The policy that indicates whether the
+    :param bool destroy_on_delete: (optional) The policy that indicates whether the
           resources are destroyed or not when a project is deleted.
-    :attr str description: (optional) A brief explanation of the project's use in
+    :param str description: (optional) A brief explanation of the project's use in
           the configuration of a deployable architecture. You can create a project without
           providing a description.
-    :attr bool monitoring_enabled: (optional) A boolean flag to enable automatic
+    :param bool monitoring_enabled: (optional) A boolean flag to enable automatic
           drift detection. Use this field to run a daily check to compare your
           configurations to your deployed resources to detect any difference.
     """
 
     def __init__(
         self,
         *,
-        name: str = None,
-        destroy_on_delete: bool = None,
-        description: str = None,
-        monitoring_enabled: bool = None,
+        name: Optional[str] = None,
+        destroy_on_delete: Optional[bool] = None,
+        description: Optional[str] = None,
+        monitoring_enabled: Optional[bool] = None,
     ) -> None:
         """
         Initialize a ProjectPatchDefinitionBlock object.
 
         :param str name: (optional) The name of the project.  It's unique within
                the account across regions.
         :param bool destroy_on_delete: (optional) The policy that indicates whether
@@ -7342,22 +7828,22 @@
         self.description = description
         self.monitoring_enabled = monitoring_enabled
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectPatchDefinitionBlock':
         """Initialize a ProjectPatchDefinitionBlock object from a json dictionary."""
         args = {}
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
-        if 'destroy_on_delete' in _dict:
-            args['destroy_on_delete'] = _dict.get('destroy_on_delete')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'monitoring_enabled' in _dict:
-            args['monitoring_enabled'] = _dict.get('monitoring_enabled')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (destroy_on_delete := _dict.get('destroy_on_delete')) is not None:
+            args['destroy_on_delete'] = destroy_on_delete
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (monitoring_enabled := _dict.get('monitoring_enabled')) is not None:
+            args['monitoring_enabled'] = monitoring_enabled
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectPatchDefinitionBlock object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -7393,33 +7879,33 @@
         return not self == other
 
 
 class ProjectPrototypeDefinition:
     """
     The definition of the project.
 
-    :attr str name: The name of the project.  It's unique within the account across
+    :param str name: The name of the project.  It's unique within the account across
           regions.
-    :attr bool destroy_on_delete: (optional) The policy that indicates whether the
+    :param bool destroy_on_delete: (optional) The policy that indicates whether the
           resources are undeployed or not when a project is deleted.
-    :attr str description: (optional) A brief explanation of the project's use in
+    :param str description: (optional) A brief explanation of the project's use in
           the configuration of a deployable architecture. You can create a project without
           providing a description.
-    :attr bool monitoring_enabled: (optional) A boolean flag to enable automatic
+    :param bool monitoring_enabled: (optional) A boolean flag to enable automatic
           drift detection. Use this field to run a daily check to compare your
           configurations to your deployed resources to detect any difference.
     """
 
     def __init__(
         self,
         name: str,
         *,
-        destroy_on_delete: bool = None,
-        description: str = None,
-        monitoring_enabled: bool = None,
+        destroy_on_delete: Optional[bool] = None,
+        description: Optional[str] = None,
+        monitoring_enabled: Optional[bool] = None,
     ) -> None:
         """
         Initialize a ProjectPrototypeDefinition object.
 
         :param str name: The name of the project.  It's unique within the account
                across regions.
         :param bool destroy_on_delete: (optional) The policy that indicates whether
@@ -7436,24 +7922,24 @@
         self.description = description
         self.monitoring_enabled = monitoring_enabled
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectPrototypeDefinition':
         """Initialize a ProjectPrototypeDefinition object from a json dictionary."""
         args = {}
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError('Required property \'name\' not present in ProjectPrototypeDefinition JSON')
-        if 'destroy_on_delete' in _dict:
-            args['destroy_on_delete'] = _dict.get('destroy_on_delete')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'monitoring_enabled' in _dict:
-            args['monitoring_enabled'] = _dict.get('monitoring_enabled')
+        if (destroy_on_delete := _dict.get('destroy_on_delete')) is not None:
+            args['destroy_on_delete'] = destroy_on_delete
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (monitoring_enabled := _dict.get('monitoring_enabled')) is not None:
+            args['monitoring_enabled'] = monitoring_enabled
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectPrototypeDefinition object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -7489,19 +7975,19 @@
         return not self == other
 
 
 class ProjectReference:
     """
     The project that is referenced by this resource.
 
-    :attr str id: The unique ID.
-    :attr str href: A URL.
-    :attr ProjectDefinitionReference definition: The definition of the project
+    :param str id: The unique ID.
+    :param str href: A URL.
+    :param ProjectDefinitionReference definition: The definition of the project
           reference.
-    :attr str crn: An IBM Cloud resource name that uniquely identifies a resource.
+    :param str crn: An IBM Cloud resource name that uniquely identifies a resource.
     """
 
     def __init__(
         self,
         id: str,
         href: str,
         definition: 'ProjectDefinitionReference',
@@ -7522,28 +8008,28 @@
         self.definition = definition
         self.crn = crn
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectReference':
         """Initialize a ProjectReference object from a json dictionary."""
         args = {}
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectReference JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectReference JSON')
-        if 'definition' in _dict:
-            args['definition'] = ProjectDefinitionReference.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectDefinitionReference.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectReference JSON')
-        if 'crn' in _dict:
-            args['crn'] = _dict.get('crn')
+        if (crn := _dict.get('crn')) is not None:
+            args['crn'] = crn
         else:
             raise ValueError('Required property \'crn\' not present in ProjectReference JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectReference object from a json dictionary."""
@@ -7580,284 +8066,51 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectReference') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
-class ProjectResourceCollection:
-    """
-    The project resource list.
-
-    :attr List[ProjectResourceSummary] resources: The collection list operation
-          response schema that defines the array property with the name `resources`.
-    :attr str token: (optional) A pagination token.
-    :attr PaginationLink first: (optional) A pagination link.
-    :attr PaginationLink next: (optional) A pagination link.
-    """
-
-    def __init__(
-        self,
-        resources: List['ProjectResourceSummary'],
-        *,
-        token: str = None,
-        first: 'PaginationLink' = None,
-        next: 'PaginationLink' = None,
-    ) -> None:
-        """
-        Initialize a ProjectResourceCollection object.
-
-        :param List[ProjectResourceSummary] resources: The collection list
-               operation response schema that defines the array property with the name
-               `resources`.
-        :param str token: (optional) A pagination token.
-        :param PaginationLink first: (optional) A pagination link.
-        :param PaginationLink next: (optional) A pagination link.
-        """
-        self.resources = resources
-        self.token = token
-        self.first = first
-        self.next = next
-
-    @classmethod
-    def from_dict(cls, _dict: Dict) -> 'ProjectResourceCollection':
-        """Initialize a ProjectResourceCollection object from a json dictionary."""
-        args = {}
-        if 'resources' in _dict:
-            args['resources'] = [ProjectResourceSummary.from_dict(v) for v in _dict.get('resources')]
-        else:
-            raise ValueError('Required property \'resources\' not present in ProjectResourceCollection JSON')
-        if 'token' in _dict:
-            args['token'] = _dict.get('token')
-        if 'first' in _dict:
-            args['first'] = PaginationLink.from_dict(_dict.get('first'))
-        if 'next' in _dict:
-            args['next'] = PaginationLink.from_dict(_dict.get('next'))
-        return cls(**args)
-
-    @classmethod
-    def _from_dict(cls, _dict):
-        """Initialize a ProjectResourceCollection object from a json dictionary."""
-        return cls.from_dict(_dict)
-
-    def to_dict(self) -> Dict:
-        """Return a json dictionary representing this model."""
-        _dict = {}
-        if hasattr(self, 'resources') and self.resources is not None:
-            resources_list = []
-            for v in self.resources:
-                if isinstance(v, dict):
-                    resources_list.append(v)
-                else:
-                    resources_list.append(v.to_dict())
-            _dict['resources'] = resources_list
-        if hasattr(self, 'token') and self.token is not None:
-            _dict['token'] = self.token
-        if hasattr(self, 'first') and self.first is not None:
-            if isinstance(self.first, dict):
-                _dict['first'] = self.first
-            else:
-                _dict['first'] = self.first.to_dict()
-        if hasattr(self, 'next') and self.next is not None:
-            if isinstance(self.next, dict):
-                _dict['next'] = self.next
-            else:
-                _dict['next'] = self.next.to_dict()
-        return _dict
-
-    def _to_dict(self):
-        """Return a json dictionary representing this model."""
-        return self.to_dict()
-
-    def __str__(self) -> str:
-        """Return a `str` version of this ProjectResourceCollection object."""
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __eq__(self, other: 'ProjectResourceCollection') -> bool:
-        """Return `true` when self and other are equal, false otherwise."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.__dict__ == other.__dict__
-
-    def __ne__(self, other: 'ProjectResourceCollection') -> bool:
-        """Return `true` when self and other are not equal, false otherwise."""
-        return not self == other
-
-
-class ProjectResourceSummary:
-    """
-    ProjectResourceSummary.
-
-    :attr str resource_crn: (optional) An IBM Cloud resource name that uniquely
-          identifies a resource.
-    :attr str resource_name: (optional) The name of the resource.
-    :attr str account_id: (optional) The ID of the account owning of the resource.
-    :attr str location: (optional) The location of the resource.
-    :attr str resource_type: (optional) The resource type.
-    :attr str resource_status: (optional) The status of the resource.
-    :attr str resource_group_id: (optional) The ID of the resource's resource group.
-    :attr List[str] tags: (optional) The collection of tags.
-    :attr List[str] service_tags: (optional) The collection of service tags.
-    """
-
-    def __init__(
-        self,
-        *,
-        resource_crn: str = None,
-        resource_name: str = None,
-        account_id: str = None,
-        location: str = None,
-        resource_type: str = None,
-        resource_status: str = None,
-        resource_group_id: str = None,
-        tags: List[str] = None,
-        service_tags: List[str] = None,
-    ) -> None:
-        """
-        Initialize a ProjectResourceSummary object.
-
-        :param str resource_crn: (optional) An IBM Cloud resource name that
-               uniquely identifies a resource.
-        :param str resource_name: (optional) The name of the resource.
-        :param str account_id: (optional) The ID of the account owning of the
-               resource.
-        :param str location: (optional) The location of the resource.
-        :param str resource_type: (optional) The resource type.
-        :param str resource_status: (optional) The status of the resource.
-        :param str resource_group_id: (optional) The ID of the resource's resource
-               group.
-        :param List[str] tags: (optional) The collection of tags.
-        :param List[str] service_tags: (optional) The collection of service tags.
-        """
-        self.resource_crn = resource_crn
-        self.resource_name = resource_name
-        self.account_id = account_id
-        self.location = location
-        self.resource_type = resource_type
-        self.resource_status = resource_status
-        self.resource_group_id = resource_group_id
-        self.tags = tags
-        self.service_tags = service_tags
-
-    @classmethod
-    def from_dict(cls, _dict: Dict) -> 'ProjectResourceSummary':
-        """Initialize a ProjectResourceSummary object from a json dictionary."""
-        args = {}
-        if 'resource_crn' in _dict:
-            args['resource_crn'] = _dict.get('resource_crn')
-        if 'resource_name' in _dict:
-            args['resource_name'] = _dict.get('resource_name')
-        if 'account_id' in _dict:
-            args['account_id'] = _dict.get('account_id')
-        if 'location' in _dict:
-            args['location'] = _dict.get('location')
-        if 'resource_type' in _dict:
-            args['resource_type'] = _dict.get('resource_type')
-        if 'resource_status' in _dict:
-            args['resource_status'] = _dict.get('resource_status')
-        if 'resource_group_id' in _dict:
-            args['resource_group_id'] = _dict.get('resource_group_id')
-        if 'tags' in _dict:
-            args['tags'] = _dict.get('tags')
-        if 'service_tags' in _dict:
-            args['service_tags'] = _dict.get('service_tags')
-        return cls(**args)
-
-    @classmethod
-    def _from_dict(cls, _dict):
-        """Initialize a ProjectResourceSummary object from a json dictionary."""
-        return cls.from_dict(_dict)
-
-    def to_dict(self) -> Dict:
-        """Return a json dictionary representing this model."""
-        _dict = {}
-        if hasattr(self, 'resource_crn') and self.resource_crn is not None:
-            _dict['resource_crn'] = self.resource_crn
-        if hasattr(self, 'resource_name') and self.resource_name is not None:
-            _dict['resource_name'] = self.resource_name
-        if hasattr(self, 'account_id') and self.account_id is not None:
-            _dict['account_id'] = self.account_id
-        if hasattr(self, 'location') and self.location is not None:
-            _dict['location'] = self.location
-        if hasattr(self, 'resource_type') and self.resource_type is not None:
-            _dict['resource_type'] = self.resource_type
-        if hasattr(self, 'resource_status') and self.resource_status is not None:
-            _dict['resource_status'] = self.resource_status
-        if hasattr(self, 'resource_group_id') and self.resource_group_id is not None:
-            _dict['resource_group_id'] = self.resource_group_id
-        if hasattr(self, 'tags') and self.tags is not None:
-            _dict['tags'] = self.tags
-        if hasattr(self, 'service_tags') and self.service_tags is not None:
-            _dict['service_tags'] = self.service_tags
-        return _dict
-
-    def _to_dict(self):
-        """Return a json dictionary representing this model."""
-        return self.to_dict()
-
-    def __str__(self) -> str:
-        """Return a `str` version of this ProjectResourceSummary object."""
-        return json.dumps(self.to_dict(), indent=2)
-
-    def __eq__(self, other: 'ProjectResourceSummary') -> bool:
-        """Return `true` when self and other are equal, false otherwise."""
-        if not isinstance(other, self.__class__):
-            return False
-        return self.__dict__ == other.__dict__
-
-    def __ne__(self, other: 'ProjectResourceSummary') -> bool:
-        """Return `true` when self and other are not equal, false otherwise."""
-        return not self == other
-
-    class ResourceTypeEnum(str, Enum):
-        """
-        The resource type.
-        """
-
-        PROJECT_DEPLOYED = 'project_deployed'
-        USER_DEPLOYED = 'user_deployed'
-
-
 class ProjectSummary:
     """
     ProjectSummary.
 
-    :attr str crn: An IBM Cloud resource name that uniquely identifies a resource.
-    :attr datetime created_at: A date and time value in the format
+    :param str crn: An IBM Cloud resource name that uniquely identifies a resource.
+    :param datetime created_at: A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
-    :attr List[CumulativeNeedsAttention] cumulative_needs_attention_view: The
+    :param List[CumulativeNeedsAttention] cumulative_needs_attention_view: The
           cumulative list of needs attention items for a project. If the view is
           successfully retrieved, an empty or nonempty array is returned.
-    :attr bool cumulative_needs_attention_view_error: (optional) A value of `true`
+    :param bool cumulative_needs_attention_view_error: (optional) A value of `true`
           indicates that the fetch of the needs attention items failed. This property only
           exists if there was an error when you retrieved the cumulative needs attention
           view.
-    :attr str id: The unique project ID.
-    :attr str location: The IBM Cloud location where a resource is deployed.
-    :attr str resource_group_id: The resource group ID where the project's data and
+    :param str id: The unique project ID.
+    :param str location: The IBM Cloud location where a resource is deployed.
+    :param str resource_group_id: The resource group ID where the project's data and
           tools are created.
-    :attr str state: The project status value.
-    :attr str href: A URL.
-    :attr ProjectDefinitionProperties definition: The definition of the project.
+    :param str state: The project status value.
+    :param str href: A URL.
+    :param ProjectDefinitionProperties definition: The definition of the project.
     """
 
     def __init__(
         self,
         crn: str,
         created_at: datetime,
         cumulative_needs_attention_view: List['CumulativeNeedsAttention'],
         id: str,
         location: str,
         resource_group_id: str,
         state: str,
         href: str,
         definition: 'ProjectDefinitionProperties',
         *,
-        cumulative_needs_attention_view_error: bool = None,
+        cumulative_needs_attention_view_error: Optional[bool] = None,
     ) -> None:
         """
         Initialize a ProjectSummary object.
 
         :param str crn: An IBM Cloud resource name that uniquely identifies a
                resource.
         :param datetime created_at: A date and time value in the format
@@ -7890,52 +8143,52 @@
         self.href = href
         self.definition = definition
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectSummary':
         """Initialize a ProjectSummary object from a json dictionary."""
         args = {}
-        if 'crn' in _dict:
-            args['crn'] = _dict.get('crn')
+        if (crn := _dict.get('crn')) is not None:
+            args['crn'] = crn
         else:
             raise ValueError('Required property \'crn\' not present in ProjectSummary JSON')
-        if 'created_at' in _dict:
-            args['created_at'] = string_to_datetime(_dict.get('created_at'))
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
         else:
             raise ValueError('Required property \'created_at\' not present in ProjectSummary JSON')
-        if 'cumulative_needs_attention_view' in _dict:
+        if (cumulative_needs_attention_view := _dict.get('cumulative_needs_attention_view')) is not None:
             args['cumulative_needs_attention_view'] = [
-                CumulativeNeedsAttention.from_dict(v) for v in _dict.get('cumulative_needs_attention_view')
+                CumulativeNeedsAttention.from_dict(v) for v in cumulative_needs_attention_view
             ]
         else:
             raise ValueError('Required property \'cumulative_needs_attention_view\' not present in ProjectSummary JSON')
-        if 'cumulative_needs_attention_view_error' in _dict:
-            args['cumulative_needs_attention_view_error'] = _dict.get('cumulative_needs_attention_view_error')
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (cumulative_needs_attention_view_error := _dict.get('cumulative_needs_attention_view_error')) is not None:
+            args['cumulative_needs_attention_view_error'] = cumulative_needs_attention_view_error
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         else:
             raise ValueError('Required property \'id\' not present in ProjectSummary JSON')
-        if 'location' in _dict:
-            args['location'] = _dict.get('location')
+        if (location := _dict.get('location')) is not None:
+            args['location'] = location
         else:
             raise ValueError('Required property \'location\' not present in ProjectSummary JSON')
-        if 'resource_group_id' in _dict:
-            args['resource_group_id'] = _dict.get('resource_group_id')
+        if (resource_group_id := _dict.get('resource_group_id')) is not None:
+            args['resource_group_id'] = resource_group_id
         else:
             raise ValueError('Required property \'resource_group_id\' not present in ProjectSummary JSON')
-        if 'state' in _dict:
-            args['state'] = _dict.get('state')
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
         else:
             raise ValueError('Required property \'state\' not present in ProjectSummary JSON')
-        if 'href' in _dict:
-            args['href'] = _dict.get('href')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
         else:
             raise ValueError('Required property \'href\' not present in ProjectSummary JSON')
-        if 'definition' in _dict:
-            args['definition'] = ProjectDefinitionProperties.from_dict(_dict.get('definition'))
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ProjectDefinitionProperties.from_dict(definition)
         else:
             raise ValueError('Required property \'definition\' not present in ProjectSummary JSON')
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectSummary object from a json dictionary."""
@@ -8006,46 +8259,46 @@
         DELETING_FAILED = 'deleting_failed'
 
 
 class SchematicsMetadata:
     """
     A Schematics workspace that is associated to a project configuration, with scripts.
 
-    :attr str workspace_crn: (optional) An IBM Cloud resource name that uniquely
+    :param str workspace_crn: (optional) An IBM Cloud resource name that uniquely
           identifies a resource.
-    :attr Script validate_pre_script: (optional) A script to be run as part of a
+    :param Script validate_pre_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
-    :attr Script validate_post_script: (optional) A script to be run as part of a
+    :param Script validate_post_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
-    :attr Script deploy_pre_script: (optional) A script to be run as part of a
+    :param Script deploy_pre_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
-    :attr Script deploy_post_script: (optional) A script to be run as part of a
+    :param Script deploy_post_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
-    :attr Script undeploy_pre_script: (optional) A script to be run as part of a
+    :param Script undeploy_pre_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
-    :attr Script undeploy_post_script: (optional) A script to be run as part of a
+    :param Script undeploy_post_script: (optional) A script to be run as part of a
           project configuration for a specific stage (pre or post) and action (validate,
           deploy, or undeploy).
     """
 
     def __init__(
         self,
         *,
-        workspace_crn: str = None,
-        validate_pre_script: 'Script' = None,
-        validate_post_script: 'Script' = None,
-        deploy_pre_script: 'Script' = None,
-        deploy_post_script: 'Script' = None,
-        undeploy_pre_script: 'Script' = None,
-        undeploy_post_script: 'Script' = None,
+        workspace_crn: Optional[str] = None,
+        validate_pre_script: Optional['Script'] = None,
+        validate_post_script: Optional['Script'] = None,
+        deploy_pre_script: Optional['Script'] = None,
+        deploy_post_script: Optional['Script'] = None,
+        undeploy_pre_script: Optional['Script'] = None,
+        undeploy_post_script: Optional['Script'] = None,
     ) -> None:
         """
         Initialize a SchematicsMetadata object.
 
         :param str workspace_crn: (optional) An IBM Cloud resource name that
                uniquely identifies a resource.
         :param Script validate_pre_script: (optional) A script to be run as part of
@@ -8075,28 +8328,28 @@
         self.undeploy_pre_script = undeploy_pre_script
         self.undeploy_post_script = undeploy_post_script
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SchematicsMetadata':
         """Initialize a SchematicsMetadata object from a json dictionary."""
         args = {}
-        if 'workspace_crn' in _dict:
-            args['workspace_crn'] = _dict.get('workspace_crn')
-        if 'validate_pre_script' in _dict:
-            args['validate_pre_script'] = Script.from_dict(_dict.get('validate_pre_script'))
-        if 'validate_post_script' in _dict:
-            args['validate_post_script'] = Script.from_dict(_dict.get('validate_post_script'))
-        if 'deploy_pre_script' in _dict:
-            args['deploy_pre_script'] = Script.from_dict(_dict.get('deploy_pre_script'))
-        if 'deploy_post_script' in _dict:
-            args['deploy_post_script'] = Script.from_dict(_dict.get('deploy_post_script'))
-        if 'undeploy_pre_script' in _dict:
-            args['undeploy_pre_script'] = Script.from_dict(_dict.get('undeploy_pre_script'))
-        if 'undeploy_post_script' in _dict:
-            args['undeploy_post_script'] = Script.from_dict(_dict.get('undeploy_post_script'))
+        if (workspace_crn := _dict.get('workspace_crn')) is not None:
+            args['workspace_crn'] = workspace_crn
+        if (validate_pre_script := _dict.get('validate_pre_script')) is not None:
+            args['validate_pre_script'] = Script.from_dict(validate_pre_script)
+        if (validate_post_script := _dict.get('validate_post_script')) is not None:
+            args['validate_post_script'] = Script.from_dict(validate_post_script)
+        if (deploy_pre_script := _dict.get('deploy_pre_script')) is not None:
+            args['deploy_pre_script'] = Script.from_dict(deploy_pre_script)
+        if (deploy_post_script := _dict.get('deploy_post_script')) is not None:
+            args['deploy_post_script'] = Script.from_dict(deploy_post_script)
+        if (undeploy_pre_script := _dict.get('undeploy_pre_script')) is not None:
+            args['undeploy_pre_script'] = Script.from_dict(undeploy_pre_script)
+        if (undeploy_post_script := _dict.get('undeploy_post_script')) is not None:
+            args['undeploy_post_script'] = Script.from_dict(undeploy_post_script)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SchematicsMetadata object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8170,37 +8423,37 @@
     `locator_id` is not found in the existing schematics workspace.
     > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
     `400`code  is returned if the specified `locator_id` does not agree with the
     `locator_id` in the existing Schematics workspace.
     > For more information, see [Creating workspaces and importing your Terraform
     template](/docs/schematics?topic=schematics-sch-create-wks).
 
-    :attr str workspace_crn: (optional) An IBM Cloud resource name that uniquely
+    :param str workspace_crn: (optional) An IBM Cloud resource name that uniquely
           identifies a resource.
     """
 
     def __init__(
         self,
         *,
-        workspace_crn: str = None,
+        workspace_crn: Optional[str] = None,
     ) -> None:
         """
         Initialize a SchematicsWorkspace object.
 
         :param str workspace_crn: (optional) An IBM Cloud resource name that
                uniquely identifies a resource.
         """
         self.workspace_crn = workspace_crn
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'SchematicsWorkspace':
         """Initialize a SchematicsWorkspace object from a json dictionary."""
         args = {}
-        if 'workspace_crn' in _dict:
-            args['workspace_crn'] = _dict.get('workspace_crn')
+        if (workspace_crn := _dict.get('workspace_crn')) is not None:
+            args['workspace_crn'] = workspace_crn
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a SchematicsWorkspace object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8231,26 +8484,26 @@
 
 
 class Script:
     """
     A script to be run as part of a project configuration for a specific stage (pre or
     post) and action (validate, deploy, or undeploy).
 
-    :attr str type: (optional) The type of the script.
-    :attr str path: (optional) The path to this script is within the current version
-          source.
-    :attr str short_description: (optional) The short description for this script.
+    :param str type: (optional) The type of the script.
+    :param str path: (optional) The path to this script is within the current
+          version source.
+    :param str short_description: (optional) The short description for this script.
     """
 
     def __init__(
         self,
         *,
-        type: str = None,
-        path: str = None,
-        short_description: str = None,
+        type: Optional[str] = None,
+        path: Optional[str] = None,
+        short_description: Optional[str] = None,
     ) -> None:
         """
         Initialize a Script object.
 
         :param str type: (optional) The type of the script.
         :param str path: (optional) The path to this script is within the current
                version source.
@@ -8261,20 +8514,20 @@
         self.path = path
         self.short_description = short_description
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'Script':
         """Initialize a Script object from a json dictionary."""
         args = {}
-        if 'type' in _dict:
-            args['type'] = _dict.get('type')
-        if 'path' in _dict:
-            args['path'] = _dict.get('path')
-        if 'short_description' in _dict:
-            args['short_description'] = _dict.get('short_description')
+        if (type := _dict.get('type')) is not None:
+            args['type'] = type
+        if (path := _dict.get('path')) is not None:
+            args['path'] = path
+        if (short_description := _dict.get('short_description')) is not None:
+            args['short_description'] = short_description
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a Script object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8304,14 +8557,1120 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'Script') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class StackConfigMember:
+    """
+    A member deployable architecture that is included in your stack.
+
+    :param str name: The name matching the alias in the stack definition.
+    :param str config_id: The unique ID.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        config_id: str,
+    ) -> None:
+        """
+        Initialize a StackConfigMember object.
+
+        :param str name: The name matching the alias in the stack definition.
+        :param str config_id: The unique ID.
+        """
+        self.name = name
+        self.config_id = config_id
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackConfigMember':
+        """Initialize a StackConfigMember object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackConfigMember JSON')
+        if (config_id := _dict.get('config_id')) is not None:
+            args['config_id'] = config_id
+        else:
+            raise ValueError('Required property \'config_id\' not present in StackConfigMember JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackConfigMember object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'config_id') and self.config_id is not None:
+            _dict['config_id'] = self.config_id
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackConfigMember object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackConfigMember') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackConfigMember') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinition:
+    """
+    The stack definition.
+
+    :param str id: The ID of the stack definition.
+    :param datetime created_at: A date and time value in the format
+          YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
+          format as specified by RFC 3339.
+    :param datetime modified_at: A date and time value in the format
+          YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
+          format as specified by RFC 3339.
+    :param str state: The state for the stack definition.
+    :param StackDefinitionMetadataConfiguration configuration: The configuration
+          reference.
+    :param str href: A URL.
+    :param StackDefinitionBlock stack_definition: The definition block for a stack
+          definition.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        created_at: datetime,
+        modified_at: datetime,
+        state: str,
+        configuration: 'StackDefinitionMetadataConfiguration',
+        href: str,
+        stack_definition: 'StackDefinitionBlock',
+    ) -> None:
+        """
+        Initialize a StackDefinition object.
+
+        :param str id: The ID of the stack definition.
+        :param datetime created_at: A date and time value in the format
+               YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
+               format as specified by RFC 3339.
+        :param datetime modified_at: A date and time value in the format
+               YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
+               format as specified by RFC 3339.
+        :param str state: The state for the stack definition.
+        :param StackDefinitionMetadataConfiguration configuration: The
+               configuration reference.
+        :param str href: A URL.
+        :param StackDefinitionBlock stack_definition: The definition block for a
+               stack definition.
+        """
+        self.id = id
+        self.created_at = created_at
+        self.modified_at = modified_at
+        self.state = state
+        self.configuration = configuration
+        self.href = href
+        self.stack_definition = stack_definition
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinition':
+        """Initialize a StackDefinition object from a json dictionary."""
+        args = {}
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
+        else:
+            raise ValueError('Required property \'id\' not present in StackDefinition JSON')
+        if (created_at := _dict.get('created_at')) is not None:
+            args['created_at'] = string_to_datetime(created_at)
+        else:
+            raise ValueError('Required property \'created_at\' not present in StackDefinition JSON')
+        if (modified_at := _dict.get('modified_at')) is not None:
+            args['modified_at'] = string_to_datetime(modified_at)
+        else:
+            raise ValueError('Required property \'modified_at\' not present in StackDefinition JSON')
+        if (state := _dict.get('state')) is not None:
+            args['state'] = state
+        else:
+            raise ValueError('Required property \'state\' not present in StackDefinition JSON')
+        if (configuration := _dict.get('configuration')) is not None:
+            args['configuration'] = StackDefinitionMetadataConfiguration.from_dict(configuration)
+        else:
+            raise ValueError('Required property \'configuration\' not present in StackDefinition JSON')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
+        else:
+            raise ValueError('Required property \'href\' not present in StackDefinition JSON')
+        if (stack_definition := _dict.get('stack_definition')) is not None:
+            args['stack_definition'] = StackDefinitionBlock.from_dict(stack_definition)
+        else:
+            raise ValueError('Required property \'stack_definition\' not present in StackDefinition JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinition object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'created_at') and self.created_at is not None:
+            _dict['created_at'] = datetime_to_string(self.created_at)
+        if hasattr(self, 'modified_at') and self.modified_at is not None:
+            _dict['modified_at'] = datetime_to_string(self.modified_at)
+        if hasattr(self, 'state') and self.state is not None:
+            _dict['state'] = self.state
+        if hasattr(self, 'configuration') and self.configuration is not None:
+            if isinstance(self.configuration, dict):
+                _dict['configuration'] = self.configuration
+            else:
+                _dict['configuration'] = self.configuration.to_dict()
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        if hasattr(self, 'stack_definition') and self.stack_definition is not None:
+            if isinstance(self.stack_definition, dict):
+                _dict['stack_definition'] = self.stack_definition
+            else:
+                _dict['stack_definition'] = self.stack_definition.to_dict()
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinition object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinition') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinition') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+    class StateEnum(str, Enum):
+        """
+        The state for the stack definition.
+        """
+
+        DRAFT = 'draft'
+        PUBLISHED = 'published'
+
+
+class StackDefinitionBlock:
+    """
+    The definition block for a stack definition.
+
+    :param List[StackDefinitionInputVariable] inputs: (optional) Defines the inputs
+          that users need to configure at the stack level. These inputs are included in
+          the catalog entry when the deployable architecture stack is exported to a
+          private catalog.
+    :param List[StackDefinitionOutputVariable] outputs: (optional) The outputs
+          associated with this stack definition.
+    :param List[StackDefinitionMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    """
+
+    def __init__(
+        self,
+        *,
+        inputs: Optional[List['StackDefinitionInputVariable']] = None,
+        outputs: Optional[List['StackDefinitionOutputVariable']] = None,
+        members: Optional[List['StackDefinitionMember']] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionBlock object.
+
+        :param List[StackDefinitionInputVariable] inputs: (optional) Defines the
+               inputs that users need to configure at the stack level. These inputs are
+               included in the catalog entry when the deployable architecture stack is
+               exported to a private catalog.
+        :param List[StackDefinitionOutputVariable] outputs: (optional) The outputs
+               associated with this stack definition.
+        :param List[StackDefinitionMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        """
+        self.inputs = inputs
+        self.outputs = outputs
+        self.members = members
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionBlock':
+        """Initialize a StackDefinitionBlock object from a json dictionary."""
+        args = {}
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = [StackDefinitionInputVariable.from_dict(v) for v in inputs]
+        if (outputs := _dict.get('outputs')) is not None:
+            args['outputs'] = [StackDefinitionOutputVariable.from_dict(v) for v in outputs]
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackDefinitionMember.from_dict(v) for v in members]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionBlock object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            inputs_list = []
+            for v in self.inputs:
+                if isinstance(v, dict):
+                    inputs_list.append(v)
+                else:
+                    inputs_list.append(v.to_dict())
+            _dict['inputs'] = inputs_list
+        if hasattr(self, 'outputs') and self.outputs is not None:
+            outputs_list = []
+            for v in self.outputs:
+                if isinstance(v, dict):
+                    outputs_list.append(v)
+                else:
+                    outputs_list.append(v.to_dict())
+            _dict['outputs'] = outputs_list
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionBlock object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionBlock') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionBlock') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionBlockPrototype:
+    """
+    The definition block for a stack definition.
+
+    :param List[StackDefinitionInputVariable] inputs: (optional) Defines the inputs
+          that users need to configure at the stack level. These inputs are included in
+          the catalog entry when the deployable architecture stack is exported to a
+          private catalog.
+    :param List[StackDefinitionOutputVariable] outputs: (optional) The outputs
+          associated with this stack definition.
+    :param List[StackDefinitionMemberPrototype] members: (optional) Defines the
+          member deployable architectures that are included in your stack.
+    """
+
+    def __init__(
+        self,
+        *,
+        inputs: Optional[List['StackDefinitionInputVariable']] = None,
+        outputs: Optional[List['StackDefinitionOutputVariable']] = None,
+        members: Optional[List['StackDefinitionMemberPrototype']] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionBlockPrototype object.
+
+        :param List[StackDefinitionInputVariable] inputs: (optional) Defines the
+               inputs that users need to configure at the stack level. These inputs are
+               included in the catalog entry when the deployable architecture stack is
+               exported to a private catalog.
+        :param List[StackDefinitionOutputVariable] outputs: (optional) The outputs
+               associated with this stack definition.
+        :param List[StackDefinitionMemberPrototype] members: (optional) Defines the
+               member deployable architectures that are included in your stack.
+        """
+        self.inputs = inputs
+        self.outputs = outputs
+        self.members = members
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionBlockPrototype':
+        """Initialize a StackDefinitionBlockPrototype object from a json dictionary."""
+        args = {}
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = [StackDefinitionInputVariable.from_dict(v) for v in inputs]
+        if (outputs := _dict.get('outputs')) is not None:
+            args['outputs'] = [StackDefinitionOutputVariable.from_dict(v) for v in outputs]
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackDefinitionMemberPrototype.from_dict(v) for v in members]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionBlockPrototype object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            inputs_list = []
+            for v in self.inputs:
+                if isinstance(v, dict):
+                    inputs_list.append(v)
+                else:
+                    inputs_list.append(v.to_dict())
+            _dict['inputs'] = inputs_list
+        if hasattr(self, 'outputs') and self.outputs is not None:
+            outputs_list = []
+            for v in self.outputs:
+                if isinstance(v, dict):
+                    outputs_list.append(v)
+                else:
+                    outputs_list.append(v.to_dict())
+            _dict['outputs'] = outputs_list
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionBlockPrototype object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionBlockPrototype') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionBlockPrototype') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionExportRequest:
+    """
+    The payload for the stack definition export request.
+
+    """
+
+    def __init__(
+        self,
+    ) -> None:
+        """
+        Initialize a StackDefinitionExportRequest object.
+
+        """
+        msg = "Cannot instantiate base class. Instead, instantiate one of the defined subclasses: {0}".format(
+            ", ".join(
+                [
+                    'StackDefinitionExportRequestStackDefinitionExportCatalogRequest',
+                    'StackDefinitionExportRequestStackDefinitionExportProductRequest',
+                ]
+            )
+        )
+        raise Exception(msg)
+
+
+class StackDefinitionExportResponse:
+    """
+    The payload for the stack definition export response.
+
+    :param str catalog_id: (optional) The catalog ID to publish.
+    :param str product_id: (optional) The product ID to publish.
+    :param str version_locator: (optional) The version locator of the created
+          deployable architecture.
+    :param str kind: (optional) The product target kind value.
+    :param str format: (optional) The product format kind value.
+    """
+
+    def __init__(
+        self,
+        *,
+        catalog_id: Optional[str] = None,
+        product_id: Optional[str] = None,
+        version_locator: Optional[str] = None,
+        kind: Optional[str] = None,
+        format: Optional[str] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionExportResponse object.
+
+        :param str catalog_id: (optional) The catalog ID to publish.
+        :param str product_id: (optional) The product ID to publish.
+        :param str version_locator: (optional) The version locator of the created
+               deployable architecture.
+        :param str kind: (optional) The product target kind value.
+        :param str format: (optional) The product format kind value.
+        """
+        self.catalog_id = catalog_id
+        self.product_id = product_id
+        self.version_locator = version_locator
+        self.kind = kind
+        self.format = format
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionExportResponse':
+        """Initialize a StackDefinitionExportResponse object from a json dictionary."""
+        args = {}
+        if (catalog_id := _dict.get('catalog_id')) is not None:
+            args['catalog_id'] = catalog_id
+        if (product_id := _dict.get('product_id')) is not None:
+            args['product_id'] = product_id
+        if (version_locator := _dict.get('version_locator')) is not None:
+            args['version_locator'] = version_locator
+        if (kind := _dict.get('kind')) is not None:
+            args['kind'] = kind
+        if (format := _dict.get('format')) is not None:
+            args['format'] = format
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionExportResponse object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'catalog_id') and self.catalog_id is not None:
+            _dict['catalog_id'] = self.catalog_id
+        if hasattr(self, 'product_id') and self.product_id is not None:
+            _dict['product_id'] = self.product_id
+        if hasattr(self, 'version_locator') and self.version_locator is not None:
+            _dict['version_locator'] = self.version_locator
+        if hasattr(self, 'kind') and self.kind is not None:
+            _dict['kind'] = self.kind
+        if hasattr(self, 'format') and self.format is not None:
+            _dict['format'] = self.format
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionExportResponse object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionExportResponse') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionExportResponse') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionInputVariable:
+    """
+    The input variables for a stack definition.
+
+    :param str name: The stack definition input name.
+    :param str type: The variable type.
+    :param str description: (optional) The description of the variable.
+    :param object default: This property can be any value - a string, number,
+          boolean, array, or object.
+    :param bool required: (optional) A boolean value to denote if the property is
+          required.
+    :param bool hidden: (optional) A boolean value to denote whether the property is
+          hidden, as in not exposed to the user.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        type: str,
+        default: object,
+        *,
+        description: Optional[str] = None,
+        required: Optional[bool] = None,
+        hidden: Optional[bool] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionInputVariable object.
+
+        :param str name: The stack definition input name.
+        :param str type: The variable type.
+        :param object default: This property can be any value - a string, number,
+               boolean, array, or object.
+        :param str description: (optional) The description of the variable.
+        :param bool required: (optional) A boolean value to denote if the property
+               is required.
+        :param bool hidden: (optional) A boolean value to denote whether the
+               property is hidden, as in not exposed to the user.
+        """
+        self.name = name
+        self.type = type
+        self.description = description
+        self.default = default
+        self.required = required
+        self.hidden = hidden
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionInputVariable':
+        """Initialize a StackDefinitionInputVariable object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionInputVariable JSON')
+        if (type := _dict.get('type')) is not None:
+            args['type'] = type
+        else:
+            raise ValueError('Required property \'type\' not present in StackDefinitionInputVariable JSON')
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (default := _dict.get('default')) is not None:
+            args['default'] = default
+        else:
+            raise ValueError('Required property \'default\' not present in StackDefinitionInputVariable JSON')
+        if (required := _dict.get('required')) is not None:
+            args['required'] = required
+        if (hidden := _dict.get('hidden')) is not None:
+            args['hidden'] = hidden
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionInputVariable object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'type') and self.type is not None:
+            _dict['type'] = self.type
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'default') and self.default is not None:
+            _dict['default'] = self.default
+        if hasattr(self, 'required') and self.required is not None:
+            _dict['required'] = self.required
+        if hasattr(self, 'hidden') and self.hidden is not None:
+            _dict['hidden'] = self.hidden
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionInputVariable object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionInputVariable') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionInputVariable') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+    class TypeEnum(str, Enum):
+        """
+        The variable type.
+        """
+
+        ARRAY = 'array'
+        BOOLEAN = 'boolean'
+        FLOAT = 'float'
+        INT = 'int'
+        NUMBER = 'number'
+        PASSWORD = 'password'
+        STRING = 'string'
+        OBJECT = 'object'
+
+
+class StackDefinitionMember:
+    """
+    The member definition associated with this stack definition.
+
+    :param str name: The name matching the alias in the stack definition.
+    :param str version_locator: The version locator of the member deployable
+          architecture.
+    :param List[StackDefinitionMemberInput] inputs: (optional) The member input
+          names to use for the stack definition.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        version_locator: str,
+        *,
+        inputs: Optional[List['StackDefinitionMemberInput']] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionMember object.
+
+        :param str name: The name matching the alias in the stack definition.
+        :param str version_locator: The version locator of the member deployable
+               architecture.
+        :param List[StackDefinitionMemberInput] inputs: (optional) The member input
+               names to use for the stack definition.
+        """
+        self.name = name
+        self.version_locator = version_locator
+        self.inputs = inputs
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionMember':
+        """Initialize a StackDefinitionMember object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionMember JSON')
+        if (version_locator := _dict.get('version_locator')) is not None:
+            args['version_locator'] = version_locator
+        else:
+            raise ValueError('Required property \'version_locator\' not present in StackDefinitionMember JSON')
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = [StackDefinitionMemberInput.from_dict(v) for v in inputs]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionMember object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'version_locator') and self.version_locator is not None:
+            _dict['version_locator'] = self.version_locator
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            inputs_list = []
+            for v in self.inputs:
+                if isinstance(v, dict):
+                    inputs_list.append(v)
+                else:
+                    inputs_list.append(v.to_dict())
+            _dict['inputs'] = inputs_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionMember object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionMember') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionMember') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionMemberInput:
+    """
+    The member input definition.
+
+    :param str name: The member input name to use.
+    :param object value: The value of the stack definition output.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        value: object,
+    ) -> None:
+        """
+        Initialize a StackDefinitionMemberInput object.
+
+        :param str name: The member input name to use.
+        :param object value: The value of the stack definition output.
+        """
+        self.name = name
+        self.value = value
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionMemberInput':
+        """Initialize a StackDefinitionMemberInput object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionMemberInput JSON')
+        if (value := _dict.get('value')) is not None:
+            args['value'] = value
+        else:
+            raise ValueError('Required property \'value\' not present in StackDefinitionMemberInput JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionMemberInput object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'value') and self.value is not None:
+            _dict['value'] = self.value
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionMemberInput object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionMemberInput') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionMemberInput') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionMemberInputPrototype:
+    """
+    The member input definition.
+
+    :param str name: The member input name to use.
+    """
+
+    def __init__(
+        self,
+        name: str,
+    ) -> None:
+        """
+        Initialize a StackDefinitionMemberInputPrototype object.
+
+        :param str name: The member input name to use.
+        """
+        self.name = name
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionMemberInputPrototype':
+        """Initialize a StackDefinitionMemberInputPrototype object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionMemberInputPrototype JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionMemberInputPrototype object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionMemberInputPrototype object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionMemberInputPrototype') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionMemberInputPrototype') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionMemberPrototype:
+    """
+    Defines the input values from member deployable architectures that are included in the
+    catalog entry when the stack is exported to a private catalog.
+
+    :param str name: The name matching the alias in the stack definition.
+    :param List[StackDefinitionMemberInputPrototype] inputs: (optional) The member
+          input names to use for the deployable architecture stack definition.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        *,
+        inputs: Optional[List['StackDefinitionMemberInputPrototype']] = None,
+    ) -> None:
+        """
+        Initialize a StackDefinitionMemberPrototype object.
+
+        :param str name: The name matching the alias in the stack definition.
+        :param List[StackDefinitionMemberInputPrototype] inputs: (optional) The
+               member input names to use for the deployable architecture stack definition.
+        """
+        self.name = name
+        self.inputs = inputs
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionMemberPrototype':
+        """Initialize a StackDefinitionMemberPrototype object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionMemberPrototype JSON')
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = [StackDefinitionMemberInputPrototype.from_dict(v) for v in inputs]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionMemberPrototype object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            inputs_list = []
+            for v in self.inputs:
+                if isinstance(v, dict):
+                    inputs_list.append(v)
+                else:
+                    inputs_list.append(v.to_dict())
+            _dict['inputs'] = inputs_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionMemberPrototype object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionMemberPrototype') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionMemberPrototype') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionMetadataConfiguration:
+    """
+    The configuration reference.
+
+    :param str id: The unique ID.
+    :param str href: A URL.
+    :param ConfigDefinitionReference definition: The definition of the config
+          reference.
+    """
+
+    def __init__(
+        self,
+        id: str,
+        href: str,
+        definition: 'ConfigDefinitionReference',
+    ) -> None:
+        """
+        Initialize a StackDefinitionMetadataConfiguration object.
+
+        :param str id: The unique ID.
+        :param str href: A URL.
+        :param ConfigDefinitionReference definition: The definition of the config
+               reference.
+        """
+        self.id = id
+        self.href = href
+        self.definition = definition
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionMetadataConfiguration':
+        """Initialize a StackDefinitionMetadataConfiguration object from a json dictionary."""
+        args = {}
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
+        else:
+            raise ValueError('Required property \'id\' not present in StackDefinitionMetadataConfiguration JSON')
+        if (href := _dict.get('href')) is not None:
+            args['href'] = href
+        else:
+            raise ValueError('Required property \'href\' not present in StackDefinitionMetadataConfiguration JSON')
+        if (definition := _dict.get('definition')) is not None:
+            args['definition'] = ConfigDefinitionReference.from_dict(definition)
+        else:
+            raise ValueError(
+                'Required property \'definition\' not present in StackDefinitionMetadataConfiguration JSON'
+            )
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionMetadataConfiguration object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'id') and self.id is not None:
+            _dict['id'] = self.id
+        if hasattr(self, 'href') and self.href is not None:
+            _dict['href'] = self.href
+        if hasattr(self, 'definition') and self.definition is not None:
+            if isinstance(self.definition, dict):
+                _dict['definition'] = self.definition
+            else:
+                _dict['definition'] = self.definition.to_dict()
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionMetadataConfiguration object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionMetadataConfiguration') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionMetadataConfiguration') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionOutputVariable:
+    """
+    The output variables for a stack definition.
+
+    :param str name: The stack definition output name.
+    :param object value: The value of the stack definition output.
+    """
+
+    def __init__(
+        self,
+        name: str,
+        value: object,
+    ) -> None:
+        """
+        Initialize a StackDefinitionOutputVariable object.
+
+        :param str name: The stack definition output name.
+        :param object value: The value of the stack definition output.
+        """
+        self.name = name
+        self.value = value
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionOutputVariable':
+        """Initialize a StackDefinitionOutputVariable object from a json dictionary."""
+        args = {}
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        else:
+            raise ValueError('Required property \'name\' not present in StackDefinitionOutputVariable JSON')
+        if (value := _dict.get('value')) is not None:
+            args['value'] = value
+        else:
+            raise ValueError('Required property \'value\' not present in StackDefinitionOutputVariable JSON')
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionOutputVariable object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'value') and self.value is not None:
+            _dict['value'] = self.value
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionOutputVariable object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionOutputVariable') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionOutputVariable') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class TerraformLogAnalyzerErrorMessage:
     """
     The error message that is parsed by the Terraform log analyzer.
 
     """
 
     def __init__(
@@ -8375,25 +9734,25 @@
         return not self == other
 
 
 class TerraformLogAnalyzerSuccessMessage:
     """
     The success message that is parsed by the terraform log analyzer.
 
-    :attr str resource_type: (optional) The resource type.
-    :attr str time_taken: (optional) The time that is taken.
-    :attr str id: (optional) The ID.
+    :param str resource_type: (optional) The resource type.
+    :param str time_taken: (optional) The time that is taken.
+    :param str id: (optional) The ID.
     """
 
     def __init__(
         self,
         *,
-        resource_type: str = None,
-        time_taken: str = None,
-        id: str = None,
+        resource_type: Optional[str] = None,
+        time_taken: Optional[str] = None,
+        id: Optional[str] = None,
     ) -> None:
         """
         Initialize a TerraformLogAnalyzerSuccessMessage object.
 
         :param str resource_type: (optional) The resource type.
         :param str time_taken: (optional) The time that is taken.
         :param str id: (optional) The ID.
@@ -8402,20 +9761,20 @@
         self.time_taken = time_taken
         self.id = id
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'TerraformLogAnalyzerSuccessMessage':
         """Initialize a TerraformLogAnalyzerSuccessMessage object from a json dictionary."""
         args = {}
-        if 'resource_type' in _dict:
-            args['resource_type'] = _dict.get('resource_type')
-        if 'time-taken' in _dict:
-            args['time_taken'] = _dict.get('time-taken')
-        if 'id' in _dict:
-            args['id'] = _dict.get('id')
+        if (resource_type := _dict.get('resource_type')) is not None:
+            args['resource_type'] = resource_type
+        if (time_taken := _dict.get('time-taken')) is not None:
+            args['time_taken'] = time_taken
+        if (id := _dict.get('id')) is not None:
+            args['id'] = id
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a TerraformLogAnalyzerSuccessMessage object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8449,17 +9808,17 @@
         return not self == other
 
 
 class ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch(ProjectConfigDefinitionPatch):
     """
     The name and description of a project configuration.
 
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
-    :attr str locator_id: (optional) A unique concatenation of the catalog ID and
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
           > 1. If only a `locator_id` is specified, a new Schematics workspace is
@@ -8468,38 +9827,38 @@
           `locator_id` is not found in the existing schematics workspace.
           > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
           `400` message is returned if the specified `locator_id` does not agree with the
           `locator_id` in the existing Schematics workspace.
           > For more information of creating a Schematics workspace, see [Creating
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
-    :attr str description: (optional) A project configuration description.
-    :attr str name: (optional) The configuration name. It's unique within the
+    :param str description: (optional) A project configuration description.
+    :param str name: (optional) The configuration name. It's unique within the
           account across projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         *,
-        compliance_profile: 'ProjectComplianceProfile' = None,
-        locator_id: str = None,
-        description: str = None,
-        name: str = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
+        locator_id: Optional[str] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch object.
 
         :param ProjectComplianceProfile compliance_profile: (optional) The profile
                that is required for compliance.
         :param str locator_id: (optional) A unique concatenation of the catalog ID
@@ -8542,30 +9901,30 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch':
         """Initialize a ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch object from a json dictionary."""
         args = {}
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
-        if 'locator_id' in _dict:
-            args['locator_id'] = _dict.get('locator_id')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionPatchDAConfigDefinitionPropertiesPatch object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8615,39 +9974,39 @@
         return not self == other
 
 
 class ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch(ProjectConfigDefinitionPatch):
     """
     The name and description of a project configuration.
 
-    :attr List[str] resource_crns: (optional) The CRNs of the resources that are
+    :param List[str] resource_crns: (optional) The CRNs of the resources that are
           associated with this configuration.
-    :attr str description: (optional) A project configuration description.
-    :attr str name: (optional) The configuration name. It's unique within the
+    :param str description: (optional) A project configuration description.
+    :param str name: (optional) The configuration name. It's unique within the
           account across projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         *,
-        resource_crns: List[str] = None,
-        description: str = None,
-        name: str = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        resource_crns: Optional[List[str]] = None,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch object.
 
         :param List[str] resource_crns: (optional) The CRNs of the resources that
                are associated with this configuration.
         :param str description: (optional) A project configuration description.
@@ -8672,28 +10031,28 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch':
         """Initialize a ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch object from a json dictionary."""
         args = {}
-        if 'resource_crns' in _dict:
-            args['resource_crns'] = _dict.get('resource_crns')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (resource_crns := _dict.get('resource_crns')) is not None:
+            args['resource_crns'] = resource_crns
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionPatchResourceConfigDefinitionPropertiesPatch object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8738,17 +10097,17 @@
         return not self == other
 
 
 class ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype(ProjectConfigDefinitionPrototype):
     """
     The description of a project configuration.
 
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
-    :attr str locator_id: (optional) A unique concatenation of the catalog ID and
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
           > 1. If only a `locator_id` is specified, a new Schematics workspace is
@@ -8757,38 +10116,38 @@
           `locator_id` is not found in the existing schematics workspace.
           > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
           `400` message is returned if the specified `locator_id` does not agree with the
           `locator_id` in the existing Schematics workspace.
           > For more information of creating a Schematics workspace, see [Creating
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
-    :attr str description: (optional) A project configuration description.
-    :attr str name: The configuration name. It's unique within the account across
+    :param str description: (optional) A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
           projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         name: str,
         *,
-        compliance_profile: 'ProjectComplianceProfile' = None,
-        locator_id: str = None,
-        description: str = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
+        locator_id: Optional[str] = None,
+        description: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype object.
 
         :param str name: The configuration name. It's unique within the account
                across projects and regions.
         :param ProjectComplianceProfile compliance_profile: (optional) The profile
@@ -8831,34 +10190,34 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype':
         """Initialize a ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype object from a json dictionary."""
         args = {}
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
-        if 'locator_id' in _dict:
-            args['locator_id'] = _dict.get('locator_id')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError(
                 'Required property \'name\' not present in ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype JSON'
             )
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionPrototypeDAConfigDefinitionPropertiesPrototype object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -8908,39 +10267,39 @@
         return not self == other
 
 
 class ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype(ProjectConfigDefinitionPrototype):
     """
     The description of a project configuration.
 
-    :attr List[str] resource_crns: (optional) The CRNs of the resources that are
+    :param List[str] resource_crns: (optional) The CRNs of the resources that are
           associated with this configuration.
-    :attr str description: (optional) A project configuration description.
-    :attr str name: The configuration name. It's unique within the account across
+    :param str description: (optional) A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
           projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         name: str,
         *,
-        resource_crns: List[str] = None,
-        description: str = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        resource_crns: Optional[List[str]] = None,
+        description: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype object.
 
         :param str name: The configuration name. It's unique within the account
                across projects and regions.
         :param List[str] resource_crns: (optional) The CRNs of the resources that
@@ -8965,32 +10324,32 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype':
         """Initialize a ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype object from a json dictionary."""
         args = {}
-        if 'resource_crns' in _dict:
-            args['resource_crns'] = _dict.get('resource_crns')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (resource_crns := _dict.get('resource_crns')) is not None:
+            args['resource_crns'] = resource_crns
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError(
                 'Required property \'name\' not present in ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype JSON'
             )
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -9031,21 +10390,164 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectConfigDefinitionPrototypeResourceConfigDefinitionPropertiesPrototype') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties(ProjectConfigDefinitionPrototype):
+    """
+    The description of a project configuration.
+
+    :param str description: (optional) A project configuration description.
+    :param str name: (optional) The configuration name. It's unique within the
+          account across projects and regions.
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
+          the version ID that identify the deployable architecture in the catalog. I
+          you're importing from an existing Schematics workspace that is not backed by
+          cart, a `locator_id` is required. If you're using a Schematics workspace that is
+          backed by cart, a `locator_id` is not necessary because the Schematics workspace
+          has one.
+          > There are 3 scenarios:
+          > 1. If only a `locator_id` is specified, a new Schematics workspace is
+          instantiated with that `locator_id`.
+          > 2. If only a schematics `workspace_crn` is specified, a `400` is returned if a
+          `locator_id` is not found in the existing schematics workspace.
+          > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
+          `400` message is returned if the specified `locator_id` does not agree with the
+          `locator_id` in the existing Schematics workspace.
+          > For more information of creating a Schematics workspace, see [Creating
+          workspaces and importing your Terraform
+          template](/docs/schematics?topic=schematics-sch-create-wks).
+    :param str environment_id: (optional) The ID of the project environment.
+    :param dict inputs: (optional) The input variables that are used for
+          configuration definition and environment.
+    :param List[StackConfigMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    """
+
+    def __init__(
+        self,
+        *,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        locator_id: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        inputs: Optional[dict] = None,
+        members: Optional[List['StackConfigMember']] = None,
+    ) -> None:
+        """
+        Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object.
+
+        :param str description: (optional) A project configuration description.
+        :param str name: (optional) The configuration name. It's unique within the
+               account across projects and regions.
+        :param str locator_id: (optional) A unique concatenation of the catalog ID
+               and the version ID that identify the deployable architecture in the
+               catalog. I you're importing from an existing Schematics workspace that is
+               not backed by cart, a `locator_id` is required. If you're using a
+               Schematics workspace that is backed by cart, a `locator_id` is not
+               necessary because the Schematics workspace has one.
+               > There are 3 scenarios:
+               > 1. If only a `locator_id` is specified, a new Schematics workspace is
+               instantiated with that `locator_id`.
+               > 2. If only a schematics `workspace_crn` is specified, a `400` is returned
+               if a `locator_id` is not found in the existing schematics workspace.
+               > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified,
+               a `400` message is returned if the specified `locator_id` does not agree
+               with the `locator_id` in the existing Schematics workspace.
+               > For more information of creating a Schematics workspace, see [Creating
+               workspaces and importing your Terraform
+               template](/docs/schematics?topic=schematics-sch-create-wks).
+        :param str environment_id: (optional) The ID of the project environment.
+        :param dict inputs: (optional) The input variables that are used for
+               configuration definition and environment.
+        :param List[StackConfigMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        """
+        # pylint: disable=super-init-not-called
+        self.description = description
+        self.name = name
+        self.locator_id = locator_id
+        self.environment_id = environment_id
+        self.inputs = inputs
+        self.members = members
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties':
+        """Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object from a json dictionary."""
+        args = {}
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'locator_id') and self.locator_id is not None:
+            _dict['locator_id'] = self.locator_id
+        if hasattr(self, 'environment_id') and self.environment_id is not None:
+            _dict['environment_id'] = self.environment_id
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            _dict['inputs'] = self.inputs
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ProjectConfigDefinitionPrototypeStackConfigDefinitionProperties') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse(ProjectConfigDefinitionResponse):
     """
     The description of a project configuration.
 
-    :attr ProjectComplianceProfile compliance_profile: (optional) The profile that
+    :param ProjectComplianceProfile compliance_profile: (optional) The profile that
           is required for compliance.
-    :attr str locator_id: (optional) A unique concatenation of the catalog ID and
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
           the version ID that identify the deployable architecture in the catalog. I
           you're importing from an existing Schematics workspace that is not backed by
           cart, a `locator_id` is required. If you're using a Schematics workspace that is
           backed by cart, a `locator_id` is not necessary because the Schematics workspace
           has one.
           > There are 3 scenarios:
           > 1. If only a `locator_id` is specified, a new Schematics workspace is
@@ -9054,38 +10556,38 @@
           `locator_id` is not found in the existing schematics workspace.
           > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
           `400` message is returned if the specified `locator_id` does not agree with the
           `locator_id` in the existing Schematics workspace.
           > For more information of creating a Schematics workspace, see [Creating
           workspaces and importing your Terraform
           template](/docs/schematics?topic=schematics-sch-create-wks).
-    :attr str description: A project configuration description.
-    :attr str name: The configuration name. It's unique within the account across
+    :param str description: A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
           projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         description: str,
         name: str,
         *,
-        compliance_profile: 'ProjectComplianceProfile' = None,
-        locator_id: str = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        compliance_profile: Optional['ProjectComplianceProfile'] = None,
+        locator_id: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse object.
 
         :param str description: A project configuration description.
         :param str name: The configuration name. It's unique within the account
                across projects and regions.
@@ -9128,38 +10630,38 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse':
         """Initialize a ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse object from a json dictionary."""
         args = {}
-        if 'compliance_profile' in _dict:
-            args['compliance_profile'] = ProjectComplianceProfile.from_dict(_dict.get('compliance_profile'))
-        if 'locator_id' in _dict:
-            args['locator_id'] = _dict.get('locator_id')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (compliance_profile := _dict.get('compliance_profile')) is not None:
+            args['compliance_profile'] = ProjectComplianceProfile.from_dict(compliance_profile)
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError(
                 'Required property \'description\' not present in ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse JSON'
             )
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError(
                 'Required property \'name\' not present in ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse JSON'
             )
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionResponseDAConfigDefinitionPropertiesResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -9209,39 +10711,39 @@
         return not self == other
 
 
 class ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse(ProjectConfigDefinitionResponse):
     """
     The description of a project configuration.
 
-    :attr List[str] resource_crns: (optional) The CRNs of the resources that are
+    :param List[str] resource_crns: (optional) The CRNs of the resources that are
           associated with this configuration.
-    :attr str description: A project configuration description.
-    :attr str name: The configuration name. It's unique within the account across
+    :param str description: A project configuration description.
+    :param str name: The configuration name. It's unique within the account across
           projects and regions.
-    :attr str environment_id: (optional) The ID of the project environment.
-    :attr ProjectConfigAuth authorizations: (optional) The authorization details.
+    :param str environment_id: (optional) The ID of the project environment.
+    :param ProjectConfigAuth authorizations: (optional) The authorization details.
           You can authorize by using a trusted profile or an API key in Secrets Manager.
-    :attr dict inputs: (optional) The input variables that are used for
+    :param dict inputs: (optional) The input variables that are used for
           configuration definition and environment.
-    :attr dict settings: (optional) The Schematics environment variables to use to
+    :param dict settings: (optional) The Schematics environment variables to use to
           deploy the configuration. Settings are only available if they are specified when
           the configuration is initially created.
     """
 
     def __init__(
         self,
         description: str,
         name: str,
         *,
-        resource_crns: List[str] = None,
-        environment_id: str = None,
-        authorizations: 'ProjectConfigAuth' = None,
-        inputs: dict = None,
-        settings: dict = None,
+        resource_crns: Optional[List[str]] = None,
+        environment_id: Optional[str] = None,
+        authorizations: Optional['ProjectConfigAuth'] = None,
+        inputs: Optional[dict] = None,
+        settings: Optional[dict] = None,
     ) -> None:
         """
         Initialize a ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse object.
 
         :param str description: A project configuration description.
         :param str name: The configuration name. It's unique within the account
                across projects and regions.
@@ -9266,36 +10768,36 @@
         self.inputs = inputs
         self.settings = settings
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse':
         """Initialize a ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse object from a json dictionary."""
         args = {}
-        if 'resource_crns' in _dict:
-            args['resource_crns'] = _dict.get('resource_crns')
-        if 'description' in _dict:
-            args['description'] = _dict.get('description')
+        if (resource_crns := _dict.get('resource_crns')) is not None:
+            args['resource_crns'] = resource_crns
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
         else:
             raise ValueError(
                 'Required property \'description\' not present in ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse JSON'
             )
-        if 'name' in _dict:
-            args['name'] = _dict.get('name')
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
         else:
             raise ValueError(
                 'Required property \'name\' not present in ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse JSON'
             )
-        if 'environment_id' in _dict:
-            args['environment_id'] = _dict.get('environment_id')
-        if 'authorizations' in _dict:
-            args['authorizations'] = ProjectConfigAuth.from_dict(_dict.get('authorizations'))
-        if 'inputs' in _dict:
-            args['inputs'] = _dict.get('inputs')
-        if 'settings' in _dict:
-            args['settings'] = _dict.get('settings')
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (authorizations := _dict.get('authorizations')) is not None:
+            args['authorizations'] = ProjectConfigAuth.from_dict(authorizations)
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (settings := _dict.get('settings')) is not None:
+            args['settings'] = settings
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -9336,41 +10838,184 @@
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other: 'ProjectConfigDefinitionResponseResourceConfigDefinitionPropertiesResponse') -> bool:
         """Return `true` when self and other are not equal, false otherwise."""
         return not self == other
 
 
+class ProjectConfigDefinitionResponseStackConfigDefinitionProperties(ProjectConfigDefinitionResponse):
+    """
+    The description of a project configuration.
+
+    :param str description: (optional) A project configuration description.
+    :param str name: (optional) The configuration name. It's unique within the
+          account across projects and regions.
+    :param str locator_id: (optional) A unique concatenation of the catalog ID and
+          the version ID that identify the deployable architecture in the catalog. I
+          you're importing from an existing Schematics workspace that is not backed by
+          cart, a `locator_id` is required. If you're using a Schematics workspace that is
+          backed by cart, a `locator_id` is not necessary because the Schematics workspace
+          has one.
+          > There are 3 scenarios:
+          > 1. If only a `locator_id` is specified, a new Schematics workspace is
+          instantiated with that `locator_id`.
+          > 2. If only a schematics `workspace_crn` is specified, a `400` is returned if a
+          `locator_id` is not found in the existing schematics workspace.
+          > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified, a
+          `400` message is returned if the specified `locator_id` does not agree with the
+          `locator_id` in the existing Schematics workspace.
+          > For more information of creating a Schematics workspace, see [Creating
+          workspaces and importing your Terraform
+          template](/docs/schematics?topic=schematics-sch-create-wks).
+    :param str environment_id: (optional) The ID of the project environment.
+    :param dict inputs: (optional) The input variables that are used for
+          configuration definition and environment.
+    :param List[StackConfigMember] members: (optional) The member deployabe
+          architectures that are included in your stack.
+    """
+
+    def __init__(
+        self,
+        *,
+        description: Optional[str] = None,
+        name: Optional[str] = None,
+        locator_id: Optional[str] = None,
+        environment_id: Optional[str] = None,
+        inputs: Optional[dict] = None,
+        members: Optional[List['StackConfigMember']] = None,
+    ) -> None:
+        """
+        Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object.
+
+        :param str description: (optional) A project configuration description.
+        :param str name: (optional) The configuration name. It's unique within the
+               account across projects and regions.
+        :param str locator_id: (optional) A unique concatenation of the catalog ID
+               and the version ID that identify the deployable architecture in the
+               catalog. I you're importing from an existing Schematics workspace that is
+               not backed by cart, a `locator_id` is required. If you're using a
+               Schematics workspace that is backed by cart, a `locator_id` is not
+               necessary because the Schematics workspace has one.
+               > There are 3 scenarios:
+               > 1. If only a `locator_id` is specified, a new Schematics workspace is
+               instantiated with that `locator_id`.
+               > 2. If only a schematics `workspace_crn` is specified, a `400` is returned
+               if a `locator_id` is not found in the existing schematics workspace.
+               > 3. If both a Schematics `workspace_crn` and a `locator_id` are specified,
+               a `400` message is returned if the specified `locator_id` does not agree
+               with the `locator_id` in the existing Schematics workspace.
+               > For more information of creating a Schematics workspace, see [Creating
+               workspaces and importing your Terraform
+               template](/docs/schematics?topic=schematics-sch-create-wks).
+        :param str environment_id: (optional) The ID of the project environment.
+        :param dict inputs: (optional) The input variables that are used for
+               configuration definition and environment.
+        :param List[StackConfigMember] members: (optional) The member deployabe
+               architectures that are included in your stack.
+        """
+        # pylint: disable=super-init-not-called
+        self.description = description
+        self.name = name
+        self.locator_id = locator_id
+        self.environment_id = environment_id
+        self.inputs = inputs
+        self.members = members
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'ProjectConfigDefinitionResponseStackConfigDefinitionProperties':
+        """Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object from a json dictionary."""
+        args = {}
+        if (description := _dict.get('description')) is not None:
+            args['description'] = description
+        if (name := _dict.get('name')) is not None:
+            args['name'] = name
+        if (locator_id := _dict.get('locator_id')) is not None:
+            args['locator_id'] = locator_id
+        if (environment_id := _dict.get('environment_id')) is not None:
+            args['environment_id'] = environment_id
+        if (inputs := _dict.get('inputs')) is not None:
+            args['inputs'] = inputs
+        if (members := _dict.get('members')) is not None:
+            args['members'] = [StackConfigMember.from_dict(v) for v in members]
+        return cls(**args)
+
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a ProjectConfigDefinitionResponseStackConfigDefinitionProperties object from a json dictionary."""
+        return cls.from_dict(_dict)
+
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'description') and self.description is not None:
+            _dict['description'] = self.description
+        if hasattr(self, 'name') and self.name is not None:
+            _dict['name'] = self.name
+        if hasattr(self, 'locator_id') and self.locator_id is not None:
+            _dict['locator_id'] = self.locator_id
+        if hasattr(self, 'environment_id') and self.environment_id is not None:
+            _dict['environment_id'] = self.environment_id
+        if hasattr(self, 'inputs') and self.inputs is not None:
+            _dict['inputs'] = self.inputs
+        if hasattr(self, 'members') and self.members is not None:
+            members_list = []
+            for v in self.members:
+                if isinstance(v, dict):
+                    members_list.append(v)
+                else:
+                    members_list.append(v.to_dict())
+            _dict['members'] = members_list
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this ProjectConfigDefinitionResponseStackConfigDefinitionProperties object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'ProjectConfigDefinitionResponseStackConfigDefinitionProperties') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'ProjectConfigDefinitionResponseStackConfigDefinitionProperties') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
 class ProjectConfigMetadataCodeRiskAnalyzerLogsVersion204(ProjectConfigMetadataCodeRiskAnalyzerLogs):
     """
     The Code Risk Analyzer logs of the configuration based on Code Risk Analyzer version
     2.0.4.
 
-    :attr str cra_version: (optional) The version of the Code Risk Analyzer logs of
+    :param str cra_version: (optional) The version of the Code Risk Analyzer logs of
           the configuration. The metadata for this schema is specific to Code Risk
           Analyzer version 2.0.4.
-    :attr str schema_version: (optional) The schema version of Code Risk Analyzer
+    :param str schema_version: (optional) The schema version of Code Risk Analyzer
           logs of the configuration.
-    :attr str status: (optional) The status of the Code Risk Analyzer logs of the
+    :param str status: (optional) The status of the Code Risk Analyzer logs of the
           configuration.
-    :attr CodeRiskAnalyzerLogsSummary summary: (optional) The Code Risk Analyzer
+    :param CodeRiskAnalyzerLogsSummary summary: (optional) The Code Risk Analyzer
           logs a summary of the configuration.
-    :attr datetime timestamp: (optional) A date and time value in the format
+    :param datetime timestamp: (optional) A date and time value in the format
           YYYY-MM-DDTHH:mm:ssZ or YYYY-MM-DDTHH:mm:ss.sssZ to match the date and time
           format as specified by RFC 3339.
     """
 
     def __init__(
         self,
         *,
-        cra_version: str = None,
-        schema_version: str = None,
-        status: str = None,
-        summary: 'CodeRiskAnalyzerLogsSummary' = None,
-        timestamp: datetime = None,
+        cra_version: Optional[str] = None,
+        schema_version: Optional[str] = None,
+        status: Optional[str] = None,
+        summary: Optional['CodeRiskAnalyzerLogsSummary'] = None,
+        timestamp: Optional[datetime] = None,
     ) -> None:
         """
         Initialize a ProjectConfigMetadataCodeRiskAnalyzerLogsVersion204 object.
 
         :param str cra_version: (optional) The version of the Code Risk Analyzer
                logs of the configuration. The metadata for this schema is specific to Code
                Risk Analyzer version 2.0.4.
@@ -9391,24 +11036,24 @@
         self.summary = summary
         self.timestamp = timestamp
 
     @classmethod
     def from_dict(cls, _dict: Dict) -> 'ProjectConfigMetadataCodeRiskAnalyzerLogsVersion204':
         """Initialize a ProjectConfigMetadataCodeRiskAnalyzerLogsVersion204 object from a json dictionary."""
         args = {}
-        if 'cra_version' in _dict:
-            args['cra_version'] = _dict.get('cra_version')
-        if 'schema_version' in _dict:
-            args['schema_version'] = _dict.get('schema_version')
-        if 'status' in _dict:
-            args['status'] = _dict.get('status')
-        if 'summary' in _dict:
-            args['summary'] = CodeRiskAnalyzerLogsSummary.from_dict(_dict.get('summary'))
-        if 'timestamp' in _dict:
-            args['timestamp'] = string_to_datetime(_dict.get('timestamp'))
+        if (cra_version := _dict.get('cra_version')) is not None:
+            args['cra_version'] = cra_version
+        if (schema_version := _dict.get('schema_version')) is not None:
+            args['schema_version'] = schema_version
+        if (status := _dict.get('status')) is not None:
+            args['status'] = status
+        if (summary := _dict.get('summary')) is not None:
+            args['summary'] = CodeRiskAnalyzerLogsSummary.from_dict(summary)
+        if (timestamp := _dict.get('timestamp')) is not None:
+            args['timestamp'] = string_to_datetime(timestamp)
         return cls(**args)
 
     @classmethod
     def _from_dict(cls, _dict):
         """Initialize a ProjectConfigMetadataCodeRiskAnalyzerLogsVersion204 object from a json dictionary."""
         return cls.from_dict(_dict)
 
@@ -9453,146 +11098,277 @@
         The status of the Code Risk Analyzer logs of the configuration.
         """
 
         PASSED = 'passed'
         FAILED = 'failed'
 
 
-##############################################################################
-# Pagers
-##############################################################################
-
-
-class ProjectsPager:
+class StackDefinitionExportRequestStackDefinitionExportCatalogRequest(StackDefinitionExportRequest):
     """
-    ProjectsPager can be used to simplify the use of the "list_projects" method.
+    The payload for the stack definition export request to create a product.
+
+    :param str catalog_id: The catalog ID to publish.
+    :param str target_version: (optional) The semver value of this new version of
+          the product.
+    :param str variation: (optional) The variation of this new version of the
+          product.
+    :param str label: The product label.
+    :param List[str] tags: (optional) Tags associated with the catalog product.
     """
 
     def __init__(
         self,
+        catalog_id: str,
+        label: str,
         *,
-        client: ProjectV1,
-        limit: int = None,
+        target_version: Optional[str] = None,
+        variation: Optional[str] = None,
+        tags: Optional[List[str]] = None,
     ) -> None:
         """
-        Initialize a ProjectsPager object.
-        :param int limit: (optional) The maximum number of resources to return. The
-               number of resources that are returned is the same, except for the last
-               page.
-        """
-        self._has_next = True
-        self._client = client
-        self._page_context = {'next': None}
-        self._limit = limit
+        Initialize a StackDefinitionExportRequestStackDefinitionExportCatalogRequest object.
 
-    def has_next(self) -> bool:
+        :param str catalog_id: The catalog ID to publish.
+        :param str label: The product label.
+        :param str target_version: (optional) The semver value of this new version
+               of the product.
+        :param str variation: (optional) The variation of this new version of the
+               product.
+        :param List[str] tags: (optional) Tags associated with the catalog product.
         """
-        Returns true if there are potentially more results to be retrieved.
-        """
-        return self._has_next
+        # pylint: disable=super-init-not-called
+        self.catalog_id = catalog_id
+        self.target_version = target_version
+        self.variation = variation
+        self.label = label
+        self.tags = tags
 
-    def get_next(self) -> List[dict]:
-        """
-        Returns the next page of results.
-        :return: A List[dict], where each element is a dict that represents an instance of ProjectSummary.
-        :rtype: List[dict]
-        """
-        if not self.has_next():
-            raise StopIteration(message='No more results available')
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionExportRequestStackDefinitionExportCatalogRequest':
+        """Initialize a StackDefinitionExportRequestStackDefinitionExportCatalogRequest object from a json dictionary."""
+        args = {}
+        if (catalog_id := _dict.get('catalog_id')) is not None:
+            args['catalog_id'] = catalog_id
+        else:
+            raise ValueError(
+                'Required property \'catalog_id\' not present in StackDefinitionExportRequestStackDefinitionExportCatalogRequest JSON'
+            )
+        if (target_version := _dict.get('target_version')) is not None:
+            args['target_version'] = target_version
+        if (variation := _dict.get('variation')) is not None:
+            args['variation'] = variation
+        if (label := _dict.get('label')) is not None:
+            args['label'] = label
+        else:
+            raise ValueError(
+                'Required property \'label\' not present in StackDefinitionExportRequestStackDefinitionExportCatalogRequest JSON'
+            )
+        if (tags := _dict.get('tags')) is not None:
+            args['tags'] = tags
+        return cls(**args)
 
-        result = self._client.list_projects(
-            limit=self._limit,
-            token=self._page_context.get('next'),
-        ).get_result()
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionExportRequestStackDefinitionExportCatalogRequest object from a json dictionary."""
+        return cls.from_dict(_dict)
 
-        next = None
-        next_page_link = result.get('next')
-        if next_page_link is not None:
-            next = get_query_param(next_page_link.get('href'), 'token')
-        self._page_context['next'] = next
-        if next is None:
-            self._has_next = False
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'catalog_id') and self.catalog_id is not None:
+            _dict['catalog_id'] = self.catalog_id
+        if hasattr(self, 'target_version') and self.target_version is not None:
+            _dict['target_version'] = self.target_version
+        if hasattr(self, 'variation') and self.variation is not None:
+            _dict['variation'] = self.variation
+        if hasattr(self, 'label') and self.label is not None:
+            _dict['label'] = self.label
+        if hasattr(self, 'tags') and self.tags is not None:
+            _dict['tags'] = self.tags
+        return _dict
 
-        return result.get('projects')
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
 
-    def get_all(self) -> List[dict]:
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionExportRequestStackDefinitionExportCatalogRequest object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionExportRequestStackDefinitionExportCatalogRequest') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionExportRequestStackDefinitionExportCatalogRequest') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+class StackDefinitionExportRequestStackDefinitionExportProductRequest(StackDefinitionExportRequest):
+    """
+    The payload for the stack definition export request to create a new product version.
+
+    :param str catalog_id: The catalog ID to publish.
+    :param str target_version: The semver value of this new version of the product.
+    :param str variation: (optional) The variation of this new version of the
+          product.
+    :param str product_id: The product ID to publish.
+    """
+
+    def __init__(
+        self,
+        catalog_id: str,
+        target_version: str,
+        product_id: str,
+        *,
+        variation: Optional[str] = None,
+    ) -> None:
         """
-        Returns all results by invoking get_next() repeatedly
-        until all pages of results have been retrieved.
-        :return: A List[dict], where each element is a dict that represents an instance of ProjectSummary.
-        :rtype: List[dict]
+        Initialize a StackDefinitionExportRequestStackDefinitionExportProductRequest object.
+
+        :param str catalog_id: The catalog ID to publish.
+        :param str target_version: The semver value of this new version of the
+               product.
+        :param str product_id: The product ID to publish.
+        :param str variation: (optional) The variation of this new version of the
+               product.
         """
-        results = []
-        while self.has_next():
-            next_page = self.get_next()
-            results.extend(next_page)
-        return results
+        # pylint: disable=super-init-not-called
+        self.catalog_id = catalog_id
+        self.target_version = target_version
+        self.variation = variation
+        self.product_id = product_id
+
+    @classmethod
+    def from_dict(cls, _dict: Dict) -> 'StackDefinitionExportRequestStackDefinitionExportProductRequest':
+        """Initialize a StackDefinitionExportRequestStackDefinitionExportProductRequest object from a json dictionary."""
+        args = {}
+        if (catalog_id := _dict.get('catalog_id')) is not None:
+            args['catalog_id'] = catalog_id
+        else:
+            raise ValueError(
+                'Required property \'catalog_id\' not present in StackDefinitionExportRequestStackDefinitionExportProductRequest JSON'
+            )
+        if (target_version := _dict.get('target_version')) is not None:
+            args['target_version'] = target_version
+        else:
+            raise ValueError(
+                'Required property \'target_version\' not present in StackDefinitionExportRequestStackDefinitionExportProductRequest JSON'
+            )
+        if (variation := _dict.get('variation')) is not None:
+            args['variation'] = variation
+        if (product_id := _dict.get('product_id')) is not None:
+            args['product_id'] = product_id
+        else:
+            raise ValueError(
+                'Required property \'product_id\' not present in StackDefinitionExportRequestStackDefinitionExportProductRequest JSON'
+            )
+        return cls(**args)
 
+    @classmethod
+    def _from_dict(cls, _dict):
+        """Initialize a StackDefinitionExportRequestStackDefinitionExportProductRequest object from a json dictionary."""
+        return cls.from_dict(_dict)
 
-class ProjectResourcesPager:
+    def to_dict(self) -> Dict:
+        """Return a json dictionary representing this model."""
+        _dict = {}
+        if hasattr(self, 'catalog_id') and self.catalog_id is not None:
+            _dict['catalog_id'] = self.catalog_id
+        if hasattr(self, 'target_version') and self.target_version is not None:
+            _dict['target_version'] = self.target_version
+        if hasattr(self, 'variation') and self.variation is not None:
+            _dict['variation'] = self.variation
+        if hasattr(self, 'product_id') and self.product_id is not None:
+            _dict['product_id'] = self.product_id
+        return _dict
+
+    def _to_dict(self):
+        """Return a json dictionary representing this model."""
+        return self.to_dict()
+
+    def __str__(self) -> str:
+        """Return a `str` version of this StackDefinitionExportRequestStackDefinitionExportProductRequest object."""
+        return json.dumps(self.to_dict(), indent=2)
+
+    def __eq__(self, other: 'StackDefinitionExportRequestStackDefinitionExportProductRequest') -> bool:
+        """Return `true` when self and other are equal, false otherwise."""
+        if not isinstance(other, self.__class__):
+            return False
+        return self.__dict__ == other.__dict__
+
+    def __ne__(self, other: 'StackDefinitionExportRequestStackDefinitionExportProductRequest') -> bool:
+        """Return `true` when self and other are not equal, false otherwise."""
+        return not self == other
+
+
+##############################################################################
+# Pagers
+##############################################################################
+
+
+class ProjectsPager:
     """
-    ProjectResourcesPager can be used to simplify the use of the "list_project_resources" method.
+    ProjectsPager can be used to simplify the use of the "list_projects" method.
     """
 
     def __init__(
         self,
         *,
         client: ProjectV1,
-        id: str,
         limit: int = None,
     ) -> None:
         """
-        Initialize a ProjectResourcesPager object.
-        :param str id: The unique project ID.
+        Initialize a ProjectsPager object.
         :param int limit: (optional) The maximum number of resources to return. The
                number of resources that are returned is the same, except for the last
                page.
         """
         self._has_next = True
         self._client = client
         self._page_context = {'next': None}
-        self._id = id
         self._limit = limit
 
     def has_next(self) -> bool:
         """
         Returns true if there are potentially more results to be retrieved.
         """
         return self._has_next
 
     def get_next(self) -> List[dict]:
         """
         Returns the next page of results.
-        :return: A List[dict], where each element is a dict that represents an instance of ProjectResourceSummary.
+        :return: A List[dict], where each element is a dict that represents an instance of ProjectSummary.
         :rtype: List[dict]
         """
         if not self.has_next():
             raise StopIteration(message='No more results available')
 
-        result = self._client.list_project_resources(
-            id=self._id,
+        result = self._client.list_projects(
             limit=self._limit,
-            start=self._page_context.get('next'),
+            token=self._page_context.get('next'),
         ).get_result()
 
         next = None
         next_page_link = result.get('next')
         if next_page_link is not None:
-            next = get_query_param(next_page_link.get('href'), 'start')
+            next = get_query_param(next_page_link.get('href'), 'token')
         self._page_context['next'] = next
         if next is None:
             self._has_next = False
 
-        return result.get('resources')
+        return result.get('projects')
 
     def get_all(self) -> List[dict]:
         """
         Returns all results by invoking get_next() repeatedly
         until all pages of results have been retrieved.
-        :return: A List[dict], where each element is a dict that represents an instance of ProjectResourceSummary.
+        :return: A List[dict], where each element is a dict that represents an instance of ProjectSummary.
         :rtype: List[dict]
         """
         results = []
         while self.has_next():
             next_page = self.get_next()
             results.extend(next_page)
         return results
```

### Comparing `ibm-project-sdk-0.0.4/ibm_project_sdk/version.py` & `ibm-project-sdk-0.0.5/ibm_project_sdk/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 Version of project
 """
-__version__ = '0.0.4'
+__version__ = '0.0.5'
```

### Comparing `ibm-project-sdk-0.0.4/ibm_project_sdk.egg-info/PKG-INFO` & `ibm-project-sdk-0.0.5/ibm_project_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-project-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: Project Services Python SDK
 Home-page: https://github.com/IBM/project-python-sdk
 Author: IBM
 Author-email: dvesperini@gmail.com
 License: Apache 2.0
 Keywords: ibm_project_sdk
 Platform: UNKNOWN
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Build Status](https://api.travis-ci.com/IBM/project-python-sdk.svg?branch=main)](https://app.travis-ci.com/github/IBM/project-python-sdk)
 [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
-# Project Services Python SDK Version 0.0.4
+# Project Services Python SDK Version 0.0.5
 
 Python client library to interact with various [IBM Cloud Platform Services APIs](https://cloud.ibm.com/apidocs?category=platform-services).
 
 Disclaimer: this SDK is being released initially as a **pre-release** version.
 Changes might occur which impact applications that use this SDK.
 
 ## Table of Contents
@@ -76,15 +76,15 @@
 * Python 3.7 or above.
 
 ## Installation
 
 To install, use `pip`:
 
 ```bash
-pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.4
+pip install --upgrade git+https://github.com/IBM/project-python-sdk@v0.0.5
 ```
 
 Then in your code, you can import the appropriate service like this:
 ```
 from ibm_project_sdk.project_v1 import *
 ```
 where `<service-module-name>` is the service's module name from the table above
```

### Comparing `ibm-project-sdk-0.0.4/setup.py` & `ibm-project-sdk-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os
 import sys
 import pkg_resources
 
-__version__ = '0.0.4'
+__version__ = '0.0.5'
 PACKAGE_NAME = 'ibm_project_sdk'
 PACKAGE_DESC = 'Project Services Python SDK'
 
 with open('requirements.txt') as f:
     install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 with open('requirements-dev.txt') as f:
     tests_require = [str(req) for req in pkg_resources.parse_requirements(f)]
```

