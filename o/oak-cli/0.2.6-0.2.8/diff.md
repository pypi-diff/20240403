# Comparing `tmp/oak_cli-0.2.6.tar.gz` & `tmp/oak_cli-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oak_cli-0.2.6.tar", max compression
+gzip compressed data, was "oak_cli-0.2.8.tar", max compression
```

## Comparing `oak_cli-0.2.6.tar` & `oak_cli-0.2.8.tar`

### file list

```diff
@@ -1,36 +1,47 @@
--rw-r--r--   0        0        0     2239 2024-03-27 11:39:20.275800 oak_cli-0.2.6/README.md
--rw-r--r--   0        0        0        0 2024-03-21 13:38:45.352806 oak_cli-0.2.6/oak_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 13:41:39.776809 oak_cli-0.2.6/oak_cli/args_parser/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 14:20:05.712854 oak_cli-0.2.6/oak_cli/args_parser/apps/__init__.py
--rw-r--r--   0        0        0     1320 2024-03-21 17:47:26.941095 oak_cli-0.2.6/oak_cli/args_parser/apps/create.py
--rw-r--r--   0        0        0     1228 2024-03-21 16:09:27.800981 oak_cli-0.2.6/oak_cli/args_parser/apps/delete.py
--rw-r--r--   0        0        0     1111 2024-03-21 15:46:57.868955 oak_cli-0.2.6/oak_cli/args_parser/apps/main.py
--rw-r--r--   0        0        0      623 2024-03-21 14:43:40.544881 oak_cli-0.2.6/oak_cli/args_parser/apps/status.py
--rw-r--r--   0        0        0      662 2024-03-27 09:12:43.559629 oak_cli-0.2.6/oak_cli/args_parser/main.py
--rw-r--r--   0        0        0        0 2024-03-21 16:14:51.264987 oak_cli-0.2.6/oak_cli/args_parser/services/__init__.py
--rw-r--r--   0        0        0     1799 2024-03-21 17:28:32.097073 oak_cli-0.2.6/oak_cli/args_parser/services/deployment.py
--rw-r--r--   0        0        0     1029 2024-03-21 17:29:37.329074 oak_cli-0.2.6/oak_cli/args_parser/services/main.py
--rw-r--r--   0        0        0     1444 2024-03-21 16:51:48.601030 oak_cli-0.2.6/oak_cli/args_parser/services/status.py
--rw-r--r--   0        0        0        0 2024-03-21 14:25:32.000860 oak_cli-0.2.6/oak_cli/commands/apps/__init__.py
--rw-r--r--   0        0        0     1747 2024-03-21 17:44:48.169092 oak_cli-0.2.6/oak_cli/commands/apps/main.py
--rw-r--r--   0        0        0      808 2024-03-21 16:55:58.093035 oak_cli-0.2.6/oak_cli/commands/apps/status.py
--rw-r--r--   0        0        0        0 2024-03-21 16:17:56.384991 oak_cli-0.2.6/oak_cli/commands/services/__init__.py
--rw-r--r--   0        0        0     1187 2024-03-21 17:33:50.841079 oak_cli-0.2.6/oak_cli/commands/services/deployment.py
--rw-r--r--   0        0        0      908 2024-03-21 16:49:42.037028 oak_cli-0.2.6/oak_cli/commands/services/get.py
--rw-r--r--   0        0        0     2613 2024-03-21 16:55:11.661034 oak_cli-0.2.6/oak_cli/commands/services/status.py
--rwxr-xr-x   0        0        0      283 2024-03-27 10:38:59.131729 oak_cli-0.2.6/oak_cli/main.py
--rw-r--r--   0        0        0        0 2024-03-21 14:26:39.340862 oak_cli-0.2.6/oak_cli/utils/SLAs/__init__.py
--rw-r--r--   0        0        0      329 2024-03-21 14:26:39.352862 oak_cli-0.2.6/oak_cli/utils/SLAs/blank_app_without_services.SLA.json
--rw-r--r--   0        0        0      310 2024-03-21 16:02:24.424973 oak_cli-0.2.6/oak_cli/utils/SLAs/common.py
--rw-r--r--   0        0        0     1949 2024-03-21 14:26:39.352862 oak_cli-0.2.6/oak_cli/utils/SLAs/default_app_with_services.SLA.json
--rw-r--r--   0        0        0        0 2024-03-21 14:26:39.368862 oak_cli-0.2.6/oak_cli/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-21 14:42:05.316880 oak_cli-0.2.6/oak_cli/utils/api/__init__.py
--rw-r--r--   0        0        0      758 2024-03-21 15:16:33.704919 oak_cli-0.2.6/oak_cli/utils/api/common.py
--rw-r--r--   0        0        0      781 2024-03-21 15:32:19.704938 oak_cli-0.2.6/oak_cli/utils/api/login.py
--rw-r--r--   0        0        0     3200 2024-03-21 16:05:23.144976 oak_cli-0.2.6/oak_cli/utils/api/main.py
--rw-r--r--   0        0        0      623 2024-03-27 11:13:10.743769 oak_cli-0.2.6/oak_cli/utils/argcomplete.py
--rw-r--r--   0        0        0      147 2024-03-21 15:59:25.536969 oak_cli-0.2.6/oak_cli/utils/common.py
--rw-r--r--   0        0        0     1355 2024-03-21 14:37:28.204874 oak_cli-0.2.6/oak_cli/utils/logging.py
--rw-r--r--   0        0        0      300 2024-03-21 17:43:49.745090 oak_cli-0.2.6/oak_cli/utils/types.py
--rw-r--r--   0        0        0      353 2024-03-27 11:39:20.275800 oak_cli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 oak_cli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2234 2024-03-27 12:16:04.091842 oak_cli-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/args_parser/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/args_parser/apps/__init__.py
+-rw-r--r--   0        0        0     1320 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/args_parser/apps/create.py
+-rw-r--r--   0        0        0     1212 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/apps/delete.py
+-rw-r--r--   0        0        0     1111 2024-03-27 12:14:42.263841 oak_cli-0.2.8/oak_cli/args_parser/apps/main.py
+-rw-r--r--   0        0        0      609 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/apps/status.py
+-rw-r--r--   0        0        0      897 2024-04-03 12:28:50.908125 oak_cli-0.2.8/oak_cli/args_parser/main.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:43:40.683785 oak_cli-0.2.8/oak_cli/args_parser/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:43:44.623785 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/__init__.py
+-rw-r--r--   0        0        0      574 2024-03-28 14:50:37.027793 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/create.py
+-rw-r--r--   0        0        0      715 2024-03-28 14:48:27.927790 oak_cli-0.2.8/oak_cli/args_parser/plugins/flops/main.py
+-rw-r--r--   0        0        0      725 2024-03-28 14:54:14.559797 oak_cli-0.2.8/oak_cli/args_parser/plugins/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/args_parser/services/__init__.py
+-rw-r--r--   0        0        0     1785 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/services/deployment.py
+-rw-r--r--   0        0        0     1029 2024-03-27 12:14:42.263841 oak_cli-0.2.8/oak_cli/args_parser/services/main.py
+-rw-r--r--   0        0        0     1431 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/args_parser/services/status.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/commands/apps/__init__.py
+-rw-r--r--   0        0        0     2708 2024-04-03 13:22:08.396187 oak_cli-0.2.8/oak_cli/commands/apps/main.py
+-rw-r--r--   0        0        0      290 2024-03-30 19:23:09.334671 oak_cli-0.2.8/oak_cli/commands/apps/status.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:49:56.455792 oak_cli-0.2.8/oak_cli/commands/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 14:49:58.079792 oak_cli-0.2.8/oak_cli/commands/plugins/flops/__init__.py
+-rw-r--r--   0        0        0      267 2024-03-30 11:20:16.086235 oak_cli-0.2.8/oak_cli/commands/plugins/flops/flops.SLA.json
+-rw-r--r--   0        0        0      885 2024-04-03 13:20:15.568185 oak_cli-0.2.8/oak_cli/commands/plugins/flops/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:28.647839 oak_cli-0.2.8/oak_cli/commands/services/__init__.py
+-rw-r--r--   0        0        0     1530 2024-04-03 13:18:56.984183 oak_cli-0.2.8/oak_cli/commands/services/deployment.py
+-rw-r--r--   0        0        0     1204 2024-04-03 13:16:47.388181 oak_cli-0.2.8/oak_cli/commands/services/get.py
+-rw-r--r--   0        0        0     1140 2024-03-30 19:39:10.414667 oak_cli-0.2.8/oak_cli/commands/services/status.py
+-rwxr-xr-x   0        0        0      901 2024-04-03 13:36:38.964204 oak_cli-0.2.8/oak_cli/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/SLAs/__init__.py
+-rw-r--r--   0        0        0      329 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/SLAs/blank_app_without_services.SLA.json
+-rw-r--r--   0        0        0      310 2024-04-03 12:27:20.648123 oak_cli-0.2.8/oak_cli/utils/SLAs/common.py
+-rw-r--r--   0        0        0     1949 2024-03-28 17:16:00.239961 oak_cli-0.2.8/oak_cli/utils/SLAs/default_app_with_services.SLA.json
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/api/__init__.py
+-rw-r--r--   0        0        0       87 2024-04-03 13:05:39.900168 oak_cli-0.2.8/oak_cli/utils/api/common.py
+-rw-r--r--   0        0        0      632 2024-04-03 12:38:29.088136 oak_cli-0.2.8/oak_cli/utils/api/custom_http.py
+-rw-r--r--   0        0        0     3034 2024-04-03 13:40:09.716208 oak_cli-0.2.8/oak_cli/utils/api/custom_requests.py
+-rw-r--r--   0        0        0     1050 2024-04-03 13:40:55.396209 oak_cli-0.2.8/oak_cli/utils/api/login.py
+-rw-r--r--   0        0        0      623 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/utils/argcomplete.py
+-rw-r--r--   0        0        0      147 2024-03-27 12:13:11.511839 oak_cli-0.2.8/oak_cli/utils/common.py
+-rw-r--r--   0        0        0      375 2024-04-03 12:39:42.116138 oak_cli-0.2.8/oak_cli/utils/exceptions.py
+-rw-r--r--   0        0        0     1354 2024-03-30 19:09:27.118675 oak_cli-0.2.8/oak_cli/utils/logging.py
+-rw-r--r--   0        0        0      264 2024-03-27 12:16:04.095842 oak_cli-0.2.8/oak_cli/utils/types.py
+-rw-r--r--   0        0        0      405 2024-04-03 13:43:04.716211 oak_cli-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 oak_cli-0.2.8/PKG-INFO
```

### Comparing `oak_cli-0.2.6/README.md` & `oak_cli-0.2.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # [Oakestra CLI](https://github.com/oakestra/oakestra-cli)
 
 **oakestra-cli** is a very basic command line tool for controlling your [Oakestra](https://github.com/oakestra/oakestra) setup. 
 
-It is intended to be a interface for the API as well as a development tool.
+It is intended to be an interface for the API as well as a development tool.
 
 The CLI supports command (tab) autocompletion.
 
 ## Usage
 The package can be called via `oak`.
 
-Currently it supports the creation, deletion, inspection, and (un)deployment of applications and services.
+Currently, it supports the creation, deletion, inspection, and (un)deployment of applications and services.
 
 E.g. To deploy a default application with two services:
 ```
 oak applications create default_app_with_services --deploy
 ```
 Note: The CLI supports short command aliases. The command above can be shortened like this:
 ```
@@ -63,15 +63,15 @@
    image: 'docker.io/library/nginx:latest'
    - networking -
    port: '6080:60/tcp'
    - instances -
    instances: '1'
 ```
 
-For a more detailed explanation have a try out the CLI and use the `-h` flag.
+For a more detailed explanation try out the CLI and use the `-h` flag.
 
 ## [Installation](https://pypi.org/project/oak-cli/)
 ```
 pip install oak-cli
 ```
 
 # For CLI Contributors/Developers
```

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/apps/create.py` & `oak_cli-0.2.8/oak_cli/args_parser/apps/create.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/apps/delete.py` & `oak_cli-0.2.8/oak_cli/args_parser/apps/delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _DELETION_HELP_TEXT = "deletes one or all applications" + _APP_ID_HELP_TEXT
 
 
 def prepare_applications_deletion_argparser(
     applications_subparsers: Subparsers,
 ) -> None:
-    def aux_delete_appliacations(args: Any):
+    def aux_delete_applications(args: Any):
         if args.all:
             delete_all_applications()
         else:
             delete_application(args.app_id)
 
     applications_deletion_parser = applications_subparsers.add_parser(
         "delete",
@@ -26,11 +26,9 @@
         help=_DELETION_HELP_TEXT,
         description=_DELETION_HELP_TEXT,
         formatter_class=argparse.RawTextHelpFormatter,
     )
     applications_deletion_parser.add_argument(
         "-a", "--all", action="store_true", help="delete all applications"
     )
-    applications_deletion_parser.add_argument(
-        "app_id", nargs="?", type=str, help=_APP_ID_HELP_TEXT
-    )
-    applications_deletion_parser.set_defaults(func=aux_delete_appliacations)
+    applications_deletion_parser.add_argument("app_id", nargs="?", type=str, help=_APP_ID_HELP_TEXT)
+    applications_deletion_parser.set_defaults(func=aux_delete_applications)
```

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/apps/main.py` & `oak_cli-0.2.8/oak_cli/args_parser/apps/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/apps/status.py` & `oak_cli-0.2.8/oak_cli/args_parser/apps/status.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,10 +9,8 @@
     applications_status_parser = applications_subparsers.add_parser(
         "status",
         aliases=["s"],
         help=HELP_TEXT,
         description=HELP_TEXT,
         formatter_class=argparse.RawTextHelpFormatter,
     )
-    applications_status_parser.set_defaults(
-        func=lambda _: display_current_applications()
-    )
+    applications_status_parser.set_defaults(func=lambda _: display_current_applications())
```

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/services/deployment.py` & `oak_cli-0.2.8/oak_cli/args_parser/services/deployment.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         "deploy",
         aliases=["d"],
         help=HELP_TEXT,
         description=HELP_TEXT,
         formatter_class=argparse.RawTextHelpFormatter,
     )
     services_deployment_parser.add_argument("service_id", type=str)
-    services_deployment_parser.set_defaults(
-        func=lambda args: deploy_new_instance(args.service_id)
-    )
+    services_deployment_parser.set_defaults(func=lambda args: deploy_new_instance(args.service_id))
 
 
 def prepare_services_undeployment_argparser(services_subparsers: Subparsers) -> None:
     def _aux_undeploy(args: Any) -> None:
         if args.all:
             undeploy_all_instances_of_service(args.service_id)
         elif args.instancenumber:
```

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/services/main.py` & `oak_cli-0.2.8/oak_cli/args_parser/services/main.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.6/oak_cli/args_parser/services/status.py` & `oak_cli-0.2.8/oak_cli/args_parser/services/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import argparse
 from typing import Any
 
 from oak_cli.commands.services.get import get_single_service
-from oak_cli.commands.services.status import (
-    display_all_current_services,
-    display_single_service,
-)
+from oak_cli.commands.services.status import display_all_current_services, display_single_service
 from oak_cli.utils.types import Subparsers
 
 
 def _aux_display_current_services(args: Any) -> None:
     if not args.serviceid:
         display_all_current_services(verbose=args.verbose, app_id=args.appid)
     elif args.serviceid:
```

### Comparing `oak_cli-0.2.6/oak_cli/commands/services/deployment.py` & `oak_cli-0.2.8/oak_cli/commands/services/deployment.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,39 @@
+import oak_cli.utils.api.custom_requests as custom_requests
 from oak_cli.commands.services.get import get_single_service
-from oak_cli.utils.api.common import SYSTEM_MANAGER_URL, HttpMethod
-from oak_cli.utils.api.main import handle_request
+from oak_cli.utils.api.common import SYSTEM_MANAGER_URL
+from oak_cli.utils.api.custom_http import HttpMethod
 from oak_cli.utils.types import Id, ServiceId
 
 
 def deploy_new_instance(service_id: ServiceId) -> None:
-    handle_request(
-        base_url=SYSTEM_MANAGER_URL,
-        http_method=HttpMethod.POST,
-        api_endpoint=f"/api/service/{service_id}/instance",
-        what_should_happen=f"Deploy a new instance for the service '{service_id}'",
-        show_msg_on_success=True,
-    )
+    custom_requests.CustomRequest(
+        custom_requests.RequestCore(
+            http_method=HttpMethod.POST,
+            base_url=SYSTEM_MANAGER_URL,
+            api_endpoint=f"/api/service/{service_id}/instance",
+        ),
+        custom_requests.RequestAuxiliaries(
+            what_should_happen=f"Deploy a new instance for the service '{service_id}'",
+            show_msg_on_success=True,
+        ),
+    ).execute()
 
 
 def undeploy_instance(service_id: ServiceId, instance_id: Id = None) -> None:
-    handle_request(
-        base_url=SYSTEM_MANAGER_URL,
-        http_method=HttpMethod.DELETE,
-        api_endpoint=f"/api/service/{service_id}/instance/{instance_id or 0}",
-        what_should_happen=f"Undeploy instance '{instance_id or 0}' for the service '{service_id}'",
-        show_msg_on_success=True,
-    )
+    custom_requests.CustomRequest(
+        custom_requests.RequestCore(
+            http_method=HttpMethod.DELETE,
+            base_url=SYSTEM_MANAGER_URL,
+            api_endpoint=f"/api/service/{service_id}/instance/{instance_id or 0}",
+        ),
+        custom_requests.RequestAuxiliaries(
+            what_should_happen=f"Undeploy instance '{instance_id or 0}' for service '{service_id}'",
+            show_msg_on_success=True,
+        ),
+    ).execute()
 
 
 def undeploy_all_instances_of_service(service_id: ServiceId) -> None:
     service = get_single_service(service_id)
     for instance in service["instance_list"]:
         undeploy_instance(service_id, instance["instance_number"])
```

### Comparing `oak_cli-0.2.6/oak_cli/utils/SLAs/default_app_with_services.SLA.json` & `oak_cli-0.2.8/oak_cli/utils/SLAs/default_app_with_services.SLA.json`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.6/oak_cli/utils/api/common.py` & `oak_cli-0.2.8/oak_cli/utils/api/custom_http.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-import os
-
 import requests
 
 from oak_cli.utils.types import CustomEnum
 
-GITHUB_PREFIX = "https://github.com/"
-SYSTEM_MANAGER_URL = f"http://{os.environ.get('SYSTEM_MANAGER_URL')}:10000"
-
 
 class HttpMethod(CustomEnum):
     GET = "get"
     POST = "post"
     PUT = "put"
     PATCH = "patch"
     DELETE = "delete"
```

### Comparing `oak_cli-0.2.6/oak_cli/utils/api/login.py` & `oak_cli-0.2.8/oak_cli/utils/api/login.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,36 @@
-from http import HTTPStatus
-
-import oak_cli.utils.api as oak_api
+import oak_cli.utils.api.custom_requests as custom_requests
+from oak_cli.utils.api.common import SYSTEM_MANAGER_URL
+from oak_cli.utils.api.custom_http import HttpMethod
+from oak_cli.utils.exceptions import LoginException
 
 _login_token = ""
 
 
 class LoginFailed(Exception):
     pass
 
 
 def _login_and_set_token() -> str:
-    data = {"username": "Admin", "password": "Admin"}
-    headers = {"accept": "application/json", "Content-Type": "application/json"}
-
-    json_data = oak_api.main.handle_request(
-        base_url=oak_api.common.SYSTEM_MANAGER_URL,
-        http_method=oak_api.common.HttpMethod.POST,
-        api_endpoint="/api/auth/login",
-        headers=headers,
-        data=data,
-        what_should_happen="Login",
-    )
+    response = custom_requests.CustomRequest(
+        custom_requests.RequestCore(
+            http_method=HttpMethod.POST,
+            base_url=SYSTEM_MANAGER_URL,
+            api_endpoint="/api/auth/login",
+            data={"username": "Admin", "password": "Admin"},
+            custom_headers={"accept": "application/json", "Content-Type": "application/json"},
+        ),
+        custom_requests.RequestAuxiliaries(
+            what_should_happen="Login",
+            exception=LoginException,
+        ),
+    ).execute()
 
     global _login_token
-    _login_token = json_data["token"]
+    _login_token = response["token"]
     return _login_token
 
 
 def get_login_token() -> str:
     if _login_token == "":
         return _login_and_set_token()
     return _login_token
```

### Comparing `oak_cli-0.2.6/oak_cli/utils/argcomplete.py` & `oak_cli-0.2.8/oak_cli/utils/argcomplete.py`

 * *Files identical despite different names*

### Comparing `oak_cli-0.2.6/oak_cli/utils/logging.py` & `oak_cli-0.2.8/oak_cli/utils/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
 _LOGGER_NAME = "logger"
-
 _FORMAT = "%(message)s"
 
 logger = logging.getLogger(_LOGGER_NAME)
 logger.setLevel(logging.DEBUG)
 
 _formatter = CustomFormatter(_FORMAT)
```

### Comparing `oak_cli-0.2.6/PKG-INFO` & `oak_cli-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: oak_cli
-Version: 0.2.6
+Version: 0.2.8
 Summary: 
 Author: Alexander Malyuk
 Author-email: malyuk.alexander1999@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: argcomplete (>=3.2.3,<4.0.0)
+Requires-Dist: icecream (>=2.1.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # [Oakestra CLI](https://github.com/oakestra/oakestra-cli)
 
 **oakestra-cli** is a very basic command line tool for controlling your [Oakestra](https://github.com/oakestra/oakestra) setup. 
 
-It is intended to be a interface for the API as well as a development tool.
+It is intended to be an interface for the API as well as a development tool.
 
 The CLI supports command (tab) autocompletion.
 
 ## Usage
 The package can be called via `oak`.
 
-Currently it supports the creation, deletion, inspection, and (un)deployment of applications and services.
+Currently, it supports the creation, deletion, inspection, and (un)deployment of applications and services.
 
 E.g. To deploy a default application with two services:
 ```
 oak applications create default_app_with_services --deploy
 ```
 Note: The CLI supports short command aliases. The command above can be shortened like this:
 ```
@@ -77,15 +78,15 @@
    image: 'docker.io/library/nginx:latest'
    - networking -
    port: '6080:60/tcp'
    - instances -
    instances: '1'
 ```
 
-For a more detailed explanation have a try out the CLI and use the `-h` flag.
+For a more detailed explanation try out the CLI and use the `-h` flag.
 
 ## [Installation](https://pypi.org/project/oak-cli/)
 ```
 pip install oak-cli
 ```
 
 # For CLI Contributors/Developers
```

