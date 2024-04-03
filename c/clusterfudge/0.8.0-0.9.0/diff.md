# Comparing `tmp/clusterfudge-0.8.0.tar.gz` & `tmp/clusterfudge-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clusterfudge-0.8.0.tar", last modified: Tue Mar  5 17:54:50 2024, max compression
+gzip compressed data, was "clusterfudge-0.9.0.tar", last modified: Tue Mar  5 18:13:25 2024, max compression
```

## Comparing `clusterfudge-0.8.0.tar` & `clusterfudge-0.9.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.426837 clusterfudge-0.8.0/
--rw-r--r--   0 george     (501) staff       (20)    11357 2024-02-20 15:57:51.000000 clusterfudge-0.8.0/LICENSE
--rw-r--r--   0 george     (501) staff       (20)      953 2024-03-05 17:54:50.426774 clusterfudge-0.8.0/PKG-INFO
--rw-r--r--   0 george     (501) staff       (20)      308 2024-02-27 18:36:08.000000 clusterfudge-0.8.0/README.md
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.405547 clusterfudge-0.8.0/clusterfudge/
--rw-r--r--   0 george     (501) staff       (20)      160 2024-03-05 17:08:17.000000 clusterfudge-0.8.0/clusterfudge/__init__.py
--rw-r--r--   0 george     (501) staff       (20)       83 2024-03-04 18:07:14.000000 clusterfudge-0.8.0/clusterfudge/__main__.py
--rw-r--r--   0 george     (501) staff       (20)     2166 2024-03-05 17:46:58.000000 clusterfudge-0.8.0/clusterfudge/cli.py
--rw-r--r--   0 george     (501) staff       (20)     3416 2024-03-05 16:29:05.000000 clusterfudge-0.8.0/clusterfudge/clusterfudge.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.426483 clusterfudge-0.8.0/clusterfudge.egg-info/
--rw-r--r--   0 george     (501) staff       (20)      953 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/PKG-INFO
--rw-r--r--   0 george     (501) staff       (20)     1053 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/SOURCES.txt
--rw-r--r--   0 george     (501) staff       (20)        1 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/dependency_links.txt
--rw-r--r--   0 george     (501) staff       (20)       60 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/entry_points.txt
--rw-r--r--   0 george     (501) staff       (20)       84 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/requires.txt
--rw-r--r--   0 george     (501) staff       (20)       32 2024-03-05 17:54:50.000000 clusterfudge-0.8.0/clusterfudge.egg-info/top_level.txt
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.406514 clusterfudge-0.8.0/clusterfudge_proto/
--rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:49:31.000000 clusterfudge-0.8.0/clusterfudge_proto/__init__.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.406974 clusterfudge-0.8.0/clusterfudge_proto/exec/
--rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:16.000000 clusterfudge-0.8.0/clusterfudge_proto/exec/__init__.py
--rw-r--r--   0 george     (501) staff       (20)     6419 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2.py
--rw-r--r--   0 george     (501) staff       (20)     8137 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2.pyi
--rw-r--r--   0 george     (501) staff       (20)     8745 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2_grpc.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.407475 clusterfudge-0.8.0/clusterfudge_proto/launches/
--rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:49:59.000000 clusterfudge-0.8.0/clusterfudge_proto/launches/__init__.py
--rw-r--r--   0 george     (501) staff       (20)     7562 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2.py
--rw-r--r--   0 george     (501) staff       (20)    10113 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2.pyi
--rw-r--r--   0 george     (501) staff       (20)    12461 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2_grpc.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.420290 clusterfudge-0.8.0/clusterfudge_proto/logs/
--rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:18.000000 clusterfudge-0.8.0/clusterfudge_proto/logs/__init__.py
--rw-r--r--   0 george     (501) staff       (20)     2983 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2.py
--rw-r--r--   0 george     (501) staff       (20)     3262 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2.pyi
--rw-r--r--   0 george     (501) staff       (20)     4060 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2_grpc.py
-drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 17:54:50.425558 clusterfudge-0.8.0/clusterfudge_proto/resources/
--rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:20.000000 clusterfudge-0.8.0/clusterfudge_proto/resources/__init__.py
--rw-r--r--   0 george     (501) staff       (20)     1403 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/resources/resources_pb2.py
--rw-r--r--   0 george     (501) staff       (20)      843 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/resources/resources_pb2.pyi
--rw-r--r--   0 george     (501) staff       (20)      159 2024-03-04 17:32:32.000000 clusterfudge-0.8.0/clusterfudge_proto/resources/resources_pb2_grpc.py
--rw-r--r--   0 george     (501) staff       (20)       96 2024-03-05 15:08:19.000000 clusterfudge-0.8.0/pyproject.toml
--rw-r--r--   0 george     (501) staff       (20)      768 2024-03-05 17:54:50.427118 clusterfudge-0.8.0/setup.cfg
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.099992 clusterfudge-0.9.0/
+-rw-r--r--   0 george     (501) staff       (20)    11357 2024-02-20 15:57:51.000000 clusterfudge-0.9.0/LICENSE
+-rw-r--r--   0 george     (501) staff       (20)      953 2024-03-05 18:13:25.099921 clusterfudge-0.9.0/PKG-INFO
+-rw-r--r--   0 george     (501) staff       (20)      308 2024-02-27 18:36:08.000000 clusterfudge-0.9.0/README.md
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.095559 clusterfudge-0.9.0/clusterfudge/
+-rw-r--r--   0 george     (501) staff       (20)      160 2024-03-05 17:08:17.000000 clusterfudge-0.9.0/clusterfudge/__init__.py
+-rw-r--r--   0 george     (501) staff       (20)       83 2024-03-04 18:07:14.000000 clusterfudge-0.9.0/clusterfudge/__main__.py
+-rw-r--r--   0 george     (501) staff       (20)     2251 2024-03-05 18:06:47.000000 clusterfudge-0.9.0/clusterfudge/cli.py
+-rw-r--r--   0 george     (501) staff       (20)     3416 2024-03-05 18:05:18.000000 clusterfudge-0.9.0/clusterfudge/clusterfudge.py
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.099663 clusterfudge-0.9.0/clusterfudge.egg-info/
+-rw-r--r--   0 george     (501) staff       (20)      953 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/PKG-INFO
+-rw-r--r--   0 george     (501) staff       (20)     1053 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/SOURCES.txt
+-rw-r--r--   0 george     (501) staff       (20)        1 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/dependency_links.txt
+-rw-r--r--   0 george     (501) staff       (20)       60 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/entry_points.txt
+-rw-r--r--   0 george     (501) staff       (20)       84 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/requires.txt
+-rw-r--r--   0 george     (501) staff       (20)       32 2024-03-05 18:13:25.000000 clusterfudge-0.9.0/clusterfudge.egg-info/top_level.txt
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.096619 clusterfudge-0.9.0/clusterfudge_proto/
+-rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:49:31.000000 clusterfudge-0.9.0/clusterfudge_proto/__init__.py
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.097236 clusterfudge-0.9.0/clusterfudge_proto/exec/
+-rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:16.000000 clusterfudge-0.9.0/clusterfudge_proto/exec/__init__.py
+-rw-r--r--   0 george     (501) staff       (20)     6419 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2.py
+-rw-r--r--   0 george     (501) staff       (20)     8137 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2.pyi
+-rw-r--r--   0 george     (501) staff       (20)     8745 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2_grpc.py
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.098303 clusterfudge-0.9.0/clusterfudge_proto/launches/
+-rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:49:59.000000 clusterfudge-0.9.0/clusterfudge_proto/launches/__init__.py
+-rw-r--r--   0 george     (501) staff       (20)     7562 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2.py
+-rw-r--r--   0 george     (501) staff       (20)    10113 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2.pyi
+-rw-r--r--   0 george     (501) staff       (20)    12461 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2_grpc.py
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.098856 clusterfudge-0.9.0/clusterfudge_proto/logs/
+-rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:18.000000 clusterfudge-0.9.0/clusterfudge_proto/logs/__init__.py
+-rw-r--r--   0 george     (501) staff       (20)     2983 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2.py
+-rw-r--r--   0 george     (501) staff       (20)     3262 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2.pyi
+-rw-r--r--   0 george     (501) staff       (20)     4060 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2_grpc.py
+drwxr-xr-x   0 george     (501) staff       (20)        0 2024-03-05 18:13:25.099434 clusterfudge-0.9.0/clusterfudge_proto/resources/
+-rw-r--r--   0 george     (501) staff       (20)        0 2024-03-05 15:50:20.000000 clusterfudge-0.9.0/clusterfudge_proto/resources/__init__.py
+-rw-r--r--   0 george     (501) staff       (20)     1403 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/resources/resources_pb2.py
+-rw-r--r--   0 george     (501) staff       (20)      843 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/resources/resources_pb2.pyi
+-rw-r--r--   0 george     (501) staff       (20)      159 2024-03-04 17:32:32.000000 clusterfudge-0.9.0/clusterfudge_proto/resources/resources_pb2_grpc.py
+-rw-r--r--   0 george     (501) staff       (20)       96 2024-03-05 15:08:19.000000 clusterfudge-0.9.0/pyproject.toml
+-rw-r--r--   0 george     (501) staff       (20)      768 2024-03-05 18:13:25.100256 clusterfudge-0.9.0/setup.cfg
```

### Comparing `clusterfudge-0.8.0/LICENSE` & `clusterfudge-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/PKG-INFO` & `clusterfudge-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfudge
-Version: 0.8.0
+Version: 0.9.0
 Summary: Clusterfudge is a supercomputer scheduler
 Author: Clusterfudge
 Author-email: support@clusterfudge.com
 Project-URL: Homepage, https://clusterfudge.com
 Keywords: clusterfudge,client,infrastructure,hpc,supercomputer,scheduler
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clusterfudge-0.8.0/clusterfudge/cli.py` & `clusterfudge-0.9.0/clusterfudge/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         token = future.result()
 
     _save_token_to_file(token)
 
 
 def _save_token_to_file(token: str):
     token_data = {"token": token}
