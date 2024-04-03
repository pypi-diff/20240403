# Comparing `tmp/netlink-keepass-0.4.1.tar.gz` & `tmp/netlink-keepass-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netlink-keepass-0.4.1.tar", max compression
+gzip compressed data, was "netlink-keepass-0.5.0.tar", max compression
```

## Comparing `netlink-keepass-0.4.1.tar` & `netlink-keepass-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      112 2024-02-08 14:32:57.009088 netlink-keepass-0.4.1/netlink/keepass/__init__.py
--rw-r--r--   0        0        0     2719 2024-02-12 15:57:54.991537 netlink-keepass-0.4.1/netlink/keepass/cli.py
--rw-r--r--   0        0        0     1240 2024-02-12 15:09:25.357668 netlink-keepass-0.4.1/netlink/keepass/keepass.py
--rw-r--r--   0        0        0     1362 2024-02-12 15:09:25.377969 netlink-keepass-0.4.1/netlink/keepass/reader.py
--rw-r--r--   0        0        0     1019 2024-02-12 15:32:48.939329 netlink-keepass-0.4.1/netlink/keepass/util.py
--rw-r--r--   0        0        0      971 2024-02-12 15:59:18.224812 netlink-keepass-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1290 2024-02-12 15:59:28.228753 netlink-keepass-0.4.1/setup.py
--rw-r--r--   0        0        0      684 2024-02-12 15:59:28.228753 netlink-keepass-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      112 2024-02-08 14:32:57.009088 netlink-keepass-0.5.0/netlink/keepass/__init__.py
+-rw-r--r--   0        0        0     2719 2024-02-12 15:57:54.991537 netlink-keepass-0.5.0/netlink/keepass/cli.py
+-rw-r--r--   0        0        0     1561 2024-04-03 08:47:59.415880 netlink-keepass-0.5.0/netlink/keepass/keepass.py
+-rw-r--r--   0        0        0     1384 2024-04-03 08:47:59.396914 netlink-keepass-0.5.0/netlink/keepass/reader.py
+-rw-r--r--   0        0        0     1019 2024-02-12 15:32:48.939329 netlink-keepass-0.5.0/netlink/keepass/util.py
+-rw-r--r--   0        0        0      971 2024-04-03 08:44:27.229256 netlink-keepass-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1290 2024-04-03 08:53:52.733897 netlink-keepass-0.5.0/setup.py
+-rw-r--r--   0        0        0      684 2024-04-03 08:53:52.734898 netlink-keepass-0.5.0/PKG-INFO
```

### Comparing `netlink-keepass-0.4.1/netlink/keepass/cli.py` & `netlink-keepass-0.5.0/netlink/keepass/cli.py`

 * *Files identical despite different names*

### Comparing `netlink-keepass-0.4.1/netlink/keepass/reader.py` & `netlink-keepass-0.5.0/netlink/keepass/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
-import signal
 import pathlib
+import signal
 
 import fastapi
 import uvicorn
 
 from netlink.keepass.keepass import KeePass
 
-
 app = fastapi.FastAPI()
 
 
 # noinspection PyUnresolvedReferences
 @app.get("/{full_path:path}")
 async def get_value(full_path: str):
     if full_path.startswith(app.state.shutdown):
@@ -21,20 +20,20 @@
         return app.state.kp.get(full_path)
     except KeyError:
         raise fastapi.HTTPException(status_code=404, detail=f"{full_path} not found")
 
 
 # noinspection PyUnresolvedReferences
 def reader(
-    filename: pathlib.Path,
-    secret: str,
-    keyfile: pathlib.Path = None,
-    token: pathlib.Path = None,
-    port: int = 8666,
-    shutdown: str = "_shutdown",
+        filename: pathlib.Path,
+        secret: str,
+        keyfile: pathlib.Path = None,
+        token: pathlib.Path = None,
+        port: int = 8666,
+        shutdown: str = "_shutdown",
 ) -> None:
     """Start REST server to read KeePass
 
     :param filename: KeePass Database file
     :param secret: Password for KeePass database or Key for Fernet
     :param keyfile: KeePass key file
     :param token: Fernet token file
```

### Comparing `netlink-keepass-0.4.1/netlink/keepass/util.py` & `netlink-keepass-0.5.0/netlink/keepass/util.py`

 * *Files identical despite different names*

### Comparing `netlink-keepass-0.4.1/pyproject.toml` & `netlink-keepass-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "netlink-keepass"
-version = "0.4.1"
+version = "0.5.0"
 description = "Tools to work with (Py)KeePass"
 authors = ["Bernhard Radermacher <bernhard.radermacher@netlink-consulting.com>"]
 repository = "https://gitlab.com/netlink_python/netlink-keepass.git"
 packages = [ { include = "netlink/keepass" } ]
 
 [tool.poetry.scripts]
 netlink-keepass-rest-reader = 'netlink.keepass.cli:reader_cli'
 netlink-keepass-fernet-token = 'netlink.keepass.cli:fernet_token_cli'
 netlink-keepass-rest-get = 'netlink.keepass.cli:rest_get_cli'
 netlink-keepass-rest-shutdown = 'netlink.keepass.cli:rest_shutdown_cli'
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = ">=3.8.1,<3.13"
 click = ">=8.1.7"
 pykeepass = ">=4.0.6"
 fastapi = ">=0.109.0"
 uvicorn = ">=0.27.0"
 cryptography = ">=42.0.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `netlink-keepass-0.4.1/setup.py` & `netlink-keepass-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,24 +22,24 @@
                      'netlink-keepass-rest-reader = '
                      'netlink.keepass.cli:reader_cli',
                      'netlink-keepass-rest-shutdown = '
                      'netlink.keepass.cli:rest_shutdown_cli']}
 
 setup_kwargs = {
     'name': 'netlink-keepass',
-    'version': '0.4.1',
+    'version': '0.5.0',
     'description': 'Tools to work with (Py)KeePass',
     'long_description': None,
     'author': 'Bernhard Radermacher',
     'author_email': 'bernhard.radermacher@netlink-consulting.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://gitlab.com/netlink_python/netlink-keepass.git',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.8.1,<3.12',
+    'python_requires': '>=3.8.1,<3.13',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `netlink-keepass-0.4.1/PKG-INFO` & `netlink-keepass-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: netlink-keepass
-Version: 0.4.1
+Version: 0.5.0
 Summary: Tools to work with (Py)KeePass
 Home-page: https://gitlab.com/netlink_python/netlink-keepass.git
 Author: Bernhard Radermacher
 Author-email: bernhard.radermacher@netlink-consulting.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: click (>=8.1.7)
 Requires-Dist: cryptography (>=42.0.1)
 Requires-Dist: fastapi (>=0.109.0)
 Requires-Dist: pykeepass (>=4.0.6)
```

