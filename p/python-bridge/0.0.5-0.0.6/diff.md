# Comparing `tmp/python-bridge-0.0.5.tar.gz` & `tmp/python-bridge-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.5.tar", last modified: Wed Apr  3 04:38:47 2024, max compression
+gzip compressed data, was "python-bridge-0.0.6.tar", last modified: Wed Apr  3 06:58:09 2024, max compression
```

## Comparing `python-bridge-0.0.5.tar` & `python-bridge-0.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.894753 python-bridge-0.0.5/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.5/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 04:38:47.894415 python-bridge-0.0.5/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.5/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.889594 python-bridge-0.0.5/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.5/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.890287 python-bridge-0.0.5/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.5/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.5/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.891142 python-bridge-0.0.5/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.5/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2225 2024-04-03 01:33:28.000000 python-bridge-0.0.5/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.5/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.5/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.891763 python-bridge-0.0.5/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.5/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.5/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1228 2024-04-03 01:58:36.000000 python-bridge-0.0.5/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.892464 python-bridge-0.0.5/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.5/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.5/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.5/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 04:38:23.000000 python-bridge-0.0.5/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.893788 python-bridge-0.0.5/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 04:38:47.894997 python-bridge-0.0.5/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.694694 python-bridge-0.0.6/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.6/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 06:58:09.694451 python-bridge-0.0.6/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.6/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.690360 python-bridge-0.0.6/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.6/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.690891 python-bridge-0.0.6/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.6/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.6/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.691693 python-bridge-0.0.6/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.6/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4141 2024-04-03 06:56:58.000000 python-bridge-0.0.6/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1086 2024-04-03 05:37:16.000000 python-bridge-0.0.6/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.6/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.692515 python-bridge-0.0.6/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.6/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.6/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1228 2024-04-03 01:58:36.000000 python-bridge-0.0.6/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.693144 python-bridge-0.0.6/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.6/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.6/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.6/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 06:57:49.000000 python-bridge-0.0.6/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 06:58:09.694205 python-bridge-0.0.6/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 06:58:09.000000 python-bridge-0.0.6/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 06:58:09.694738 python-bridge-0.0.6/setup.cfg
```

### Comparing `python-bridge-0.0.5/LICENSE` & `python-bridge-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/PKG-INFO` & `python-bridge-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.5/bridge/cli/bridge.py` & `python-bridge-0.0.6/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/bridge/cli/deploy/base.py` & `python-bridge-0.0.6/bridge/cli/deploy/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
+import os
 import sys
 import tempfile
 import uuid
 import zipfile
 from abc import ABC, abstractmethod
 from pathlib import Path
+from time import sleep
 
+import requests
 from google.cloud import storage
 from rich.console import Console
 
-from bridge.console import log_task
+from bridge.console import log_error, log_task
+
+API_URL = "https://api.bridge-cli.com/api/v0.1/deploy"
 
 
 class DeployHandler(ABC):
     def __init__(self, bucket_name, project_root=".", deploy_name=None):
         self.python_path = (
             sys.executable
         )  # TODO need to better interpret and utilize this
-        self.project_root = Path(project_root)
+        self.project_root = Path(os.path.abspath(project_root))
         self.bucket_name = bucket_name
         if not deploy_name:
             deploy_name = str(uuid.uuid4())
         self.deploy_name = deploy_name
 
     @abstractmethod
     def validate(self):
@@ -39,25 +44,69 @@
                 for file_path in self.project_root.rglob(
                     "*"
                 ):  # TODO add .gitignore support
                     if file_path.is_file():
                         zipf.write(file_path, file_path.relative_to(self.project_root))
         return zip_path
 
-    def upload(self, zip_path: Path):
+    def upload(self, zip_path: Path) -> str:
         with log_task(
             start_message="Uploading bundle...", end_message="Bundle uploaded"
         ):
             storage_client = storage.Client()
             bucket = storage_client.bucket(self.bucket_name)
             destination_blob_name = f"deploys/{self.deploy_name}.zip"
             blob = bucket.blob(destination_blob_name)
             blob.upload_from_filename(str(zip_path))
+            public_url = blob.public_url
+            return public_url
+
+    def trigger(self, project_name, source_url):
+        with log_task(
+            start_message="Triggering deploy...", end_message="Deploy triggered"
+        ):
+            data = {
+                "name": self.deploy_name[:8],
+                "project_name": project_name,
+                "source_url": source_url,
+            }
+            resp = requests.post(API_URL, json=data)
+            if resp.status_code != 200:
+                print(resp.status_code, resp.content)
+                log_error("Failed to trigger the deploy")
+                sys.exit(1)
+
+    def check_status(self):
+        with log_task(
+            start_message="Checking deploy status...", end_message="Status updated"
+        ):
+            status = "pending"
+            while status == "pending":
+                resp = requests.get(API_URL)
+                sleep(0.1)
+                if resp.status_code == 200:
+                    deployment_data = resp.json()
+                    for deployment in deployment_data["deployments"]:
+                        if deployment["name"] == self.deploy_name[:8]:
+                            status = deployment["status"]
+                            if status == "error":
+                                log_error(deployment["debug"])
+                            break
+                else:
+                    sleep(3)
 
     def deploy(self):
         console = Console()
-        console.print("Deploying...", style="bold green")
+        console.print(
+            f"Deploying [bold white]{self.project_root.name}"
+            f"[bold green] as [bold white]{self.deploy_name[:8]}[bold green]...",
+        )
         self.validate()
         with tempfile.TemporaryDirectory() as temp_dir:
             zip_path = self.bundle(temp_dir)
-            self.upload(zip_path)
+            url = self.upload(zip_path)
+            project_name = (
+                self.project_root.name
+            )  # TODO we should infer an asgi or wsgi entrypoint
+            self.trigger(project_name=project_name, source_url=url)
+            self.check_status()
         console.print(f"[bold white]{self.deploy_name[:8]} [bold green]deployed!")
```

### Comparing `python-bridge-0.0.5/bridge/cli/deploy/django.py` & `python-bridge-0.0.6/bridge/cli/deploy/django.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 class DjangoDeployer(DeployHandler):
     def __init__(self, bucket_name: str, project_root="."):
         super().__init__(bucket_name, project_root)
 
     def validate(self):
         with log_task(
-            start_message="Validating Django project integrity...",
-            end_message="Django project valid",
+            start_message="Validating project...",
+            end_message="Project is valid",
         ):
             manage_py_path = self.project_root / "manage.py"
             if not manage_py_path.exists():
                 log_error(f"No manage.py file found in {self.project_root}")
                 sys.exit(1)
 
             try:
```

### Comparing `python-bridge-0.0.5/bridge/console.py` & `python-bridge-0.0.6/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/bridge/framework/base.py` & `python-bridge-0.0.6/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/bridge/framework/django.py` & `python-bridge-0.0.6/bridge/framework/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/bridge/service/docker.py` & `python-bridge-0.0.6/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/bridge/service/postgres.py` & `python-bridge-0.0.6/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.5/pyproject.toml` & `python-bridge-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.5/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.6/python_bridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.5/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.6/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

