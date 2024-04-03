# Comparing `tmp/esrt-1.24.0.tar.gz` & `tmp/esrt-1.25.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esrt-1.24.0.tar", last modified: Wed Apr  3 05:08:33 2024, max compression
+gzip compressed data, was "esrt-1.25.0.tar", last modified: Wed Apr  3 05:46:15 2024, max compression
```

## Comparing `esrt-1.24.0.tar` & `esrt-1.25.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:08:33.249637 esrt-1.24.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-03 05:08:33.249637 esrt-1.24.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9840 2024-04-03 05:08:17.000000 esrt-1.24.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 05:08:17.000000 esrt-1.24.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:08:33.249637 esrt-1.24.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:08:33.245637 esrt-1.24.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:08:33.245637 esrt-1.24.0/src/esrt/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 05:08:17.000000 esrt-1.24.0/src/esrt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:08:33.249637 esrt-1.24.0/src/esrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 05:08:33.000000 esrt-1.24.0/src/esrt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:15.683805 esrt-1.25.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-04-03 05:46:15.683805 esrt-1.25.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-04-03 05:45:56.000000 esrt-1.25.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 05:45:56.000000 esrt-1.25.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:46:15.683805 esrt-1.25.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:15.679805 esrt-1.25.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:15.683805 esrt-1.25.0/src/esrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 05:45:56.000000 esrt-1.25.0/src/esrt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:15.683805 esrt-1.25.0/src/esrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10218 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 05:46:15.000000 esrt-1.25.0/src/esrt.egg-info/top_level.txt
```

### Comparing `esrt-1.24.0/PKG-INFO` & `esrt-1.25.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: esrt
-Version: 1.24.0
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Requires-Dist: elasticsearch==6.8.2
-Requires-Dist: typer-slim[standard]>=0.12.0
-Requires-Dist: uvicorn>=0.2.14
-
 # esrt - Elasticsearch Request Tool
 
 [![pypi](https://img.shields.io/pypi/v/esrt.svg)](https://pypi.python.org/pypi/esrt)
 
 ```sh
 pip install pipx
 pipx install esrt -f
@@ -128,15 +119,15 @@
 ---
 
 Pipe `_search` result and update `_index` with `customized handler` to do more operations before bulk!
 
 ```sh
 alias jq_es_hits="jq '.hits.hits.[]'"
 #
-esrt r localhost -X GET /my-index-2/_search | jq_es_hits  -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
+esrt r localhost -X GET /my-index-2/_search | jq_es_hits -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
 # ->
 # <Client([{'host': 'localhost', 'port': 9200}])>
 # streaming_bulk  [####################################]  3
 
 # success = 3
 # failed = 0
 ```
@@ -157,15 +148,19 @@
             obj['_index'] = prefix + obj['_index']
         return obj
 
 
 # function style
 def my_handler(actions: t.Iterable[str]):
     for action in actions:
-        yield json.loads(action)
+        obj = json.loads(action)
+        prefix = 'new-'
+        if not t.cast(str, obj['_index']).startswith(prefix):
+            obj['_index'] = prefix + obj['_index']
+        yield obj
 ```
 
 ---
 
 ## `e` Search docs
 
 ```sh
```

### Comparing `esrt-1.24.0/README.md` & `esrt-1.25.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: esrt
+Version: 1.25.0
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Requires-Dist: elasticsearch==6.8.2
+Requires-Dist: typer-slim[standard]>=0.12.0
+Requires-Dist: uvicorn>=0.2.14
+
 # esrt - Elasticsearch Request Tool
 
 [![pypi](https://img.shields.io/pypi/v/esrt.svg)](https://pypi.python.org/pypi/esrt)
 
 ```sh
 pip install pipx
 pipx install esrt -f
@@ -119,15 +128,15 @@
 ---
 
 Pipe `_search` result and update `_index` with `customized handler` to do more operations before bulk!
 
 ```sh
 alias jq_es_hits="jq '.hits.hits.[]'"
 #
-esrt r localhost -X GET /my-index-2/_search | jq_es_hits  -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
+esrt r localhost -X GET /my-index-2/_search | jq_es_hits -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
 # ->
 # <Client([{'host': 'localhost', 'port': 9200}])>
 # streaming_bulk  [####################################]  3
 
 # success = 3
 # failed = 0
 ```
@@ -148,15 +157,19 @@
             obj['_index'] = prefix + obj['_index']
         return obj
 
 
 # function style
 def my_handler(actions: t.Iterable[str]):
     for action in actions:
-        yield json.loads(action)
+        obj = json.loads(action)
+        prefix = 'new-'
+        if not t.cast(str, obj['_index']).startswith(prefix):
+            obj['_index'] = prefix + obj['_index']
+        yield obj
 ```
 
 ---
 
 ## `e` Search docs
 
 ```sh
```

### Comparing `esrt-1.24.0/pyproject.toml` & `esrt-1.25.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "esrt"
-version = "1.24.0"
+version = "1.25.0"
 requires-python = ">=3.9"
 readme = "README.md"
 dependencies = [
     "elasticsearch==6.8.2",
     "typer-slim[standard]>=0.12.0",
     # uvicorn.importer.import_from_string
     "uvicorn>=0.2.14",
```

### Comparing `esrt-1.24.0/src/esrt/__main__.py` & `esrt-1.25.0/src/esrt/__main__.py`

 * *Files identical despite different names*

### Comparing `esrt-1.24.0/src/esrt/handlers.py` & `esrt-1.25.0/src/esrt/handlers.py`

 * *Files identical despite different names*

### Comparing `esrt-1.24.0/src/esrt/utils.py` & `esrt-1.25.0/src/esrt/utils.py`

 * *Files identical despite different names*

### Comparing `esrt-1.24.0/src/esrt.egg-info/PKG-INFO` & `esrt-1.25.0/src/esrt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.24.0
+Version: 1.25.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
@@ -128,15 +128,15 @@
 ---
 
 Pipe `_search` result and update `_index` with `customized handler` to do more operations before bulk!
 
 ```sh
 alias jq_es_hits="jq '.hits.hits.[]'"
 #
-esrt r localhost -X GET /my-index-2/_search | jq_es_hits  -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
+esrt r localhost -X GET /my-index-2/_search | jq_es_hits -c | esrt t localhost -w examples.my-handlers:MyHandler  # <- `examples/my-handlers.py`
 # ->
 # <Client([{'host': 'localhost', 'port': 9200}])>
 # streaming_bulk  [####################################]  3
 
 # success = 3
 # failed = 0
 ```
@@ -157,15 +157,19 @@
             obj['_index'] = prefix + obj['_index']
         return obj
 
 
 # function style
 def my_handler(actions: t.Iterable[str]):
     for action in actions:
-        yield json.loads(action)
+        obj = json.loads(action)
+        prefix = 'new-'
+        if not t.cast(str, obj['_index']).startswith(prefix):
+            obj['_index'] = prefix + obj['_index']
+        yield obj
 ```
 
 ---
 
 ## `e` Search docs
 
 ```sh
```

