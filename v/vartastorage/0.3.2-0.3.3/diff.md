# Comparing `tmp/vartastorage-0.3.2.tar.gz` & `tmp/vartastorage-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vartastorage-0.3.2.tar", last modified: Mon Apr  1 11:01:41 2024, max compression
+gzip compressed data, was "vartastorage-0.3.3.tar", last modified: Wed Apr  3 17:50:59 2024, max compression
```

## Comparing `vartastorage-0.3.2.tar` & `vartastorage-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.704043 vartastorage-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 11:01:41.700043 vartastorage-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-01 11:01:37.000000 vartastorage-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 11:01:41.704043 vartastorage-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 11:01:37.000000 vartastorage-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/vartastorage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/cgi_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/cgi_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/modbus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-01 11:01:37.000000 vartastorage-0.3.2/src/vartastorage/vartastorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 11:01:41.700043 vartastorage-0.3.2/src/vartastorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 11:01:41.000000 vartastorage-0.3.2/src/vartastorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:50:59.085394 vartastorage-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-03 17:50:59.085394 vartastorage-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-03 17:50:54.000000 vartastorage-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:50:59.085394 vartastorage-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 17:50:54.000000 vartastorage-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:50:59.081394 vartastorage-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:50:59.081394 vartastorage-0.3.3/src/vartastorage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:50:54.000000 vartastorage-0.3.3/src/vartastorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-03 17:50:54.000000 vartastorage-0.3.3/src/vartastorage/cgi_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2024-04-03 17:50:54.000000 vartastorage-0.3.3/src/vartastorage/cgi_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-03 17:50:54.000000 vartastorage-0.3.3/src/vartastorage/modbus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-03 17:50:54.000000 vartastorage-0.3.3/src/vartastorage/vartastorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:50:59.085394 vartastorage-0.3.3/src/vartastorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-03 17:50:59.000000 vartastorage-0.3.3/src/vartastorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 17:50:59.000000 vartastorage-0.3.3/src/vartastorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:50:59.000000 vartastorage-0.3.3/src/vartastorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:50:58.000000 vartastorage-0.3.3/src/vartastorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 17:50:59.000000 vartastorage-0.3.3/src/vartastorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 17:50:59.000000 vartastorage-0.3.3/src/vartastorage.egg-info/top_level.txt
```

### Comparing `vartastorage-0.3.2/README.md` & `vartastorage-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `vartastorage-0.3.2/setup.py` & `vartastorage-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="vartastorage",
-    version="0.3.2",
+    version="0.3.3",
     description="VARTA Battery",
     long_description="""
         With this Python module you can read modbus registers
         and xml/cgi api values from various VARTA batteries""",
     url="http://github.com/vip0r/vartastorage",
     author="edAndy",
     author_email="an-dy@gmx.de",
```

### Comparing `vartastorage-0.3.2/src/vartastorage/cgi_client.py` & `vartastorage-0.3.3/src/vartastorage/cgi_client.py`

 * *Files identical despite different names*

### Comparing `vartastorage-0.3.2/src/vartastorage/cgi_data.py` & `vartastorage-0.3.3/src/vartastorage/cgi_data.py`

 * *Files identical despite different names*

### Comparing `vartastorage-0.3.2/src/vartastorage/modbus_client.py` & `vartastorage-0.3.3/src/vartastorage/modbus_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,17 @@
 
 class ModbusClient:
     def __init__(self, modbus_host, modbus_port) -> None:
         self._slave = 255
 
         self.modbus_host = modbus_host
         self.modbus_port = modbus_port
-        self._modbus_client = ModbusTcpClient(self.modbus_host, self.modbus_port)
+        self._modbus_client = ModbusTcpClient(
+            host=self.modbus_host, port=self.modbus_port, unit_id=255
+        )
 
     def connect(self) -> bool:
         return self._modbus_client.connect()
 
     def disconnect(self) -> None:
         return self._modbus_client.close()
```

### Comparing `vartastorage-0.3.2/src/vartastorage/vartastorage.py` & `vartastorage-0.3.3/src/vartastorage/vartastorage.py`

 * *Files identical despite different names*

