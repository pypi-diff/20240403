# Comparing `tmp/python-bridge-0.0.4.tar.gz` & `tmp/python-bridge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.4.tar", last modified: Wed Apr  3 01:43:51 2024, max compression
+gzip compressed data, was "python-bridge-0.0.5.tar", last modified: Wed Apr  3 04:38:47 2024, max compression
```

## Comparing `python-bridge-0.0.4.tar` & `python-bridge-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.827288 python-bridge-0.0.4/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.4/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:43:51.827072 python-bridge-0.0.4/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.4/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.822456 python-bridge-0.0.4/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.4/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.822988 python-bridge-0.0.4/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.4/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.4/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.823883 python-bridge-0.0.4/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.4/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2225 2024-04-03 01:33:28.000000 python-bridge-0.0.4/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.4/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.4/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.824651 python-bridge-0.0.4/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.4/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.4/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1209 2024-04-03 01:29:01.000000 python-bridge-0.0.4/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.825457 python-bridge-0.0.4/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.4/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.4/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.4/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 01:34:22.000000 python-bridge-0.0.4/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.826809 python-bridge-0.0.4/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:43:51.827336 python-bridge-0.0.4/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.894753 python-bridge-0.0.5/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.5/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 04:38:47.894415 python-bridge-0.0.5/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.5/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.889594 python-bridge-0.0.5/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.5/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.890287 python-bridge-0.0.5/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.5/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.5/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.891142 python-bridge-0.0.5/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.5/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2225 2024-04-03 01:33:28.000000 python-bridge-0.0.5/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.5/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.5/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.891763 python-bridge-0.0.5/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.5/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.5/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1228 2024-04-03 01:58:36.000000 python-bridge-0.0.5/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.892464 python-bridge-0.0.5/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.5/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.5/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.5/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 04:38:23.000000 python-bridge-0.0.5/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 04:38:47.893788 python-bridge-0.0.5/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 04:38:47.000000 python-bridge-0.0.5/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 04:38:47.894997 python-bridge-0.0.5/setup.cfg
```

### Comparing `python-bridge-0.0.4/LICENSE` & `python-bridge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.4/PKG-INFO` & `python-bridge-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.4/bridge/cli/bridge.py` & `python-bridge-0.0.5/bridge/cli/bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,20 @@
 def main():
     # Create the top-level parser for the 'bridge-sdk' command
     parser = argparse.ArgumentParser(prog="bridge-sdk")
     subparsers = parser.add_subparsers(dest="command", help="sub-command help")
 
     # Parser for 'deploy' command
     deploy_parser = subparsers.add_parser("deploy", help="Deploy help")
-    deploy_subparsers = deploy_parser.add_subparsers(
-        dest="deploy_command", help="Deploy sub-command help"
-    )
+    deploy_parser.add_subparsers(dest="deploy_command", help="Deploy sub-command help")
 
     # # Sub-parser for 'deploy' without sub-commands but with optional args
     # deploy_parser.add_argument(
-    #     "optional_args", nargs="*", help="Optional arguments for deploy", required=False
+    #     "optional_args", nargs="*", help="Optional arguments for deploy",
+    #     required=False
     # )
     #
     # # Sub-parser for 'deploy list'
     # deploy_list_parser = deploy_subparsers.add_parser("list", help="List deployments")
     #
     # # Sub-parser for 'deploy rollback'
     # deploy_rollback_parser = deploy_subparsers.add_parser(
@@ -48,18 +47,18 @@
     # )
     #
     # env_list_parser = env_subparsers.add_parser(
     #     "list", help="List environment variables"
     # )
 
     # Parser for 'shell' command
-    shell_parser = subparsers.add_parser("shell", help="Open a shell")
+    subparsers.add_parser("shell", help="Open a shell")
 
     # Parser for 'logs' command
-    logs_parser = subparsers.add_parser("logs", help="Show logs")
+    subparsers.add_parser("logs", help="Show logs")
 
     # Parse the arguments
     args = parser.parse_args()
 
     if args.command == "deploy":
         if args.deploy_command is None:
             # assume django for now
```

### Comparing `python-bridge-0.0.4/bridge/cli/deploy/base.py` & `python-bridge-0.0.5/bridge/cli/deploy/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.4/bridge/cli/deploy/django.py` & `python-bridge-0.0.5/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.4/bridge/console.py` & `python-bridge-0.0.5/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.4/bridge/framework/base.py` & `python-bridge-0.0.5/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.4/bridge/framework/django.py` & `python-bridge-0.0.5/bridge/framework/django.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from bridge.service.postgres import PostgresEnvironment
 
 
 class DjangoHandler(FrameWorkHandler):
     def configure_postgres(self, environment: PostgresEnvironment) -> None:
         if "DATABASES" in self.framework_locals:
             log_warning(
-                "databases already configured; overwriting key. Make sure no other instances of postgres are running."
+                "databases already configured; overwriting key. "
+                "Make sure no other instances of postgres are running."
             )
         self.framework_locals["DATABASES"] = {
             "default": {
                 "ENGINE": "django.db.backends.postgresql",
                 "NAME": environment.POSTGRES_DB,
                 "USER": environment.POSTGRES_USER,
                 "PASSWORD": environment.POSTGRES_PASSWORD,
```

### Comparing `python-bridge-0.0.4/bridge/service/docker.py` & `python-bridge-0.0.5/bridge/service/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     return client
 
 
 class ContainerConfig(BaseModel):
     """
     Container configuration information.
 
-    All of the data needed to start a container. Matches the method signature of `docker.container.create()`
+    All of the data needed to start a container.
+    Matches the method signature of `docker.container.create()`
     """
 
     image: str
     name: str
     ports: dict = {}
     volumes: dict = {}
     restart_policy: dict = {"Name": "always"}
@@ -38,15 +39,16 @@
         self.client = client
         self.config = config
         # todo add self.container - should we start or fetch the container on startup?
 
     def start(self):
         console = Console()
         console.print(
-            f"[bold bright_green]Setting up service [white]{self.config.name}[/white]..."
+            f"[bold bright_green]Setting up service "
+            f"[white]{self.config.name}[/white]..."
         )
         self.pull_image()
         self.start_container()
         self.ensure_ready()
         console.print(
             f"[bold bright_green]Service [white]{self.config.name}[/white] started!"
         )
```

### Comparing `python-bridge-0.0.4/bridge/service/postgres.py` & `python-bridge-0.0.5/bridge/service/postgres.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,20 @@
     POSTGRES_PASSWORD: str = "postgres"
     POSTGRES_DB: str = "postgres"
     POSTGRES_HOST: str = "localhost"
     POSTGRES_PORT: str = "5432"
 
 
 def resolve_pg_data_path():
-    return os.path.abspath("./pgdata")
+    # TODO create a folder per project or separate db for each
+    current_file_dir = os.path.dirname(os.path.abspath(__file__))
+    dir_path = os.path.join(current_file_dir, "pgdata")
+    if not os.path.exists(dir_path):
+        os.makedirs(dir_path)
+    return dir_path
 
 
 class PostgresConfig(ContainerConfig):
     image: str = "postgres:12"
     name: str = "bridge_postgres"
     ports: dict = {"5432/tcp": 5432}
     volumes: dict = Field(
```

### Comparing `python-bridge-0.0.4/pyproject.toml` & `python-bridge-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.4/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.5/python_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.4
+Version: 0.0.5
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.4/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.5/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

