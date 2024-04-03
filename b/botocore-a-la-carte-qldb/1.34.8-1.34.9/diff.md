# Comparing `tmp/botocore-a-la-carte-qldb-1.34.8.tar.gz` & `tmp/botocore-a-la-carte-qldb-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-qldb-1.34.8.tar", last modified: Wed Dec 27 01:06:54 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-qldb-1.34.9.tar", last modified: Thu Dec 28 01:06:55 2023, max compression
```

## Comparing `botocore-a-la-carte-qldb-1.34.8.tar` & `botocore-a-la-carte-qldb-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-27 01:06:53.000000 botocore-a-la-carte-qldb-1.34.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2023-12-27 01:06:29.000000 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-27 01:06:29.000000 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-27 01:06:29.000000 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)    74308 2023-12-27 01:06:29.000000 botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-27 01:06:54.000000 botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-27 01:06:54.000000 botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-27 01:06:54.000000 botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-27 01:06:54.000000 botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-27 01:06:54.171345 botocore-a-la-carte-qldb-1.34.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-27 01:06:53.000000 botocore-a-la-carte-qldb-1.34.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.894390 botocore-a-la-carte-qldb-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2023-12-28 01:06:26.000000 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-28 01:06:26.000000 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    74308 2023-12-28 01:06:26.000000 botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:55.890390 botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:55.894390 botocore-a-la-carte-qldb-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-12-28 01:06:55.000000 botocore-a-la-carte-qldb-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-qldb-1.34.8/LICENSE.txt` & `botocore-a-la-carte-qldb-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qldb-1.34.8/PKG-INFO` & `botocore-a-la-carte-qldb-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qldb
-Version: 1.34.8
+Version: 1.34.9
 Summary: qldb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json` & `botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qldb-1.34.8/botocore/data/qldb/2019-01-02/service-2.json` & `botocore-a-la-carte-qldb-1.34.9/botocore/data/qldb/2019-01-02/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-qldb-1.34.8/botocore_a_la_carte_qldb.egg-info/PKG-INFO` & `botocore-a-la-carte-qldb-1.34.9/botocore_a_la_carte_qldb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-qldb
-Version: 1.34.8
+Version: 1.34.9
 Summary: qldb data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-qldb-1.34.8/setup.py` & `botocore-a-la-carte-qldb-1.34.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-qldb',
-    version="1.34.8",
+    version="1.34.9",
     description='qldb data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/qldb/*/*.json'],
```
