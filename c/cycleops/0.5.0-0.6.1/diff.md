# Comparing `tmp/cycleops-0.5.0.tar.gz` & `tmp/cycleops-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cycleops-0.5.0.tar", max compression
+gzip compressed data, was "cycleops-0.6.1.tar", max compression
```

## Comparing `cycleops-0.5.0.tar` & `cycleops-0.6.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     1069 2024-01-15 10:09:12.801595 cycleops-0.5.0/LICENSE
--rw-r--r--   0        0        0     4663 2024-01-15 10:09:12.801595 cycleops-0.5.0/README.md
--rw-r--r--   0        0        0     1125 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/__main__.py
--rw-r--r--   0        0        0      414 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/auth.py
--rw-r--r--   0        0        0     6207 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/client.py
--rw-r--r--   0        0        0     1113 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/exceptions.py
--rw-r--r--   0        0        0    13019 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/services.py
--rw-r--r--   0        0        0     5988 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/setups.py
--rw-r--r--   0        0        0     3607 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/stacks.py
--rw-r--r--   0        0        0      869 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/units.py
--rw-r--r--   0        0        0      972 2024-01-15 10:09:12.801595 cycleops-0.5.0/cycleops/utils.py
--rw-r--r--   0        0        0      558 2024-01-15 10:09:12.801595 cycleops-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     5188 1970-01-01 00:00:00.000000 cycleops-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-03 06:13:49.912218 cycleops-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5466 2024-04-03 06:13:49.912218 cycleops-0.6.1/README.md
+-rw-r--r--   0        0        0     1512 2024-04-03 06:13:49.912218 cycleops-0.6.1/cycleops/__main__.py
+-rw-r--r--   0        0        0      414 2024-04-03 06:13:49.912218 cycleops-0.6.1/cycleops/auth.py
+-rw-r--r--   0        0        0     8708 2024-04-03 06:13:49.912218 cycleops-0.6.1/cycleops/client.py
+-rw-r--r--   0        0        0     1155 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/environments.py
+-rw-r--r--   0        0        0     1113 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/exceptions.py
+-rw-r--r--   0        0        0     3762 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/hostgroups.py
+-rw-r--r--   0        0        0     4349 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/hosts.py
+-rw-r--r--   0        0        0    13019 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/services.py
+-rw-r--r--   0        0        0     5988 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/setups.py
+-rw-r--r--   0        0        0     3607 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/stacks.py
+-rw-r--r--   0        0        0      869 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/units.py
+-rw-r--r--   0        0        0      972 2024-04-03 06:13:49.916218 cycleops-0.6.1/cycleops/utils.py
+-rw-r--r--   0        0        0      558 2024-04-03 06:13:49.916218 cycleops-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5991 1970-01-01 00:00:00.000000 cycleops-0.6.1/PKG-INFO
```

### Comparing `cycleops-0.5.0/LICENSE` & `cycleops-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/README.md` & `cycleops-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,14 +53,56 @@
 
 #### List of all of the available units
 
 ```
 cycleops units list
 ```
 
+### Environments
+
+#### List your environments
+
+```
+cycleops environments list
+```
+
+
+### Hosts
+
+#### List your hosts
+
+```
+cycleops hosts list
+```
+
+#### Retrieve a host
+
+```
+cycleops hosts retrieve <host_name>|<host_id>
+```
+
+#### Create a host
+
+```
+cycleops hosts create --name <host_name> --ip <host_ip> --environment-id <environment_id> --jump-host true|false --hostgroup-id <hostgroup_id> ... --hostgroup-id <hostgroup_id>
+```
+
+#### Update a host
+
+```
+cycleops hosts update <host_name>|<host_id> --name <host_name> --ip <host_ip> --environment-id <environment_id> --jump-host true|false --hostgroup-id <hostgroup_id> ... --hostgroup-id <hostgroup_id>
+```
+
+#### Delete a host
+
+```
+cycleops hosts delete <host_name>|<host_id>
+```
+
+
 ### Services
 
 #### List your services
 
 ```
 cycleops services list
 ```
@@ -164,17 +206,19 @@
 ```
 cycleops setups delete <setup_name>|<setup_id>
 ```
 
 #### Deploy a setup
 
 ```
-cycleops setups deploy <setup_name>|<setup_id>
+cycleops setups deploy <setup_name>|<setup_id> --wait
 ```
 
