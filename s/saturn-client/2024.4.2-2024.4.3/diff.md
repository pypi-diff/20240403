# Comparing `tmp/saturn-client-2024.4.2.tar.gz` & `tmp/saturn-client-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saturn-client-2024.4.2.tar", last modified: Mon Apr  1 21:07:19 2024, max compression
+gzip compressed data, was "saturn-client-2024.4.3.tar", last modified: Wed Apr  3 20:50:26 2024, max compression
```

## Comparing `saturn-client-2024.4.2.tar` & `saturn-client-2024.4.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/saturn_client/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/saturn_client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/saturn_client/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15882 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/saturn_client/tar_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/saturn_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 21:07:19.000000 saturn-client-2024.4.2/saturn_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-01 21:07:19.723282 saturn-client-2024.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-04-01 21:07:17.000000 saturn-client-2024.4.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/saturn_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/saturn_client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/saturn_client/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15882 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8740 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/saturn_client/tar_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/saturn_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 20:50:26.000000 saturn-client-2024.4.3/saturn_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 20:50:26.518405 saturn-client-2024.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68621 2024-04-03 20:50:24.000000 saturn-client-2024.4.3/versioneer.py
```

### Comparing `saturn-client-2024.4.2/LICENSE` & `saturn-client-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/PKG-INFO` & `saturn-client-2024.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-client
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: Python library for interacting with Saturn Cloud API
 Home-page: https://saturncloud.io/
 Maintainer: Saturn Cloud Developers
 Maintainer-email: dev@saturncloud.io
 License: BSD-3-Clause
 Project-URL: Documentation, http://docs.saturncloud.io
 Project-URL: Source, https://github.com/saturncloud/saturn-client
@@ -19,10 +19,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: fsspec>=2024.2
+Requires-Dist: saturnfs
+Requires-Dist: ruamel.yaml
+Requires-Dist: cytoolz
 
 # saturn-client
 Python library for interacting with [Saturn Cloud](https://www.saturncloud.io/) API.
```

### Comparing `saturn-client-2024.4.2/saturn_client/cli/commands.py` & `saturn-client-2024.4.3/saturn_client/cli/commands.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/cli/utils.py` & `saturn-client-2024.4.3/saturn_client/cli/utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/core.py` & `saturn-client-2024.4.3/saturn_client/core.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/logs.py` & `saturn-client-2024.4.3/saturn_client/logs.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/run.py` & `saturn-client-2024.4.3/saturn_client/run.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/settings.py` & `saturn-client-2024.4.3/saturn_client/settings.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client/tar_utils.py` & `saturn-client-2024.4.3/saturn_client/tar_utils.py`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/saturn_client.egg-info/PKG-INFO` & `saturn-client-2024.4.3/saturn_client.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saturn-client
-Version: 2024.4.2
+Version: 2024.4.3
 Summary: Python library for interacting with Saturn Cloud API
 Home-page: https://saturncloud.io/
 Maintainer: Saturn Cloud Developers
 Maintainer-email: dev@saturncloud.io
 License: BSD-3-Clause
 Project-URL: Documentation, http://docs.saturncloud.io
 Project-URL: Source, https://github.com/saturncloud/saturn-client
@@ -19,10 +19,13 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: fsspec>=2024.2
+Requires-Dist: saturnfs
+Requires-Dist: ruamel.yaml
+Requires-Dist: cytoolz
 
 # saturn-client
 Python library for interacting with [Saturn Cloud](https://www.saturncloud.io/) API.
```

### Comparing `saturn-client-2024.4.2/saturn_client.egg-info/SOURCES.txt` & `saturn-client-2024.4.3/saturn_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saturn-client-2024.4.2/setup.py` & `saturn-client-2024.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 import versioneer
 
-install_requires = ["requests", "fsspec>=2024.2"]
+install_requires = ["requests", "fsspec>=2024.2", "saturnfs", "ruamel.yaml", "cytoolz"]
 
 
 setup(
     name="saturn-client",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     maintainer="Saturn Cloud Developers",
```

### Comparing `saturn-client-2024.4.2/versioneer.py` & `saturn-client-2024.4.3/versioneer.py`

 * *Files identical despite different names*

