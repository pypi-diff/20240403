# Comparing `tmp/trustauthx-0.6.3.tar.gz` & `tmp/trustauthx-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustauthx-0.6.3.tar", last modified: Sat Mar 30 21:28:16 2024, max compression
+gzip compressed data, was "trustauthx-0.6.5.tar", last modified: Wed Apr  3 17:04:43 2024, max compression
```

## Comparing `trustauthx-0.6.3.tar` & `trustauthx-0.6.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:28:16.546208 trustauthx-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-30 21:28:07.000000 trustauthx-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-03-30 21:28:16.546208 trustauthx-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-03-30 21:28:07.000000 trustauthx-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 21:28:16.546208 trustauthx-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-03-30 21:28:07.000000 trustauthx-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:28:16.542208 trustauthx-0.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-30 21:28:07.000000 trustauthx-0.6.3/test/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:28:16.546208 trustauthx-0.6.3/trustauthx/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-30 21:28:07.000000 trustauthx-0.6.3/trustauthx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29311 2024-03-30 21:28:07.000000 trustauthx-0.6.3/trustauthx/authlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-03-30 21:28:07.000000 trustauthx-0.6.3/trustauthx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-30 21:28:07.000000 trustauthx-0.6.3/trustauthx/llmai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-03-30 21:28:07.000000 trustauthx-0.6.3/trustauthx/scheme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 21:28:16.546208 trustauthx-0.6.3/trustauthx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-30 21:28:16.000000 trustauthx-0.6.3/trustauthx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.182959 trustauthx-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 17:04:34.000000 trustauthx-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:04:43.182959 trustauthx-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9100 2024-04-03 17:04:34.000000 trustauthx-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:04:43.182959 trustauthx-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 17:04:34.000000 trustauthx-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.178959 trustauthx-0.6.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-03 17:04:34.000000 trustauthx-0.6.5/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.178959 trustauthx-0.6.5/trustauthx/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32857 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/authlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/llmai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-04-03 17:04:34.000000 trustauthx-0.6.5/trustauthx/scheme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:04:43.182959 trustauthx-0.6.5/trustauthx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 17:04:43.000000 trustauthx-0.6.5/trustauthx.egg-info/top_level.txt
```

### Comparing `trustauthx-0.6.3/LICENSE` & `trustauthx-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.3/PKG-INFO` & `trustauthx-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.3
+Version: 0.6.5
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `trustauthx-0.6.3/README.md` & `trustauthx-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.3/setup.py` & `trustauthx-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='trustauthx',
-    version='0.6.3',
+    version='0.6.5',
     description='Official connector SDK for TrustAuthx',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This is important!
     author='moonlightnexus',
     author_email='nexus@trustauthx.com',
     url="https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git",
     license="MIT",
```

### Comparing `trustauthx-0.6.3/trustauthx/authlite.py` & `trustauthx-0.6.5/trustauthx/authlite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import requests
 from requests.exceptions import HTTPError
 from jose import JWTError, jwt
 from jose.constants import ALGORITHMS
 import json
 import sqlite3
 from .scheme import *
+from functools import wraps
+import threading
 
 class _EdgeDBRoleQuery:
     """
     A class for querying and managing roles and permissions.
 
     Attributes:
         in_memory (bool): Flag indicating whether to store the roles in-memory or in a SQLite database.
@@ -25,59 +27,63 @@
 
         validate(self, role_id, permission_key, permission_val):
             Validates a permission value for a given role ID and permission key.
 
         count_roles(self):
             Returns the number of roles stored.
     """
+    total_roles = 0
+    roles = None
+
     def __init__(self, roles, in_memory=True):
         """
         Initializes the _EdgeDBRoleQuery instance.
 
         Args:
             roles (List[Dict[str, Dict[str, str]]]): A list of dictionaries representing roles and their permissions.
             in_memory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True.
         """
         self.in_memory = in_memory
         if self.in_memory:
