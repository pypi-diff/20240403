# Comparing `tmp/PyOracleClient-0.2.5.tar.gz` & `tmp/PyOracleClient-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyOracleClient-0.2.5.tar", last modified: Tue Dec 29 02:27:19 2020, max compression
+gzip compressed data, was "PyOracleClient-0.2.6.tar", last modified: Wed Apr  3 14:39:41 2024, max compression
```

## Comparing `PyOracleClient-0.2.5.tar` & `PyOracleClient-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 Luca       (501) staff       (20)        0 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/
--rw-r--r--   0 Luca       (501) staff       (20)     3630 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PKG-INFO
-drwxr-xr-x   0 Luca       (501) staff       (20)        0 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/
--rw-r--r--   0 Luca       (501) staff       (20)     3630 2020-12-29 02:27:18.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/PKG-INFO
--rw-r--r--   0 Luca       (501) staff       (20)      298 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/SOURCES.txt
--rw-r--r--   0 Luca       (501) staff       (20)        1 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/dependency_links.txt
--rw-r--r--   0 Luca       (501) staff       (20)        5 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/requires.txt
--rw-r--r--   0 Luca       (501) staff       (20)       15 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/PyOracleClient.egg-info/top_level.txt
--rwxr-xr-x   0 Luca       (501) staff       (20)     2562 2020-12-29 02:26:45.000000 PyOracleClient-0.2.5/README.md
-drwxr-xr-x   0 Luca       (501) staff       (20)        0 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/pyoracleclient/
--rwxr-xr-x   0 Luca       (501) staff       (20)      343 2020-12-29 02:26:25.000000 PyOracleClient-0.2.5/pyoracleclient/__init__.py
--rw-r--r--   0 Luca       (501) staff       (20)     5466 2020-12-29 02:21:45.000000 PyOracleClient-0.2.5/pyoracleclient/pyoracleclient.py
--rw-r--r--   0 Luca       (501) staff       (20)      794 2020-12-25 19:50:38.000000 PyOracleClient-0.2.5/pyoracleclient/tns_template.py
--rw-r--r--   0 Luca       (501) staff       (20)       38 2020-12-29 02:27:19.000000 PyOracleClient-0.2.5/setup.cfg
--rwxr-xr-x   0 Luca       (501) staff       (20)      848 2020-12-28 19:41:34.000000 PyOracleClient-0.2.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     1073 2024-04-03 14:23:52.000000 PyOracleClient-0.2.6/LICENSE.txt
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4234 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/PKG-INFO
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/PyOracleClient.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)     4234 2024-04-03 14:39:41.000000 PyOracleClient-0.2.6/PyOracleClient.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      338 2024-04-03 14:39:41.000000 PyOracleClient-0.2.6/PyOracleClient.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-04-03 14:39:41.000000 PyOracleClient-0.2.6/PyOracleClient.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        5 2024-04-03 14:39:41.000000 PyOracleClient-0.2.6/PyOracleClient.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       15 2024-04-03 14:39:41.000000 PyOracleClient-0.2.6/PyOracleClient.egg-info/top_level.txt
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)     3711 2024-04-03 14:38:07.000000 PyOracleClient-0.2.6/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/pyoracleclient/
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      345 2024-04-03 14:31:33.000000 PyOracleClient-0.2.6/pyoracleclient/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5482 2024-04-03 14:23:52.000000 PyOracleClient-0.2.6/pyoracleclient/pyoracleclient.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/pyoracleclient/res/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   105266 2024-04-03 14:23:52.000000 PyOracleClient-0.2.6/pyoracleclient/res/icon.png
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      794 2024-04-03 14:23:52.000000 PyOracleClient-0.2.6/pyoracleclient/tns_template.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-04-03 14:39:41.854146 PyOracleClient-0.2.6/setup.cfg
+-rwxrwxrwx   0 codespace  (1000) codespace  (1000)      848 2024-04-03 14:23:52.000000 PyOracleClient-0.2.6/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyOracleClient-0.2.5/pyoracleclient/pyoracleclient.py` & `PyOracleClient-0.2.6/pyoracleclient/pyoracleclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Created on Thu Dec 24 10:10:01 2020
 @author: Luca Mingarelli
 """
+from pathlib import Path
+
 from pyoracleclient import __file__
 import ntpath, os, shutil
 from datetime import datetime
 from pyoracleclient.tns_template import _TNS_TEMPLATE
 
 _ROOT = ntpath.dirname(__file__)
 _TNSORA_PATH = f'{_ROOT}/instantclient/network/admin/tnsnames.ora'
@@ -99,15 +101,15 @@
     new_tns = _TNS_TEMPLATE.format(_name=name, _failover=failover, _load_balance=load_balance,
                                    _protocol1=protocol1, _host1=host1, _port1=port1,
                                    _protocol2=protocol2, _host2=host2, _port2=port2,
                                    _service_name=service_name)
 
     if not os.path.exists(_TNSORA_PATH):
         os.makedirs(ntpath.dirname(_TNSORA_PATH), exist_ok=True)
-        os.system(f"touch '{_TNSORA_PATH}'")
+        Path(_TNSORA_PATH).touch()
     with open(_TNSORA_PATH, "a+") as f:
         f.write(new_tns)
         f.write('\n')
 
 
 def add_custom_tns(tns):
     """Adds the tns specification to the file tnsnames.ora.
```

### Comparing `PyOracleClient-0.2.5/pyoracleclient/tns_template.py` & `PyOracleClient-0.2.6/pyoracleclient/tns_template.py`

 * *Files identical despite different names*

### Comparing `PyOracleClient-0.2.5/setup.py` & `PyOracleClient-0.2.6/setup.py`

 * *Files identical despite different names*