+Using `--wait` you can wait for the deployment job to complete.
+
 ### GitHub Actions
 
 You can use Cycleops with your GitHub Actions to deploy a setup right from GitHub. For example this is how you could update the Docker image of a service and deploy a setup:
 
 ```yml
  deploy:
     runs-on: ubuntu-latest
```

### Comparing `cycleops-0.5.0/cycleops/__main__.py` & `cycleops-0.6.1/cycleops/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from typing import Optional
 
 import typer
 
 from .client import cycleops_client
+from .environments import app as environments_app
+from .hostgroups import app as hostgroups_app
+from .hosts import app as hosts_app
 from .services import app as services_app
 from .setups import app as setups_app
 from .stacks import app as stacks_app
 from .units import app as units_app
 
 cycleops = typer.Typer(pretty_exceptions_show_locals=False)
 
 cycleops.add_typer(services_app, name="services", help="Manage your services.")
 cycleops.add_typer(stacks_app, name="stacks", help="Manage your stacks.")
 cycleops.add_typer(setups_app, name="setups", help="Manage your setups.")
 cycleops.add_typer(units_app, name="units", help="List all of the available units.")
+cycleops.add_typer(
+    environments_app, name="environments", help="Manage your environments."
+)
+cycleops.add_typer(hosts_app, name="hosts", help="Manage your hosts.")
+cycleops.add_typer(hostgroups_app, name="hostgroups", help="Manage your hostgroups.")
 
 
 @cycleops.callback()
 def configure_cycleops_client(
     base_url: Optional[str] = typer.Option(
         None, help="Configure a base URL for the Cycleops API."
     ),
```

### Comparing `cycleops-0.5.0/cycleops/client.py` & `cycleops-0.6.1/cycleops/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -27,20 +27,22 @@
         self,
         method: str,
         endpoint: str,
         payload: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, Any]] = None,
     ) -> Optional[Dict[str, Any]]:
         url: str = f"{self.base_url}/{endpoint}"
+        headers: Dict[str] = {"Accept": "application/json; version=v2"}
         response: Response = requests.request(
             method,
             url,
             json=payload,
             auth=CycleopsAuthentication(self.api_key),
             params=params,
+            headers=headers,
         )
         return self._handle_response(response)
 
     def _handle_response(self, response: Response) -> Optional[Dict[str, Any]]:
         try:
             if response.status_code == 401:
                 error_message: str = extract_error_message(response)
@@ -188,8 +190,79 @@
 
         return self.client._request("PATCH", f"stacks/{stack_id}", payload)
 
     def delete(self, stack_id: int) -> Optional[Dict[str, Any]]:
         return self.client._request("DELETE", f"stacks/{stack_id}")
 
 
+class EnvironmentClient(SubClient):
+    """
+    Client for managing Cycleops environments.
+    """
+
+    def list(self) -> Optional[Dict[str, Any]]:
+        return self.client._request("GET", f"environments")
+
+
+class HostClient(SubClient):
+    """
+    Client for managing Cycleops hosts.
+    """
+
+    def list(self) -> Optional[Dict[str, Any]]:
+        return self.client._request("GET", f"hosts")
+
+    def retrieve(
+        self, host_id: Optional[int] = None, params: Optional[Dict[str, Any]] = None
+    ) -> Optional[Dict[str, Any]]:
+        if host_id:
+            return self.client._request("GET", f"hosts/{host_id}")
+
+        return self.client._request("GET", f"hosts", params=params)
+
+    def create(self, **kwargs: Any) -> Optional[Dict[str, Any]]:
+        payload: Dict[str, Any] = {k: v for (k, v) in kwargs.items() if v}
+
+        return self.client._request("POST", "hosts", payload)
+
+    def update(self, host_id: int, **kwargs: Any) -> Optional[Dict[str, Any]]:
+        payload: Dict[str, Any] = {k: v for (k, v) in kwargs.items() if v}
+
+        return self.client._request("PATCH", f"hosts/{host_id}", payload)
+
+    def delete(self, host_id: int) -> Optional[Dict[str, Any]]:
+        return self.client._request("DELETE", f"hosts/{host_id}")
+
+
+class HostgroupClient(SubClient):
+    """
+    Client for managing Cycleops hostgroups.
+    """
+
+    def list(self) -> Optional[Dict[str, Any]]:
+        return self.client._request("GET", f"hostgroups")
+
+    def retrieve(
+        self,
+        hostgroup_id: Optional[int] = None,
+        params: Optional[Dict[str, Any]] = None,
+    ) -> Optional[Dict[str, Any]]:
+        if hostgroup_id:
+            return self.client._request("GET", f"hostgroups/{hostgroup_id}")
+
+        return self.client._request("GET", f"hostgroups", params=params)
+
+    def create(self, **kwargs: Any) -> Optional[Dict[str, Any]]:
+        payload: Dict[str, Any] = {k: v for (k, v) in kwargs.items() if v}
+
+        return self.client._request("POST", "hostgroups", payload)
+
+    def update(self, hostgroup_id: int, **kwargs: Any) -> Optional[Dict[str, Any]]:
+        payload: Dict[str, Any] = {k: v for (k, v) in kwargs.items() if v}
+
+        return self.client._request("PATCH", f"hostgroups/{hostgroup_id}", payload)
+
+    def delete(self, hostgroup_id: int) -> Optional[Dict[str, Any]]:
+        return self.client._request("DELETE", f"hostgroups/{hostgroup_id}")
+
+
 cycleops_client: Client = Client()
