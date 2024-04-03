# Comparing `tmp/config2py-0.1.8.tar.gz` & `tmp/config2py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config2py-0.1.8.tar", last modified: Thu Sep 14 15:29:59 2023, max compression
+gzip compressed data, was "config2py-0.1.9.tar", last modified: Thu Sep 14 18:12:51 2023, max compression
```

## Comparing `config2py-0.1.8.tar` & `config2py-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:59.111926 config2py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-14 15:29:05.000000 config2py-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-14 15:29:59.111926 config2py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-09-14 15:29:05.000000 config2py-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:59.107926 config2py-0.1.8/config2py/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14879 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    15676 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/s_configparser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:59.111926 config2py-0.1.8/config2py/scrap/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/scrap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:59.111926 config2py-0.1.8/config2py/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-09-14 15:29:05.000000 config2py-0.1.8/config2py/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2023-09-14 15:29:57.000000 config2py-0.1.8/config2py/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 15:29:59.111926 config2py-0.1.8/config2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-14 15:29:58.000000 config2py-0.1.8/config2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2023-09-14 15:29:59.000000 config2py-0.1.8/config2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 15:29:58.000000 config2py-0.1.8/config2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 15:29:58.000000 config2py-0.1.8/config2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-14 15:29:58.000000 config2py-0.1.8/config2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-14 15:29:58.000000 config2py-0.1.8/config2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-09-14 15:29:59.111926 config2py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-14 15:29:05.000000 config2py-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:51.251839 config2py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-14 18:12:08.000000 config2py-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-14 18:12:51.251839 config2py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2023-09-14 18:12:08.000000 config2py-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:51.247839 config2py-0.1.9/config2py/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14879 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15676 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/s_configparser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:51.251839 config2py-0.1.9/config2py/scrap/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/scrap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:51.251839 config2py-0.1.9/config2py/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-14 18:12:08.000000 config2py-0.1.9/config2py/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-09-14 18:12:48.000000 config2py-0.1.9/config2py/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2023-09-14 18:12:49.000000 config2py-0.1.9/config2py/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-14 18:12:51.251839 config2py-0.1.9/config2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2023-09-14 18:12:50.000000 config2py-0.1.9/config2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2023-09-14 18:12:51.000000 config2py-0.1.9/config2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 18:12:50.000000 config2py-0.1.9/config2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-14 18:12:50.000000 config2py-0.1.9/config2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-14 18:12:50.000000 config2py-0.1.9/config2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-14 18:12:50.000000 config2py-0.1.9/config2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-09-14 18:12:51.251839 config2py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-09-14 18:12:08.000000 config2py-0.1.9/setup.py
```

### Comparing `config2py-0.1.8/LICENSE` & `config2py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `config2py-0.1.8/PKG-INFO` & `config2py-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config2py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simplified reading and writing configurations from various sources and formats
 Home-page: https://github.com/i2mint/config2py
 Author: OtoSense
 License: apache-2.0
 Description: # config2py
         
         Simplified reading and writing configurations from various sources and formats.
```

### Comparing `config2py-0.1.8/README.md` & `config2py-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `config2py-0.1.8/config2py/base.py` & `config2py-0.1.9/config2py/base.py`

 * *Files identical despite different names*

### Comparing `config2py-0.1.8/config2py/s_configparser.py` & `config2py-0.1.9/config2py/s_configparser.py`

 * *Files identical despite different names*

### Comparing `config2py-0.1.8/config2py/tools.py` & `config2py-0.1.9/config2py/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,27 @@
 """Various tools"""
 
 from pathlib import Path
 import re
 import getpass
 from dol import Pipe, resolve_path
+import os
+from config2py.util import local_configs
+from config2py.base import get_config, user_gettable
+
+
+config_getter = get_config(
+    sources=[
+        os.environ,  # search in environment variables first
+        local_configs,  # then search in local_configs
+        user_gettable(
+            local_configs
+        ),  # if not found, ask the user and store in local_configs
+    ]
+)
 
 export_line_p = re.compile('export .+')
 export_p = re.compile(r'(\w+)\s?\=\s?"(.+)"')
 
 _extract_name_and_value_from_export_line = Pipe(
     lambda x: x[len('export ') :],
     lambda x: export_p.match(x),
```

### Comparing `config2py-0.1.8/config2py/util.py` & `config2py-0.1.9/config2py/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -250,15 +250,16 @@
 
 
 def get_configs_local_store(dirname=DFLT_APP_NAME):
     """Get the local store of configs."""
     return Configs(get_app_data_directory(dirname))
 
 
-configs = get_configs_local_store()
+local_configs = get_configs_local_store()
+configs = local_configs  # TODO: backwards compatibility alias
 
 
 # def extract_variable_declarations(string):
 #     """
 #     Reads the contents of a config file, extracting Unix-style environment variable
 #     declarations of the form
 #     `export {NAME}={value}`, returning a dictionary of `{NAME: value, ...}` pairs.
```

### Comparing `config2py-0.1.8/config2py.egg-info/PKG-INFO` & `config2py-0.1.9/config2py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config2py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simplified reading and writing configurations from various sources and formats
 Home-page: https://github.com/i2mint/config2py
 Author: OtoSense
 License: apache-2.0
 Description: # config2py
         
         Simplified reading and writing configurations from various sources and formats.
```

### Comparing `config2py-0.1.8/setup.cfg` & `config2py-0.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = config2py
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/i2mint/config2py
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = Simplified reading and writing configurations from various sources and formats
```

