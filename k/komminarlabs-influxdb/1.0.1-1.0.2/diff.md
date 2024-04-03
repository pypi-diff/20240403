# Comparing `tmp/komminarlabs_influxdb-1.0.1.tar.gz` & `tmp/komminarlabs_influxdb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komminarlabs_influxdb-1.0.1.tar", last modified: Wed Mar 13 10:20:36 2024, max compression
+gzip compressed data, was "komminarlabs_influxdb-1.0.2.tar", last modified: Wed Apr  3 16:46:58 2024, max compression
```

## Comparing `komminarlabs_influxdb-1.0.1.tar` & `komminarlabs_influxdb-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:20:36.724397 komminarlabs_influxdb-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-13 10:20:36.724397 komminarlabs_influxdb-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:20:36.720397 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/bucket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:20:36.724397 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_authorizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_buckets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17872 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:20:36.720397 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 10:20:36.724397 komminarlabs_influxdb-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-03-13 10:20:36.000000 komminarlabs_influxdb-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9282 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20570 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/bucket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7155 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9224 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17872 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:46:58.423710 komminarlabs_influxdb-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-03 16:46:58.000000 komminarlabs_influxdb-1.0.2/setup.py
```

### Comparing `komminarlabs_influxdb-1.0.1/PKG-INFO` & `komminarlabs_influxdb-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komminarlabs_influxdb
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Pulumi package for creating and managing InfluxDB resources.
 Home-page: https://www.influxdata.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/komminarlabs/pulumi-influxdb
 Keywords: pulumi influxdb category/database
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `komminarlabs_influxdb-1.0.1/README.md` & `komminarlabs_influxdb-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/__init__.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/__init__.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/_inputs.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_inputs.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/_utilities.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/_utilities.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/authorization.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/authorization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/bucket.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/bucket.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/config/vars.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/config/vars.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_authorization.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_authorizations.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_authorizations.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_bucket.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_bucket.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_buckets.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_buckets.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_organization.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/get_organizations.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/get_organizations.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/organization.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/organization.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/outputs.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/outputs.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb/provider.py` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb/provider.py`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/PKG-INFO` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komminarlabs-influxdb
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Pulumi package for creating and managing InfluxDB resources.
 Home-page: https://www.influxdata.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/komminarlabs/pulumi-influxdb
 Keywords: pulumi influxdb category/database
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `komminarlabs_influxdb-1.0.1/komminarlabs_influxdb.egg-info/SOURCES.txt` & `komminarlabs_influxdb-1.0.2/komminarlabs_influxdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `komminarlabs_influxdb-1.0.1/setup.py` & `komminarlabs_influxdb-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import errno
 import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.1"
+VERSION = "1.0.2"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "influxdb Pulumi Package - Development Version"
```