-            self.roles = {role_id: permissions for role in roles for role_id, permissions in role.items()}
+            self.__class__.roles = {role_id: permissions for role in roles for role_id, permissions in role.items()}
         else:
             self.conn = sqlite3.connect(':memory:')  # replace ':memory:' with your database path
             self.cursor = self.conn.cursor()
             self.cursor.execute("""
                 CREATE TABLE IF NOT EXISTS roles (
                     role_id TEXT PRIMARY KEY,
                     permissions TEXT
                 )
             """)
             for role in roles:
                 for role_id, permissions in role.items():
                     self.cursor.execute("INSERT INTO roles VALUES (?, ?)", (role_id, permissions))
             self.conn.commit()
+        self.count_roles()
 
     def query(self, role_id=None, permission_key=None):
         """
         Queries the roles and permissions based on the provided role ID and/or permission key.
 
         Args:
             role_id (str, optional): The role ID to query.
             permission_key (str, optional): The permission key to query.
 
         Returns:
             Union[Dict[str, Dict[str, str]], Dict[str, str], str, None]: The queried roles, permissions, or permission value, depending on the provided arguments.
         """
         if self.in_memory:
             if role_id and permission_key:
-                return self.roles.get(role_id, {}).get(permission_key, None)
+                return self.__class__.roles.get(role_id, {}).get(permission_key, None)
             elif role_id:
-                return self.roles.get(role_id, None)
+                return self.__class__.roles.get(role_id, None)
             elif permission_key:
-                return {role_id: permissions[permission_key] for role_id, permissions in self.roles.items() if permission_key in permissions}
+                return {role_id: permissions[permission_key] for role_id, permissions in self.__class__.roles.items() if permission_key in permissions}
             else:
-                return self.roles
+                return self.__class__.roles
         else:
             if role_id and permission_key:
                 self.cursor.execute("SELECT permissions FROM roles WHERE role_id = ?", (role_id,))
                 permissions = self.cursor.fetchone()
                 if permissions:
                     return permissions[0].get(permission_key, None)
             elif role_id:
@@ -99,33 +105,68 @@
             permission_key (str): The permission key to validate.
             permission_val (str): The expected permission value to validate.
 
         Returns:
             bool: True if the permission value matches the expected value, False otherwise.
         """
         if self.in_memory:
-            return self.roles.get(role_id, {}).get(permission_key, None) == permission_val
+            return self.__class__.roles.get(role_id, {}).get(permission_key, None) == permission_val
         else:
             self.cursor.execute("SELECT permissions FROM roles WHERE role_id = ?", (role_id,))
             permissions = self.cursor.fetchone()
             if permissions:
                 return permissions[0].get(permission_key, None) == permission_val
 
     def count_roles(self):
         """
         Returns the number of roles stored.
 
         Returns:
             int: The number of roles stored.
         """
         if self.in_memory:
-            return len(self.roles)
+            r = len(self.__class__.roles)
+            _EdgeDBRoleQuery.total_roles = r
+            return 
         else:
             self.cursor.execute("SELECT COUNT(*) FROM roles")
-            return self.cursor.fetchone()[0]
+            r = self.cursor.fetchone()[0]
+            _EdgeDBRoleQuery.total_roles = r
+            return 
+
+    @classmethod
+    def reinitialize_all(foreground=True):
+        if foreground:
+            for instance in AuthLiteClient.instances:
+                instance:AuthLiteClient = instance
+                instance._re_init_roles()
+        else:
+            def target():
+                for instance in AuthLiteClient.instances:
+                    instance:AuthLiteClient = instance
+                    instance._re_init_roles()
+            thread = threading.Thread(target=target)
+            thread.start()
+
+    @staticmethod
+    def _EDGE_Wrapper(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            # Call the function
+            response = func(*args, **kwargs)
+            # Check for "X-EDGE"
+            x_edge = response.headers.get("X-EDGE")
+            if int(x_edge) != _EdgeDBRoleQuery.total_roles:
+                _EdgeDBRoleQuery.reinitialize_all() # Add data
+            return response
+        return wrapper
+
+requests.get = _EdgeDBRoleQuery._EDGE_Wrapper(requests.get)
+requests.post = _EdgeDBRoleQuery._EDGE_Wrapper(requests.post)
+requests.delete = _EdgeDBRoleQuery._EDGE_Wrapper(requests.delete)
 
 class _Roles(_EdgeDBRoleQuery):
     """
     A class for managing roles and permissions in the EdgeDB system.
 
     Attributes:
         org_id (str): The organization ID associated with the roles.
