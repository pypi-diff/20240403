# Comparing `tmp/python-bridge-0.0.8.tar.gz` & `tmp/python-bridge-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.8.tar", last modified: Wed Apr  3 16:30:13 2024, max compression
+gzip compressed data, was "python-bridge-0.0.9.tar", last modified: Wed Apr  3 16:46:42 2024, max compression
```

## Comparing `python-bridge-0.0.8.tar` & `python-bridge-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.662610 python-bridge-0.0.8/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.8/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:30:13.662357 python-bridge-0.0.8/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.8/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.657979 python-bridge-0.0.8/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.8/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.658705 python-bridge-0.0.8/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.8/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.8/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.659525 python-bridge-0.0.8/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.8/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4342 2024-04-03 07:27:17.000000 python-bridge-0.0.8/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1086 2024-04-03 05:37:16.000000 python-bridge-0.0.8/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.8/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.660400 python-bridge-0.0.8/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.8/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.8/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1362 2024-04-03 16:23:57.000000 python-bridge-0.0.8/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.661015 python-bridge-0.0.8/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.8/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.8/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.8/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 16:29:43.000000 python-bridge-0.0.8/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.662058 python-bridge-0.0.8/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 16:30:13.662661 python-bridge-0.0.8/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.489123 python-bridge-0.0.9/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.9/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:46:42.488846 python-bridge-0.0.9/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.9/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.484133 python-bridge-0.0.9/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.9/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.484751 python-bridge-0.0.9/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.9/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.9/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.485555 python-bridge-0.0.9/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.9/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4415 2024-04-03 16:46:17.000000 python-bridge-0.0.9/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1086 2024-04-03 05:37:16.000000 python-bridge-0.0.9/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.9/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.486913 python-bridge-0.0.9/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.9/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.9/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1455 2024-04-03 16:45:46.000000 python-bridge-0.0.9/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.487600 python-bridge-0.0.9/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.9/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.9/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.9/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 16:46:33.000000 python-bridge-0.0.9/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:46:42.488591 python-bridge-0.0.9/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 16:46:42.000000 python-bridge-0.0.9/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 16:46:42.489183 python-bridge-0.0.9/setup.cfg
```

### Comparing `python-bridge-0.0.8/LICENSE` & `python-bridge-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/PKG-INFO` & `python-bridge-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.8/bridge/cli/bridge.py` & `python-bridge-0.0.9/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/bridge/cli/deploy/base.py` & `python-bridge-0.0.9/bridge/cli/deploy/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import requests
 from google.cloud import storage
 from rich.console import Console
 
 from bridge.console import log_error, log_task
 
 API_URL = "https://api.bridge-cli.com/api/v0.1/deploy"
+DEMO_URL = "demo.bridge-cli.com"
 
 
 class DeployHandler(ABC):
     def __init__(self, bucket_name, project_root=".", deploy_name=None):
         self.python_path = (
             sys.executable
         )  # TODO need to better interpret and utilize this
@@ -108,8 +109,8 @@
             url = self.upload(zip_path)
             project_name = (
                 self.project_root.name
             )  # TODO we should infer an asgi or wsgi entrypoint
             self.trigger(project_name=project_name, source_url=url)
             deployment_url = self.retrieve()
         console.print(f"[bold white]{self.deploy_name[:8]} [bold green]deployed!")
-        console.print(f"[blue]{deployment_url}")
+        console.print(f"[blue]https://{deployment_url if deployment_url else DEMO_URL}")
```

### Comparing `python-bridge-0.0.8/bridge/cli/deploy/django.py` & `python-bridge-0.0.9/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/bridge/console.py` & `python-bridge-0.0.9/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/bridge/framework/base.py` & `python-bridge-0.0.9/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/bridge/framework/django.py` & `python-bridge-0.0.9/bridge/framework/django.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import os.path
+import os
 
+from bridge.cli.deploy.base import DEMO_URL
 from bridge.console import log_warning
 from bridge.framework.base import FrameWorkHandler
 from bridge.service.postgres import PostgresEnvironment
 
 
 class DjangoHandler(FrameWorkHandler):
     def configure_postgres(self, environment: PostgresEnvironment) -> None:
@@ -19,15 +20,18 @@
                 "USER": environment.POSTGRES_USER,
                 "PASSWORD": environment.POSTGRES_PASSWORD,
                 "HOST": environment.POSTGRES_HOST,
                 "PORT": environment.POSTGRES_PORT,
             }
         }
         if os.environ.get("IS_BRIDGE_PLATFORM"):
-            self.framework_locals["ALLOWED_HOSTS"].append(os.environ["BRIDGE_HOST"])
+            self.framework_locals["ALLOWED_HOSTS"] += [
+                os.environ["BRIDGE_HOST"],
+                DEMO_URL,
+            ]
 
 
 def configure(settings_locals: dict, enable_postgres=True) -> None:
     project_name = os.path.basename(settings_locals["BASE_DIR"])
 
     handler = DjangoHandler(
         project_name=project_name,
```

### Comparing `python-bridge-0.0.8/bridge/service/docker.py` & `python-bridge-0.0.9/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/bridge/service/postgres.py` & `python-bridge-0.0.9/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.8/pyproject.toml` & `python-bridge-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.8/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.9/python_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.8/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.9/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