```

### Comparing `cycleops-0.5.0/cycleops/exceptions.py` & `cycleops-0.6.1/cycleops/exceptions.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/cycleops/services.py` & `cycleops-0.6.1/cycleops/services.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/cycleops/setups.py` & `cycleops-0.6.1/cycleops/setups.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/cycleops/stacks.py` & `cycleops-0.6.1/cycleops/stacks.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/cycleops/units.py` & `cycleops-0.6.1/cycleops/units.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/cycleops/utils.py` & `cycleops-0.6.1/cycleops/utils.py`

 * *Files identical despite different names*

### Comparing `cycleops-0.5.0/pyproject.toml` & `cycleops-0.6.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cycleops"
-version = "0.5.0"
+version = "0.6.1"
 description = "The official command line interface for Cycleops"
 authors = ["George Margaritis <george@withlogic.co>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `cycleops-0.5.0/PKG-INFO` & `cycleops-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cycleops
-Version: 0.5.0
+Version: 0.6.1
 Summary: The official command line interface for Cycleops
 License: MIT
 Author: George Margaritis
 Author-email: george@withlogic.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -69,14 +69,56 @@
 
 #### List of all of the available units
 
 ```
 cycleops units list
 ```
 
+### Environments
+
+#### List your environments
+
+```
+cycleops environments list
+```
+
+
+### Hosts
+
+#### List your hosts
+
+```
+cycleops hosts list
+```
+
+#### Retrieve a host
+
+```
+cycleops hosts retrieve <host_name>|<host_id>
+```
+
+#### Create a host
+
+```
+cycleops hosts create --name <host_name> --ip <host_ip> --environment-id <environment_id> --jump-host true|false --hostgroup-id <hostgroup_id> ... --hostgroup-id <hostgroup_id>
+```
+
+#### Update a host
+
+```
+cycleops hosts update <host_name>|<host_id> --name <host_name> --ip <host_ip> --environment-id <environment_id> --jump-host true|false --hostgroup-id <hostgroup_id> ... --hostgroup-id <hostgroup_id>
+```
+
+#### Delete a host
+
+```
+cycleops hosts delete <host_name>|<host_id>
+```
+
+
 ### Services
 
 #### List your services
 
 ```
 cycleops services list
 ```
@@ -180,17 +222,19 @@
 ```
 cycleops setups delete <setup_name>|<setup_id>
 ```
 
 #### Deploy a setup
 
 ```
-cycleops setups deploy <setup_name>|<setup_id>
+cycleops setups deploy <setup_name>|<setup_id> --wait
 ```
 
+Using `--wait` you can wait for the deployment job to complete.
+
 ### GitHub Actions
 
 You can use Cycleops with your GitHub Actions to deploy a setup right from GitHub. For example this is how you could update the Docker image of a service and deploy a setup:
 
 ```yml
  deploy:
     runs-on: ubuntu-latest
```