@@ -147,123 +188,126 @@
 
         add_permission(self, rol_id, **Permission_):
             Adds a new permission to a role with the specified role ID.
 
         delete_permission(self, rol_id, **Permission_):
             Deletes a permission from a role with the specified role ID.
     """
+    instances = []
+
     def __init__(self, roles, org_id, api_key, signed_key, secret_key, API_BASE_URL, InMemory=True):
         """
         Initializes the _Roles instance.
 
         Args:
             roles (List[Dict[str, Dict[str, str]]]): A list of dictionaries representing roles and their permissions.
             org_id (str): The organization ID associated with the roles.
             api_key (str): The API key for authentication.
             signed_key (str): The signed key for authentication.
             secret_key (str): The secret key for JWT encoding/decoding.
             API_BASE_URL (str): The base URL for the API.
             InMemory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True.
         """
         self.org_id = org_id
-        self.api_key = api_key
+        self._api_key = api_key
         self._secret_key = secret_key
-        self.signed_key = signed_key
+        self._signed_key = signed_key
         self.API_BASE_URL = API_BASE_URL
+        self.__class__.instances.append(self)
         super().__init__(roles, in_memory=InMemory)
-        print(self.roles)
+        print(self.__class__.roles)
 
     def get_all_roles(self) -> GetAllRolesResponse:
         """
         Retrieves all roles and their permissions from the API.
 
         Returns:
-            List[Role]: A list of Role objects representing the roles and their permissions.
+            roles_list = List[Role]: A list of Role objects representing the roles and their permissions.roles
+            roles_json_list = List[dict]: A list of dict representing the roles and their permissions
         
-
         demo response ==> [
-  {
-    "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-    "rol_id": "rol_gCD_ebc6f7715bb14554",
-    "name": "string",
-    "permissions": [
-      {
-        "user": "administration"
-      }
-    ]
-  },
-  {
-    "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-    "rol_id": "rol_Ahy_f51d73ff656545e5",
-    "name": "string",
-    "permissions": []
-  },
-  {
-    "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-    "rol_id": "rol_rce_474ae9e59b3d49ce",
-    "name": "string",
-    "permissions": [
-      {
-        "user": "administration"
-      },
-      {
-        "viewer": "administration"
-      },
-      {
-        "maintainer": "administration"
-      }
-    ]
-  }
-]"""
+          {
+            "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+            "rol_id": "rol_gCD_ebc6f7715bb14554",
+            "name": "string",
+            "permissions": [
+              {
+                "user": "administration"
+              }
+            ]
+          },
+          {
+            "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+            "rol_id": "rol_Ahy_f51d73ff656545e5",
+            "name": "string",
+            "permissions": []
+          },
+          {
+            "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+            "rol_id": "rol_rce_474ae9e59b3d49ce",
+            "name": "string",
+            "permissions": [
+              {
+                "user": "administration"
+              },
+              {
+                "viewer": "administration"
+              },
+              {
+                "maintainer": "administration"
+              }
+            ]
+          }
+        ]"""
         url = f'{self.API_BASE_URL}/rbac/role'
         headers = {'accept': 'application/json'}
         params = {
             'org_id': f'{self.org_id}',
-            'api_key': f'{self.api_key}',
+            'api_key': f'{self._api_key}',
             'signed_key': f'{self._secret_key}'
         }
         response = requests.get(url, headers=headers, params=params)
         roles = [Role(**role_data) for role_data in response.json()]
