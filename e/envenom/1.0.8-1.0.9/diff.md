# Comparing `tmp/envenom-1.0.8.tar.gz` & `tmp/envenom-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envenom-1.0.8.tar", max compression
+gzip compressed data, was "envenom-1.0.9.tar", max compression
```

## Comparing `envenom-1.0.8.tar` & `envenom-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35145 2024-03-10 17:49:14.024313 envenom-1.0.8/LICENSE
--rw-r--r--   0        0        0     7162 2024-03-10 17:49:14.024313 envenom-1.0.8/README.md
--rw-r--r--   0        0        0     2576 2024-03-10 17:49:14.025313 envenom-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      936 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/__init__.py
--rw-r--r--   0        0        0     3499 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/configs.py
--rw-r--r--   0        0        0     2057 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/entries.py
--rw-r--r--   0        0        0     1471 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/errors.py
--rw-r--r--   0        0        0     3736 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/examples/advanced.py
--rw-r--r--   0        0        0     1454 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/examples/fastapi.py
--rw-r--r--   0        0        0     3001 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/examples/quickstart.py
--rw-r--r--   0        0        0     1394 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/parsers.py
--rw-r--r--   0        0        0        0 2024-03-10 17:49:14.051312 envenom-1.0.8/src/envenom/py.typed
--rw-r--r--   0        0        0     4076 2024-03-10 17:49:14.025313 envenom-1.0.8/src/envenom/vars.py
--rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 envenom-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35145 2024-04-03 12:51:41.122433 envenom-1.0.9/LICENSE
+-rw-r--r--   0        0        0     7162 2024-04-03 12:51:41.122433 envenom-1.0.9/README.md
+-rw-r--r--   0        0        0     2576 2024-04-03 12:51:41.122433 envenom-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      936 2024-04-03 12:51:41.122433 envenom-1.0.9/src/envenom/__init__.py
+-rw-r--r--   0        0        0     3499 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/configs.py
+-rw-r--r--   0        0        0     2057 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/entries.py
+-rw-r--r--   0        0        0     1471 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/errors.py
+-rw-r--r--   0        0        0     3736 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/examples/advanced.py
+-rw-r--r--   0        0        0     1454 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/examples/fastapi.py
+-rw-r--r--   0        0        0     3001 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/examples/quickstart.py
+-rw-r--r--   0        0        0     1394 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/parsers.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:51:41.151433 envenom-1.0.9/src/envenom/py.typed
+-rw-r--r--   0        0        0     4076 2024-04-03 12:51:41.123433 envenom-1.0.9/src/envenom/vars.py
+-rw-r--r--   0        0        0     8363 1970-01-01 00:00:00.000000 envenom-1.0.9/PKG-INFO
```

### Comparing `envenom-1.0.8/LICENSE` & `envenom-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/README.md` & `envenom-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/pyproject.toml` & `envenom-1.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "envenom"
 description = "An elegant application configurator for the more civilized age"
-version = "1.0.8"
+version = "1.0.9"
 license = "GPL-3.0-or-later"
 authors = ["Artur Ciesielski <artur.ciesielski@gmail.com>"]
 readme = "README.md"
 homepage = "https://gitlab.com/python-arcana/envenom"
 repository = "https://gitlab.com/python-arcana/envenom"
 documentation = "https://gitlab.com/python-arcana/envenom/-/wikis/Home"
 keywords = ["env", "environment", "config", "configuration"]
```

### Comparing `envenom-1.0.8/src/envenom/__init__.py` & `envenom-1.0.9/src/envenom/__init__.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/configs.py` & `envenom-1.0.9/src/envenom/configs.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/entries.py` & `envenom-1.0.9/src/envenom/entries.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/errors.py` & `envenom-1.0.9/src/envenom/errors.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/examples/advanced.py` & `envenom-1.0.9/src/envenom/examples/advanced.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/examples/fastapi.py` & `envenom-1.0.9/src/envenom/examples/fastapi.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/examples/quickstart.py` & `envenom-1.0.9/src/envenom/examples/quickstart.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/parsers.py` & `envenom-1.0.9/src/envenom/parsers.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/src/envenom/vars.py` & `envenom-1.0.9/src/envenom/vars.py`

 * *Files identical despite different names*

### Comparing `envenom-1.0.8/PKG-INFO` & `envenom-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envenom
-Version: 1.0.8
+Version: 1.0.9
 Summary: An elegant application configurator for the more civilized age
 Home-page: https://gitlab.com/python-arcana/envenom
 License: GPL-3.0-or-later
 Keywords: env,environment,config,configuration
 Author: Artur Ciesielski
 Author-email: artur.ciesielski@gmail.com
 Requires-Python: >=3.10,<4.0
```

