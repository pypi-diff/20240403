# Comparing `tmp/python-bridge-0.0.3.tar.gz` & `tmp/python-bridge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.3.tar", last modified: Wed Apr  3 01:14:51 2024, max compression
+gzip compressed data, was "python-bridge-0.0.4.tar", last modified: Wed Apr  3 01:43:51 2024, max compression
```

## Comparing `python-bridge-0.0.3.tar` & `python-bridge-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.281896 python-bridge-0.0.3/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.3/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:14:51.281658 python-bridge-0.0.3/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.3/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.276930 python-bridge-0.0.3/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.3/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.277287 python-bridge-0.0.3/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.3/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.3/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.277962 python-bridge-0.0.3/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.3/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2221 2024-04-02 22:47:43.000000 python-bridge-0.0.3/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.3/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      843 2024-04-02 22:55:44.000000 python-bridge-0.0.3/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.278982 python-bridge-0.0.3/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.3/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.3/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1157 2024-04-03 00:33:01.000000 python-bridge-0.0.3/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.280092 python-bridge-0.0.3/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.3/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.3/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.3/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 01:14:41.000000 python-bridge-0.0.3/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.281371 python-bridge-0.0.3/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:14:51.281955 python-bridge-0.0.3/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.827288 python-bridge-0.0.4/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.4/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:43:51.827072 python-bridge-0.0.4/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.4/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.822456 python-bridge-0.0.4/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.4/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.822988 python-bridge-0.0.4/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.4/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.4/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.823883 python-bridge-0.0.4/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.4/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2225 2024-04-03 01:33:28.000000 python-bridge-0.0.4/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.4/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.4/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.824651 python-bridge-0.0.4/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.4/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.4/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1209 2024-04-03 01:29:01.000000 python-bridge-0.0.4/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.825457 python-bridge-0.0.4/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.4/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.4/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.4/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 01:34:22.000000 python-bridge-0.0.4/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:43:51.826809 python-bridge-0.0.4/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:43:51.000000 python-bridge-0.0.4/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:43:51.827336 python-bridge-0.0.4/setup.cfg
```

### Comparing `python-bridge-0.0.3/LICENSE` & `python-bridge-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/PKG-INFO` & `python-bridge-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.3/bridge/cli/bridge.py` & `python-bridge-0.0.4/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/bridge/cli/deploy/base.py` & `python-bridge-0.0.4/bridge/cli/deploy/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def upload(self, zip_path: Path):
         with log_task(
             start_message="Uploading bundle...", end_message="Bundle uploaded"
         ):
             storage_client = storage.Client()
             bucket = storage_client.bucket(self.bucket_name)
-            destination_blob_name = f"deploys/{uuid.uuid4()}.zip"
+            destination_blob_name = f"deploys/{self.deploy_name}.zip"
             blob = bucket.blob(destination_blob_name)
             blob.upload_from_filename(str(zip_path))
 
     def deploy(self):
         console = Console()
         console.print("Deploying...", style="bold green")
         self.validate()
```

### Comparing `python-bridge-0.0.3/bridge/cli/deploy/django.py` & `python-bridge-0.0.4/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/bridge/console.py` & `python-bridge-0.0.4/bridge/console.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,7 +23,12 @@
                 highlight=False,
             )
 
 
 def log_error(message):
     console = Console()
     console.print(f"[bright_red]✗ Bridge Error[/bright_red]: {message}")
+
+
+def log_warning(message):
+    console = Console()
+    console.print(f"[yellow]Bridge Warning[/yellow]: {message}")
```

### Comparing `python-bridge-0.0.3/bridge/framework/base.py` & `python-bridge-0.0.4/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/bridge/service/docker.py` & `python-bridge-0.0.4/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/bridge/service/postgres.py` & `python-bridge-0.0.4/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.3/pyproject.toml` & `python-bridge-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.3/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.4/python_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.3/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.4/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