-        return GetAllRolesResponse(roles=[role.to_dict() for role in roles])
+        return GetAllRolesResponse(roles_list=roles, roles_json_list=[role.to_dict() for role in roles])
 
-    def add_role(self, name, **Permission_) ->AddRoleResponse:
+    def add_role(self, name, **Permission_)->AddRoleResponse:
         """
         Adds a new role with the specified name and permissions.
 
         Args:
             name (str): The name of the new role.
             **Permission_: Keyword arguments representing the permissions to be added to the new role.
 
         Returns:
             AddRoleResponse: An AddRoleResponse object representing the newly created role.
             
         demo response ==> {
-  "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-  "rol_id": "rol_rce_474ae9e59b3d49ce",
-  "name": "string",
-  "permissions": [
-    {
-      "user": "administration"
-    },
-    {
-      "viewer": "administration"
-    },
-    {
-      "maintainer": "administration"
-    }
-  ]
-}"""
+          "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+          "rol_id": "rol_rce_474ae9e59b3d49ce",
+          "name": "string",
+          "permissions": [
+            {
+              "user": "administration"
+            },
+            {
+              "viewer": "administration"
+            },
+            {
+              "maintainer": "administration"
+            }
+          ]
+        }"""
         url = f'{self.API_BASE_URL}/rbac/role'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json'
         }
         params = {
             'org_id': f'{self.org_id}',
-            'api_key': f'{self.api_key}',
+            'api_key': f'{self._api_key}',
             'signed_key': f'{self._secret_key}'
         }
         permissions = [{k: v} for k, v in Permission_.items()]
         data = {
             "org_id": f'{self.org_id}',
             "name": name,
             "permissions": permissions
@@ -286,37 +330,37 @@
         Args:
             rol_id (str): The ID of the role to be deleted.
 
         Returns:
             DeleteRoleResponse: A DeleteRoleResponse object representing the deleted role.
         
         demo response ==> {
-  "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-  "rol_id": "rol_YHV_78ae9006bcaa4c77",
-  "name": "string",
-  "permissions": [
-    {
-      "user": "administration"
-    },
-    {
-      "viewer": "administration"
-    },
-    {
-      "maintainer": "administration"
-    }
-  ]
-}"""
+          "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+          "rol_id": "rol_YHV_78ae9006bcaa4c77",
+          "name": "string",
+          "permissions": [
+            {
+              "user": "administration"
+            },
+            {
+              "viewer": "administration"
+            },
+            {
+              "maintainer": "administration"
+            }
+          ]
+        }"""
         url = f'{self.API_BASE_URL}/rbac/role'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json'
         }
         params = {
             'org_id': f'{self.org_id}',
-            'api_key': f'{self.api_key}',
+            'api_key': f'{self._api_key}',
             'signed_key': f'{self._secret_key}'
         }
         data = {
             "org_id": f'{self.org_id}',
             "rol_id": rol_id
         }
         response = requests.delete(url, headers=headers, params=params, data=json.dumps(data))
@@ -325,105 +369,108 @@
         return DeleteRoleResponse(
             org_id=role_data.get("org_id"),
             rol_id=role_data.get("rol_id"),
             name=role_data.get("name"),
             permissions=permissions
         )
 
-    def add_permission(self, rol_id, **Permission_) -> AddPermissionResponse:
+    def add_permission(self, rol_id, foreground=False, **Permission_) -> AddPermissionResponse:
         """
         Adds a new permission to a role with the specified role ID.
 
         Args:
             rol_id (str): The ID of the role to which the permission should be added.
             **Permission_: Keyword arguments representing the permissions to be added.
 
         Returns:
             AddPermissionResponse: An AddPermissionResponse object representing the added permission.
               
         demo response ==> {
-  "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-  "rol_id": "rol_rce_474ae9e59b3d49ce",
-  "permissions": [
-    {
-      "any": "view" ##only return added content
-    }
-  ]
-}"""
+          "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+          "rol_id": "rol_rce_474ae9e59b3d49ce",
+          "permissions": [
+            {
+              "any": "view" ##only return added content
+            }
+          ]
+        }"""
         url = f'{self.API_BASE_URL}/rbac/permission'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json'
         }
         params = {
             'org_id': f'{self.org_id}',
-            'api_key': f'{self.api_key}',
+            'api_key': f'{self._api_key}',
             'signed_key': f'{self._secret_key}'
         }
         permissions = [{k: v} for k, v in Permission_.items()]
         data = {
             "org_id": f'{self.org_id}',
             "rol_id": rol_id,
             "permissions": permissions
         }
         response = requests.post(url, headers=headers, params=params, data=json.dumps(data))
         response_data = response.json()
         permissions = [{k: v} for k, v in permissions.items()]
