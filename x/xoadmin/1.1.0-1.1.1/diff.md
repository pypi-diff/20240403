# Comparing `tmp/xoadmin-1.1.0.tar.gz` & `tmp/xoadmin-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xoadmin-1.1.0.tar", max compression
+gzip compressed data, was "xoadmin-1.1.1.tar", max compression
```

## Comparing `xoadmin-1.1.0.tar` & `xoadmin-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11336 2024-04-03 17:41:50.542843 xoadmin-1.1.0/LICENSE
--rw-r--r--   0        0        0     1904 2024-04-03 17:41:50.542843 xoadmin-1.1.0/README.md
--rw-r--r--   0        0        0      786 2024-04-03 17:41:50.542843 xoadmin-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/__init__.py
--rw-r--r--   0        0        0      717 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/__main__.py
--rw-r--r--   0        0        0     4536 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/api.py
--rw-r--r--   0        0        0      389 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/error.py
--rw-r--r--   0        0        0     1249 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/host.py
--rw-r--r--   0        0        0     5138 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/manager.py
--rw-r--r--   0        0        0      816 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/storage.py
--rw-r--r--   0        0        0     2381 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/user.py
--rw-r--r--   0        0        0     1523 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/vm.py
--rw-r--r--   0        0        0     5719 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/api/websocket.py
--rw-r--r--   0        0        0        0 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/__init__.py
--rw-r--r--   0        0        0      614 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/config.py
--rw-r--r--   0        0        0     1287 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/configurator.py
--rw-r--r--   0        0        0      274 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/configurator/loader.py
--rw-r--r--   0        0        0     1822 2024-04-03 17:41:50.542843 xoadmin-1.1.0/src/xoadmin/utils.py
--rw-r--r--   0        0        0     2772 1970-01-01 00:00:00.000000 xoadmin-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-03 18:28:34.045574 xoadmin-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1904 2024-04-03 18:28:34.045574 xoadmin-1.1.1/README.md
+-rw-r--r--   0        0        0      788 2024-04-03 18:28:34.049574 xoadmin-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/__init__.py
+-rw-r--r--   0        0        0      631 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/__main__.py
+-rw-r--r--   0        0        0     4536 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/api.py
+-rw-r--r--   0        0        0      389 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/error.py
+-rw-r--r--   0        0        0     1249 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/host.py
+-rw-r--r--   0        0        0     5138 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/manager.py
+-rw-r--r--   0        0        0      816 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/storage.py
+-rw-r--r--   0        0        0     2381 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/user.py
+-rw-r--r--   0        0        0     1523 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/vm.py
+-rw-r--r--   0        0        0     5719 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/api/websocket.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/__init__.py
+-rw-r--r--   0        0        0      614 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/config.py
+-rw-r--r--   0        0        0     1287 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/configurator.py
+-rw-r--r--   0        0        0      274 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/configurator/loader.py
+-rw-r--r--   0        0        0     1822 2024-04-03 18:28:34.049574 xoadmin-1.1.1/src/xoadmin/utils.py
+-rw-r--r--   0        0        0     2768 1970-01-01 00:00:00.000000 xoadmin-1.1.1/PKG-INFO
```

### Comparing `xoadmin-1.1.0/LICENSE` & `xoadmin-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/README.md` & `xoadmin-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/pyproject.toml` & `xoadmin-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "xoadmin"
-version = "1.1.0"
+version = "1.1.1"
 description = "bindings and wrappers to manage an XOA instance"
 authors = ["dennis <it.admin@elnissi.co.id>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{ include = "xoadmin", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.9.2"
 jinja2 = "^3.1.3"
 python-dotenv = "^1.0.1"
 requests = "^2.31.0"
 httpx = "^0.27.0"
 colorlog = "^6.8.2"
 websockets = "^12.0"
 pydantic = "^2.6.4"
```

### Comparing `xoadmin-1.1.0/src/xoadmin/api/api.py` & `xoadmin-1.1.1/src/xoadmin/api/api.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/host.py` & `xoadmin-1.1.1/src/xoadmin/api/host.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/manager.py` & `xoadmin-1.1.1/src/xoadmin/api/manager.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/storage.py` & `xoadmin-1.1.1/src/xoadmin/api/storage.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/user.py` & `xoadmin-1.1.1/src/xoadmin/api/user.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/vm.py` & `xoadmin-1.1.1/src/xoadmin/api/vm.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/api/websocket.py` & `xoadmin-1.1.1/src/xoadmin/api/websocket.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/configurator/config.py` & `xoadmin-1.1.1/src/xoadmin/configurator/config.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/configurator/configurator.py` & `xoadmin-1.1.1/src/xoadmin/configurator/configurator.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/src/xoadmin/utils.py` & `xoadmin-1.1.1/src/xoadmin/utils.py`

 * *Files identical despite different names*

### Comparing `xoadmin-1.1.0/PKG-INFO` & `xoadmin-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: xoadmin
-Version: 1.1.0
+Version: 1.1.1
 Summary: bindings and wrappers to manage an XOA instance
 License: Apache 2.0
 Author: dennis
 Author-email: it.admin@elnissi.co.id
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9.2
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorlog (>=6.8.2,<7.0.0)
```