-    filepath = os.path.join(os.path.expanduser("~"), ".clusterfudge", "config.json")
+    config_dir = os.path.join(os.path.expanduser("~"), ".clusterfudge")
+    os.makedirs(config_dir, exist_ok=True)
+    filepath = os.path.join(config_dir, "config.json")
     with open(filepath, "w") as token_file:
         json.dump(token_data, token_file)
     typer.echo("Token saved to file successfully.")
 
 
 @app.command()
 def login(tenant_id: Optional[str] = None):
```

### Comparing `clusterfudge-0.8.0/clusterfudge/clusterfudge.py` & `clusterfudge-0.9.0/clusterfudge/clusterfudge.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge.egg-info/PKG-INFO` & `clusterfudge-0.9.0/clusterfudge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clusterfudge
-Version: 0.8.0
+Version: 0.9.0
 Summary: Clusterfudge is a supercomputer scheduler
 Author: Clusterfudge
 Author-email: support@clusterfudge.com
 Project-URL: Homepage, https://clusterfudge.com
 Keywords: clusterfudge,client,infrastructure,hpc,supercomputer,scheduler
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clusterfudge-0.8.0/clusterfudge.egg-info/SOURCES.txt` & `clusterfudge-0.9.0/clusterfudge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2.py` & `clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2.pyi` & `clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/exec/exec_pb2_grpc.py` & `clusterfudge-0.9.0/clusterfudge_proto/exec/exec_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2.py` & `clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2.pyi` & `clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/launches/launches_pb2_grpc.py` & `clusterfudge-0.9.0/clusterfudge_proto/launches/launches_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2.py` & `clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2.pyi` & `clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/logs/logs_pb2_grpc.py` & `clusterfudge-0.9.0/clusterfudge_proto/logs/logs_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/resources/resources_pb2.py` & `clusterfudge-0.9.0/clusterfudge_proto/resources/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/clusterfudge_proto/resources/resources_pb2.pyi` & `clusterfudge-0.9.0/clusterfudge_proto/resources/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `clusterfudge-0.8.0/setup.cfg` & `clusterfudge-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = clusterfudge
 author = Clusterfudge
-version = 0.8.0
+version = 0.9.0
 author_email = support@clusterfudge.com
 description = Clusterfudge is a supercomputer scheduler
 long_description = file: README.md
 long_description_content_type = text/markdown
 project_urls = 
 	Homepage = https://clusterfudge.com
 keywords = clusterfudge, client, infrastructure, hpc, supercomputer, scheduler
```