+        self.reinitialize_all(foreground)
         return AddPermissionResponse(
             org_id=response_data.get("org_id"),
             rol_id=response_data.get("rol_id"),
             permissions=permissions
         )
 
-    def delete_permission(self, rol_id, **Permission_) -> DeletePermissionResponse:
+    def delete_permission(self, rol_id, foreground=False, **Permission_) -> DeletePermissionResponse:
         """
         Deletes a permission from a role with the specified role ID.
 
         Args:
             rol_id (str): The ID of the role from which the permission should be deleted.
             **Permission_: Keyword arguments representing the permissions to be deleted.
 
         Returns:
             DeletePermissionResponse: A DeletePermissionResponse object representing the role with the deleted permission.
         
         demo response ==> {
-  "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
-  "rol_id": "rol_rce_474ae9e59b3d49ce",
-  "permissions": [
-    {
-      "user": "administration"
-    },
-    {
-      "viewer": "administration"
-    },
-    {
-      "maintainer": "administration"
-    }
-  ]
-}""" #return full
+          "org_id": "4195502c85984d27ae1aceb677d99551543808625aeb11ee88069dc8f7663e88",
+          "rol_id": "rol_rce_474ae9e59b3d49ce",
+          "permissions": [
+            {
+              "user": "administration"
+            },
+            {
+              "viewer": "administration"
+            },
+            {
+              "maintainer": "administration"
+            }
+          ]
+        }""" #return full
         url = f'{self.API_BASE_URL}/rbac/permission'
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json'
         }
         params = {
             'org_id': f'{self.org_id}',
-            'api_key': f'{self.api_key}',
+            'api_key': f'{self._api_key}',
             'signed_key': f'{self._secret_key}'
         }
         permissions = [{k: v} for k, v in Permission_.items()]
         data = {
             "org_id": f'{self.org_id}',
             "rol_id": rol_id,
             "permissions": permissions
         }
         response = requests.delete(url, headers=headers, params=params, data=json.dumps(data))
+        self.reinitialize_all(foreground)
         return response.json()
     
 class AuthLiteClient():
+    instances = []
 
     """
     AuthLiteClient is a Python client for the TrustAuthX authentication service.
 
     Attributes:
         api_key (str): The API key used for authentication.
         secret_key (str): The secret key used for JWT encoding.
@@ -490,24 +537,26 @@
            org_id (str, optional): The organization ID for generating authentication URLs.
            API_BASE_URL (str, optional): The base URL for the API. Defaults to "https://api.trustauthx.com".
            in_memory (bool, optional): Flag indicating whether to store the roles in-memory or in a SQLite database. Defaults to True (ie. in-memory).
        
        """
         self.jwt_encode = lambda key, data: jwt.encode(data, key=key, algorithm= ALGORITHMS.HS256)
         self.jwt_decode = lambda key, data: jwt.decode(str(data), key=key, algorithms=ALGORITHMS.HS256)
-        self.secret_key = secret_key
-        self.api_key = api_key
+        self._secret_key = secret_key
+        self._api_key = api_key
         self.org_id = org_id
-        self.signed_key = self.jwt_encode(key=self.secret_key, data={"api_key":self.api_key})
+        self._signed_key = self.jwt_encode(key=self._secret_key, data={"api_key":self._api_key})
         self.API_BASE_URL = API_BASE_URL
+        self.in_memory = in_memory
         self.Roles: _Roles = _Roles(roles=self._set_edge_roles(), org_id=self.org_id, 
-                                    api_key=self.api_key, signed_key=self.signed_key, 
-                                    secret_key=self.secret_key, API_BASE_URL=self.API_BASE_URL,
+                                    api_key=self._api_key, signed_key=self._signed_key, 
+                                    secret_key=self._secret_key, API_BASE_URL=self.API_BASE_URL,
                                     InMemory=in_memory)
-
+        self.__class__.instances.append(self)
+        
     def generate_url(self) -> str:
         """
         Generates an authentication URL for the given organization.
 
         Returns:
             str: The generated authentication URL.
         
@@ -529,16 +578,16 @@
         Returns:
             str: The generated authentication URL.
         """
         # Generate an authentication url for the given org
         headers = {'accept': 'application/json'}
         params = {
             'AccessToken': access_token,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key,
+            'api_key': self._api_key,
+            'signed_key': self._signed_key,
             'url':url
                  }
         url = f"{self.API_BASE_URL}/api/user/me/settings/"
         req = requests.Request('GET', url, params=params, headers=headers).prepare()
         return req.url
 
     def re_auth(self, code):
@@ -553,21 +602,21 @@
 
         Raises:
             HTTPError: If the request fails with an HTTP error status code.
         """
         url = f"{self.API_BASE_URL}/api/user/me/widget/re-auth/token"
         params = {
             "code": code,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key
+            'api_key': self._api_key,
+            'signed_key': self._signed_key
         }
         headers = {"accept": "application/json"}
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self.secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key,response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
             return rtn
         else:raise HTTPError(
             'Request failed with status code : {} \n this code contains a msg : {}'.format(
@@ -589,20 +638,20 @@
             HTTPError: If the request fails with an HTTP error status code.
         """
         # Validate the given authentication token
         url = f'{self.API_BASE_URL}/api/user/me/auth/data'
         headers = {'accept': 'application/json'}
         params = {
             'UserToken': token,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key
+            'api_key': self._api_key,
+            'signed_key': self._signed_key
                  }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self.secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key,response.json())
             sub = json.loads(rtn["sub"])
             rtn.pop("sub")
             rtn["email"] = sub["email"]
             rtn["uid"] = sub["uid"]
             return rtn
         else:raise HTTPError(
             'Request failed with status code : {} \n this code contains a msg : {}'.format(
@@ -625,20 +674,20 @@
         """
         # Validate the given authentication token
         """returns a dict containing 'access_token', 'refresh_token', 'img', 'sub'"""
         url = f'{self.API_BASE_URL}/api/user/me/data'
         headers = {'accept': 'application/json'}
         params = {
             'AccessToken': AccessToken,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key
+            'api_key': self._api_key,
+            'signed_key': self._signed_key
                  }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:
-            rtn = self.jwt_decode(self.secret_key,response.json())
+            rtn = self.jwt_decode(self._secret_key,response.json())
             return rtn
         else:raise HTTPError(
             'Request failed with status code : {} \n this code contains a msg : {}'.format(
                                                                             response.status_code, 
                                                                             response.text)
                             )
 
@@ -656,16 +705,16 @@
             HTTPError: If the request fails with an HTTP error status code.
         """
         # Store the given authentication token
         url = f'{self.API_BASE_URL}/api/user/me/access/token/'
         headers = {'accept': 'application/json'}
         params = {
             'RefreshToken': refresh_token,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key
+            'api_key': self._api_key,
+            'signed_key': self._signed_key
                  }
         response = requests.get(url, headers=headers, params=params)
         if response.status_code == 200:return response.json()
         else:raise HTTPError(
             'Request failed with status code : {} \n this code contains a msg : {}'.format(
                                                                             response.status_code, 
                                                                             response.text)
@@ -682,16 +731,16 @@
             bool: True if the access token is valid, False otherwise.
         """
         # Store the given authentication token
         url = f'{self.API_BASE_URL}/api/user/me/auth/validate/token'
         headers = {'accept': 'application/json'}
         params = {
             'AccessToken': access_token,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key
+            'api_key': self._api_key,
+            'signed_key': self._signed_key
                  }
         response = requests.get(url, headers=headers, params=params)
         return response.status_code == 200
 
     def revoke_token(self,AccessToken:str=None, RefreshToken:str = None, revoke_all_tokens:bool = False) -> bool:
         """
         Revokes an access token or refresh token.
@@ -711,16 +760,16 @@
         url = f'{self.API_BASE_URL}/api/user/me/token/'
         headers = {'accept': 'application/json'}
         if not AccessToken and not RefreshToken:raise AttributeError("must provide either AccessToken or RefreshToken")
         tt=True if AccessToken else False
         t = AccessToken if AccessToken else RefreshToken
         params = {
             'Token': t,
-            'api_key': self.api_key,
-            'signed_key': self.signed_key,
+            'api_key': self._api_key,
+            'signed_key': self._signed_key,
             'AccessToken': tt,
             'SpecificTokenOnly':not revoke_all_tokens,
                 }
         response = requests.delete(url, headers=headers, params=params)
         if response.status_code == 200:return response.json()
         else:raise HTTPError(
             'Request failed with status code : {} \n this code contains a msg : {}'.format(response.status_code, response.text))
@@ -754,8 +803,26 @@
                 d.access = access_token
                 d.refresh = refresh_token
                 return d
         except:
             raise HTTPError('both tokens are invalid login again')
         
     def _set_edge_roles(self) -> list:
-        return []
+        self.Roles
+        url = f'{self.API_BASE_URL}/rbac/role'
+        headers = {'accept': 'application/json'}
+        params = {
+            'org_id': f'{self.org_id}',
+            'api_key': f'{self._api_key}',
+            'signed_key': f'{self._secret_key}'
+        }
+        response = requests.get(url, headers=headers, params=params)
+        roles = [Role(**role_data) for role_data in response.json()]
+        roles = GetAllRolesResponse(roles_list=roles, roles_json_list=[role.to_dict() for role in roles])
+        return roles.roles_json_list
+
+    def _re_init_roles(self) -> _Roles:
+        self.Roles: _Roles = _Roles(roles=self._set_edge_roles(), org_id=self.org_id, 
+                                    api_key=self._api_key, signed_key=self._signed_key, 
+                                    secret_key=self._secret_key, API_BASE_URL=self.API_BASE_URL,
+                                    InMemory=self.in_memory)
+        return self.Roles
```

### Comparing `trustauthx-0.6.3/trustauthx/cli.py` & `trustauthx-0.6.5/trustauthx/cli.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.3/trustauthx/llmai.py` & `trustauthx-0.6.5/trustauthx/llmai.py`

 * *Files identical despite different names*

### Comparing `trustauthx-0.6.3/trustauthx/scheme.py` & `trustauthx-0.6.5/trustauthx/scheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,16 @@
 @dataclass
 class Permission:
     name: str
     value: str
 
 @dataclass
 class GetAllRolesResponse:
-    roles: List[Dict[str, Union[str, List[Dict[str, str]]]]]
+    roles_list: List[Role]
+    roles_json_list: List[Dict[str, Union[str, List[Dict[str, str]]]]]
 
 @dataclass
 class AddRoleResponse:
     org_id: str
     rol_id: str
     name: str
     permissions: List[Permission]
```

### Comparing `trustauthx-0.6.3/trustauthx.egg-info/PKG-INFO` & `trustauthx-0.6.5/trustauthx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trustauthx
-Version: 0.6.3
+Version: 0.6.5
 Summary: Official connector SDK for TrustAuthx
 Home-page: https://github.com/One-Click-Auth/TrustAuthx-Py-SDK.git
 Author: moonlightnexus
 Author-email: nexus@trustauthx.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

