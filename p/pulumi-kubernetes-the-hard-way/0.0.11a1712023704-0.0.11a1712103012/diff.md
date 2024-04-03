# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712023704.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.11a1712103012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712023704.tar", last modified: Tue Apr  2 02:10:23 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.11a1712103012.tar", last modified: Wed Apr  3 00:12:51 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704.tar` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.448833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-02 02:10:23.448833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.440833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     2285 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.444833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      318 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      463 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)     4567 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     2843 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.444833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      345 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)      334 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)     8177 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12010 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)     6927 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.444833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      403 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)      942 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     1401 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    18602 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    14904 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4166 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)    15417 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.448833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      369 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     8252 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    10335 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    19738 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    10561 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    11452 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    12663 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:10:23.448833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-02 02:10:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 02:10:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:10:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 02:10:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 02:10:23.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      860 2024-04-02 02:10:17.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 02:10:23.448833 pulumi_kubernetes_the_hard_way-0.0.11a1712023704/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7411 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.855682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     2285 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.855682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      318 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      463 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     4567 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     2843 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.855682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      345 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      334 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     8177 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    21549 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)     6927 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      403 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      942 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     1401 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    18602 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    14904 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4166 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)    15417 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      369 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     8252 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    10335 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    19738 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    10561 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    11452 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    12663 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8045 2024-04-03 00:12:51.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 00:12:51.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:12:51.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 00:12:51.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 00:12:51.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      860 2024-04-03 00:12:39.000000 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:12:51.859682 pulumi_kubernetes_the_hard_way-0.0.11a1712103012/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712023704
+Version: 0.0.11a1712103012
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/README.md` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,312 +4,299 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from .. import tools as _tools
-from ._enums import *
-from .download import Download
 import pulumi_command
 
-__all__ = ['EtcdInstallArgs', 'EtcdInstall']
+__all__ = ['TarArgs', 'Tar']
 
 @pulumi.input_type
-class EtcdInstallArgs:
+class TarArgs:
     def __init__(__self__, *,
+                 archive: pulumi.Input[str],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None):
-        """
-        The set of arguments for constructing a EtcdInstall resource.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The connection details.
-        :param pulumi.Input['Architecture'] architecture: The etcd CPU architecture.
-        :param pulumi.Input[str] download_directory: Temporary directory to download files to. Defaults to `/tmp/<random string>`.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
-        :param pulumi.Input[str] version: The version of etcd to install.
+                 directory: Optional[pulumi.Input[str]] = None,
+                 extract: Optional[pulumi.Input[bool]] = None,
+                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
+                 gzip: Optional[pulumi.Input[bool]] = None,
+                 strip_components: Optional[pulumi.Input[int]] = None):
+        """
+        The set of arguments for constructing a Tar resource.
+        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
+        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system.
+        :param pulumi.Input[str] directory: Corresponds to the --directory option.
+        :param pulumi.Input[bool] extract: Corresponds to the --extract option.
+        :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[bool] gzip: Corresponds to the --gzip option.
+        :param pulumi.Input[int] strip_components: Corresponds to the --strip-components option.
         """
+        pulumi.set(__self__, "archive", archive)
         pulumi.set(__self__, "connection", connection)
-        if architecture is not None:
-            pulumi.set(__self__, "architecture", architecture)
-        if download_directory is not None:
-            pulumi.set(__self__, "download_directory", download_directory)
-        if install_directory is None:
-            install_directory = '/usr/local/bin'
-        if install_directory is not None:
-            pulumi.set(__self__, "install_directory", install_directory)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if extract is not None:
+            pulumi.set(__self__, "extract", extract)
+        if files is not None:
+            pulumi.set(__self__, "files", files)
+        if gzip is not None:
+            pulumi.set(__self__, "gzip", gzip)
+        if strip_components is not None:
+            pulumi.set(__self__, "strip_components", strip_components)
+
+    @property
+    @pulumi.getter
+    def archive(self) -> pulumi.Input[str]:
+        """
+        Corresponds to the [ARCHIVE] argument.
+        """
+        return pulumi.get(self, "archive")
+
+    @archive.setter
+    def archive(self, value: pulumi.Input[str]):
+        pulumi.set(self, "archive", value)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
-        The connection details.
+        Connection details for the remote system.
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def architecture(self) -> Optional[pulumi.Input['Architecture']]:
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        The etcd CPU architecture.
+        Corresponds to the --directory option.
         """
-        return pulumi.get(self, "architecture")
+        return pulumi.get(self, "directory")
 
-    @architecture.setter
-    def architecture(self, value: Optional[pulumi.Input['Architecture']]):
-        pulumi.set(self, "architecture", value)
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="downloadDirectory")
-    def download_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def extract(self) -> Optional[pulumi.Input[bool]]:
         """
-        Temporary directory to download files to. Defaults to `/tmp/<random string>`.
+        Corresponds to the --extract option.
         """
-        return pulumi.get(self, "download_directory")
+        return pulumi.get(self, "extract")
 
-    @download_directory.setter
-    def download_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "download_directory", value)
+    @extract.setter
+    def extract(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "extract", value)
 
     @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def files(self) -> Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]]:
         """
-        Directory to install the `etcd` and `etcdctl` binaries.
+        Corresponds to the [FILE] argument.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "files")
 
-    @install_directory.setter
-    def install_directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "install_directory", value)
+    @files.setter
+    def files(self, value: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]]):
+        pulumi.set(self, "files", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[str]]:
+    def gzip(self) -> Optional[pulumi.Input[bool]]:
         """
-        The version of etcd to install.
+        Corresponds to the --gzip option.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "gzip")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "version", value)
+    @gzip.setter
+    def gzip(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "gzip", value)
+
+    @property
+    @pulumi.getter(name="stripComponents")
+    def strip_components(self) -> Optional[pulumi.Input[int]]:
+        """
+        Corresponds to the --strip-components option.
+        """
+        return pulumi.get(self, "strip_components")
+
+    @strip_components.setter
+    def strip_components(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "strip_components", value)
 
 
-class EtcdInstall(pulumi.ComponentResource):
+class Tar(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 extract: Optional[pulumi.Input[bool]] = None,
+                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
+                 gzip: Optional[pulumi.Input[bool]] = None,
+                 strip_components: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         """
-        Represents an etcd binary on a remote system.
+        Abstracion over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input['Architecture'] architecture: The etcd CPU architecture.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The connection details.
-        :param pulumi.Input[str] download_directory: Temporary directory to download files to. Defaults to `/tmp/<random string>`.
-        :param pulumi.Input[str] install_directory: Directory to install the `etcd` and `etcdctl` binaries.
-        :param pulumi.Input[str] version: The version of etcd to install.
+        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
+        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system.
+        :param pulumi.Input[str] directory: Corresponds to the --directory option.
+        :param pulumi.Input[bool] extract: Corresponds to the --extract option.
+        :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[bool] gzip: Corresponds to the --gzip option.
+        :param pulumi.Input[int] strip_components: Corresponds to the --strip-components option.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: EtcdInstallArgs,
+                 args: TarArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Represents an etcd binary on a remote system.
+        Abstracion over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param EtcdInstallArgs args: The arguments to use to populate this resource's properties.
+        :param TarArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(EtcdInstallArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 architecture: Optional[pulumi.Input['Architecture']] = None,
+                 archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 download_directory: Optional[pulumi.Input[str]] = None,
-                 install_directory: Optional[pulumi.Input[str]] = None,
-                 version: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 extract: Optional[pulumi.Input[bool]] = None,
+                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
+                 gzip: Optional[pulumi.Input[bool]] = None,
+                 strip_components: Optional[pulumi.Input[int]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = EtcdInstallArgs.__new__(EtcdInstallArgs)
+            __props__ = TarArgs.__new__(TarArgs)
 
-            __props__.__dict__["architecture"] = architecture
+            if archive is None and not opts.urn:
+                raise TypeError("Missing required property 'archive'")
+            __props__.__dict__["archive"] = archive
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["download_directory"] = download_directory
-            if install_directory is None:
-                install_directory = '/usr/local/bin'
-            __props__.__dict__["install_directory"] = install_directory
-            __props__.__dict__["version"] = version
-            __props__.__dict__["archive_name"] = None
-            __props__.__dict__["download"] = None
-            __props__.__dict__["download_mkdir"] = None
-            __props__.__dict__["etcd_path"] = None
-            __props__.__dict__["etcdctl_path"] = None
-            __props__.__dict__["install_mkdir"] = None
-            __props__.__dict__["mv_etcd"] = None
-            __props__.__dict__["mv_etcdctl"] = None
-            __props__.__dict__["name"] = None
-            __props__.__dict__["tar"] = None
-            __props__.__dict__["url"] = None
-        super(EtcdInstall, __self__).__init__(
-            'kubernetes-the-hard-way:remote:EtcdInstall',
+            __props__.__dict__["directory"] = directory
+            __props__.__dict__["extract"] = extract
+            __props__.__dict__["files"] = files
+            __props__.__dict__["gzip"] = gzip
+            __props__.__dict__["strip_components"] = strip_components
+            __props__.__dict__["command"] = None
+            __props__.__dict__["stderr"] = None
+            __props__.__dict__["stdin"] = None
+            __props__.__dict__["stdout"] = None
+        super(Tar, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tar',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def architecture(self) -> pulumi.Output['Architecture']:
+    def archive(self) -> pulumi.Output[str]:
         """
-        The etcd CPU architecture.
+        Corresponds to the [ARCHIVE] argument.
         """
-        return pulumi.get(self, "architecture")
-
-    @property
-    @pulumi.getter(name="archiveName")
-    def archive_name(self) -> pulumi.Output[str]:
-        """
-        The name of the etcd release archive.
-        """
-        return pulumi.get(self, "archive_name")
+        return pulumi.get(self, "archive")
 
     @property
     @pulumi.getter
-    def download(self) -> pulumi.Output['Download']:
-        """
-        The etcd download operation.
-        """
-        return pulumi.get(self, "download")
-
-    @property
-    @pulumi.getter(name="downloadDirectory")
-    def download_directory(self) -> pulumi.Output[str]:
-        """
-        The directory where the etcd binary was downloaded to.
-        """
-        return pulumi.get(self, "download_directory")
-
-    @property
-    @pulumi.getter(name="downloadMkdir")
-    def download_mkdir(self) -> pulumi.Output['_tools.Mkdir']:
-        """
-        The operation to create the download directory.
-        """
-        return pulumi.get(self, "download_mkdir")
-
-    @property
-    @pulumi.getter(name="etcdPath")
-    def etcd_path(self) -> pulumi.Output[str]:
+    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
-        The path to the etcd binary on the remote system.
+        Represents the remote `tar` operation.
         """
-        return pulumi.get(self, "etcd_path")
+        return pulumi.get(self, "command")
 
     @property
-    @pulumi.getter(name="etcdctlPath")
-    def etcdctl_path(self) -> pulumi.Output[str]:
-        """
-        The path to the etcdctl binary on the remote system.
-        """
-        return pulumi.get(self, "etcdctl_path")
-
-    @property
-    @pulumi.getter(name="installDirectory")
-    def install_directory(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def directory(self) -> pulumi.Output[Optional[str]]:
         """
-        Directory to install the `etcd` and `etcdctl` binaries.
+        Corresponds to the --directory option.
         """
-        return pulumi.get(self, "install_directory")
+        return pulumi.get(self, "directory")
 
     @property
-    @pulumi.getter(name="installMkdir")
-    def install_mkdir(self) -> pulumi.Output['_tools.Mkdir']:
+    @pulumi.getter
+    def extract(self) -> pulumi.Output[bool]:
         """
-        The operation to create the install directory.
+        Corresponds to the --extract option.
         """
-        return pulumi.get(self, "install_mkdir")
+        return pulumi.get(self, "extract")
 
     @property
-    @pulumi.getter(name="mvEtcd")
-    def mv_etcd(self) -> pulumi.Output['_tools.Mv']:
+    @pulumi.getter
+    def files(self) -> pulumi.Output[Sequence[str]]:
         """
-        The operation to move the etcd binary to the install directory.
+        Corresponds to the [FILE] argument.
         """
-        return pulumi.get(self, "mv_etcd")
+        return pulumi.get(self, "files")
 
     @property
-    @pulumi.getter(name="mvEtcdctl")
-    def mv_etcdctl(self) -> pulumi.Output['_tools.Mv']:
+    @pulumi.getter
+    def gzip(self) -> pulumi.Output[Optional[bool]]:
         """
-        The operation to move the etcdctl binary to the install directory.
+        Corresponds to the --gzip option.
         """
-        return pulumi.get(self, "mv_etcdctl")
+        return pulumi.get(self, "gzip")
 
     @property
     @pulumi.getter
-    def name(self) -> pulumi.Output[str]:
+    def stderr(self) -> pulumi.Output[str]:
         """
-        The name of the resource.
+        The process' stderr.
         """
-        return pulumi.get(self, "name")
+        return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
-    def tar(self) -> pulumi.Output['_tools.Tar']:
+    def stdin(self) -> pulumi.Output[Optional[str]]:
         """
-        The tar operation.
+        The process' stdin.
         """
-        return pulumi.get(self, "tar")
+        return pulumi.get(self, "stdin")
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Output[str]:
+    def stdout(self) -> pulumi.Output[str]:
         """
-        The url used to download etcd.
+        The process' stdout.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "stdout")
 
     @property
-    @pulumi.getter
-    def version(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="stripComponents")
+    def strip_components(self) -> pulumi.Output[Optional[int]]:
         """
-        The version of etcd downloaded.
+        Corresponds to the --strip-components option.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "strip_components")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,60 +6,52 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 import pulumi_command
 
-__all__ = ['TarArgs', 'Tar']
+__all__ = ['WgetArgs', 'Wget']
 
 @pulumi.input_type
-class TarArgs:
+class WgetArgs:
     def __init__(__self__, *,
-                 archive: pulumi.Input[str],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 directory: Optional[pulumi.Input[str]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None):
+                 url: pulumi.Input[str],
+                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 https_only: Optional[pulumi.Input[bool]] = None,
+                 no_verbose: Optional[pulumi.Input[bool]] = None,
+                 output_document: Optional[pulumi.Input[str]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 timestamping: Optional[pulumi.Input[bool]] = None):
         """
-        The set of arguments for constructing a Tar resource.
-        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
+        The set of arguments for constructing a Wget resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system.
-        :param pulumi.Input[str] directory: Corresponds to the --directory option.
-        :param pulumi.Input[bool] extract: Corresponds to the --extract option.
-        :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] gzip: Corresponds to the --gzip option.
-        :param pulumi.Input[int] strip_components: Corresponds to the --strip-components option.
+        :param pulumi.Input[str] url: Corresponse to the [URL] argument.
+        :param pulumi.Input[str] directory_prefix: Corresponds to the --directory-prefix option.
+        :param pulumi.Input[bool] https_only: Corresponds to the --https-only option.
+        :param pulumi.Input[bool] no_verbose: Corresponds t- the --no-verbose option.
+        :param pulumi.Input[str] output_document: Corresponds to the --output-document option.
+        :param pulumi.Input[bool] quiet: Corresponds to the --quiet option.
+        :param pulumi.Input[bool] timestamping: Corresponds to the --timestamping option.
         """
-        pulumi.set(__self__, "archive", archive)
         pulumi.set(__self__, "connection", connection)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
-        if extract is not None:
-            pulumi.set(__self__, "extract", extract)
-        if files is not None:
-            pulumi.set(__self__, "files", files)
-        if gzip is not None:
-            pulumi.set(__self__, "gzip", gzip)
-        if strip_components is not None:
-            pulumi.set(__self__, "strip_components", strip_components)
-
-    @property
-    @pulumi.getter
-    def archive(self) -> pulumi.Input[str]:
-        """
-        Corresponds to the [ARCHIVE] argument.
-        """
-        return pulumi.get(self, "archive")
-
-    @archive.setter
-    def archive(self, value: pulumi.Input[str]):
-        pulumi.set(self, "archive", value)
+        pulumi.set(__self__, "url", url)
+        if directory_prefix is not None:
+            pulumi.set(__self__, "directory_prefix", directory_prefix)
+        if https_only is not None:
+            pulumi.set(__self__, "https_only", https_only)
+        if no_verbose is not None:
+            pulumi.set(__self__, "no_verbose", no_verbose)
+        if output_document is not None:
+            pulumi.set(__self__, "output_document", output_document)
+        if quiet is not None:
+            pulumi.set(__self__, "quiet", quiet)
+        if timestamping is not None:
+            pulumi.set(__self__, "timestamping", timestamping)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system.
         """
@@ -67,210 +59,238 @@
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[str]]:
+    def url(self) -> pulumi.Input[str]:
         """
-        Corresponds to the --directory option.
+        Corresponse to the [URL] argument.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "url")
 
-    @directory.setter
-    def directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "directory", value)
+    @url.setter
+    def url(self, value: pulumi.Input[str]):
+        pulumi.set(self, "url", value)
 
     @property
-    @pulumi.getter
-    def extract(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter(name="directoryPrefix")
+    def directory_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        Corresponds to the --extract option.
+        Corresponds to the --directory-prefix option.
         """
-        return pulumi.get(self, "extract")
+        return pulumi.get(self, "directory_prefix")
 
-    @extract.setter
-    def extract(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "extract", value)
+    @directory_prefix.setter
+    def directory_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory_prefix", value)
 
     @property
-    @pulumi.getter
-    def files(self) -> Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]]:
+    @pulumi.getter(name="httpsOnly")
+    def https_only(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Corresponds to the --https-only option.
+        """
+        return pulumi.get(self, "https_only")
+
+    @https_only.setter
+    def https_only(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "https_only", value)
+
+    @property
+    @pulumi.getter(name="noVerbose")
+    def no_verbose(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Corresponds t- the --no-verbose option.
+        """
+        return pulumi.get(self, "no_verbose")
+
+    @no_verbose.setter
+    def no_verbose(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_verbose", value)
+
+    @property
+    @pulumi.getter(name="outputDocument")
+    def output_document(self) -> Optional[pulumi.Input[str]]:
         """
-        Corresponds to the [FILE] argument.
+        Corresponds to the --output-document option.
         """
-        return pulumi.get(self, "files")
+        return pulumi.get(self, "output_document")
 
-    @files.setter
-    def files(self, value: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]]):
-        pulumi.set(self, "files", value)
+    @output_document.setter
+    def output_document(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "output_document", value)
 
     @property
     @pulumi.getter
-    def gzip(self) -> Optional[pulumi.Input[bool]]:
+    def quiet(self) -> Optional[pulumi.Input[bool]]:
         """
-        Corresponds to the --gzip option.
+        Corresponds to the --quiet option.
         """
-        return pulumi.get(self, "gzip")
+        return pulumi.get(self, "quiet")
 
-    @gzip.setter
-    def gzip(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "gzip", value)
+    @quiet.setter
+    def quiet(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "quiet", value)
 
     @property
-    @pulumi.getter(name="stripComponents")
-    def strip_components(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def timestamping(self) -> Optional[pulumi.Input[bool]]:
         """
-        Corresponds to the --strip-components option.
+        Corresponds to the --timestamping option.
         """
-        return pulumi.get(self, "strip_components")
+        return pulumi.get(self, "timestamping")
 
-    @strip_components.setter
-    def strip_components(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "strip_components", value)
+    @timestamping.setter
+    def timestamping(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "timestamping", value)
 
 
-class Tar(pulumi.ComponentResource):
+class Wget(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None,
+                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 https_only: Optional[pulumi.Input[bool]] = None,
+                 no_verbose: Optional[pulumi.Input[bool]] = None,
+                 output_document: Optional[pulumi.Input[str]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 timestamping: Optional[pulumi.Input[bool]] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        Abstracion over the `tar` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system.
-        :param pulumi.Input[str] directory: Corresponds to the --directory option.
-        :param pulumi.Input[bool] extract: Corresponds to the --extract option.
-        :param pulumi.Input[Union[Sequence[pulumi.Input[str]], str]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] gzip: Corresponds to the --gzip option.
-        :param pulumi.Input[int] strip_components: Corresponds to the --strip-components option.
+        :param pulumi.Input[str] directory_prefix: Corresponds to the --directory-prefix option.
+        :param pulumi.Input[bool] https_only: Corresponds to the --https-only option.
+        :param pulumi.Input[bool] no_verbose: Corresponds t- the --no-verbose option.
+        :param pulumi.Input[str] output_document: Corresponds to the --output-document option.
+        :param pulumi.Input[bool] quiet: Corresponds to the --quiet option.
+        :param pulumi.Input[bool] timestamping: Corresponds to the --timestamping option.
+        :param pulumi.Input[str] url: Corresponse to the [URL] argument.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TarArgs,
+                 args: WgetArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstracion over the `tar` utility on a remote system.
+        Abstraction over the `wget` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TarArgs args: The arguments to use to populate this resource's properties.
+        :param WgetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 archive: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[Sequence[pulumi.Input[str]], str]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None,
+                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 https_only: Optional[pulumi.Input[bool]] = None,
+                 no_verbose: Optional[pulumi.Input[bool]] = None,
+                 output_document: Optional[pulumi.Input[str]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 timestamping: Optional[pulumi.Input[bool]] = None,
+                 url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TarArgs.__new__(TarArgs)
+            __props__ = WgetArgs.__new__(WgetArgs)
 
-            if archive is None and not opts.urn:
-                raise TypeError("Missing required property 'archive'")
-            __props__.__dict__["archive"] = archive
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["directory"] = directory
-            __props__.__dict__["extract"] = extract
-            __props__.__dict__["files"] = files
-            __props__.__dict__["gzip"] = gzip
-            __props__.__dict__["strip_components"] = strip_components
+            __props__.__dict__["directory_prefix"] = directory_prefix
+            __props__.__dict__["https_only"] = https_only
+            __props__.__dict__["no_verbose"] = no_verbose
+            __props__.__dict__["output_document"] = output_document
+            __props__.__dict__["quiet"] = quiet
+            __props__.__dict__["timestamping"] = timestamping
+            if url is None and not opts.urn:
+                raise TypeError("Missing required property 'url'")
+            __props__.__dict__["url"] = url
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdin"] = None
             __props__.__dict__["stdout"] = None
-        super(Tar, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tar',
+        super(Wget, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Wget',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter
-    def archive(self) -> pulumi.Output[str]:
+    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
-        Corresponds to the [ARCHIVE] argument.
+        Represents the remote `tar` operation.
         """
-        return pulumi.get(self, "archive")
+        return pulumi.get(self, "command")
 
     @property
-    @pulumi.getter
-    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
+    @pulumi.getter(name="directoryPrefix")
+    def directory_prefix(self) -> pulumi.Output[Optional[str]]:
         """
-        Represents the remote `tar` operation.
+        Corresponds to the --directory-prefix option.
         """
-        return pulumi.get(self, "command")
+        return pulumi.get(self, "directory_prefix")
 
     @property
-    @pulumi.getter
-    def directory(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="httpsOnly")
+    def https_only(self) -> pulumi.Output[bool]:
         """
-        Corresponds to the --directory option.
+        Corresponds to the --https-only option.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "https_only")
 
     @property
-    @pulumi.getter
-    def extract(self) -> pulumi.Output[bool]:
+    @pulumi.getter(name="noVerbose")
+    def no_verbose(self) -> pulumi.Output[Optional[bool]]:
         """
-        Corresponds to the --extract option.
+        Corresponds to the --no-verbose option.
         """
-        return pulumi.get(self, "extract")
+        return pulumi.get(self, "no_verbose")
 
     @property
-    @pulumi.getter
-    def files(self) -> pulumi.Output[Sequence[str]]:
+    @pulumi.getter(name="outputDocument")
+    def output_document(self) -> pulumi.Output[Optional[str]]:
         """
-        Corresponds to the [FILE] argument.
+        Corresponds to the --output-document option.
         """
-        return pulumi.get(self, "files")
+        return pulumi.get(self, "output_document")
 
     @property
     @pulumi.getter
-    def gzip(self) -> pulumi.Output[Optional[bool]]:
+    def quiet(self) -> pulumi.Output[bool]:
         """
-        Corresponds to the --gzip option.
+        Corresponds to the --quiet option.
         """
-        return pulumi.get(self, "gzip")
+        return pulumi.get(self, "quiet")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         The process' stderr.
         """
@@ -289,14 +309,22 @@
     def stdout(self) -> pulumi.Output[str]:
         """
         The process' stdout.
         """
         return pulumi.get(self, "stdout")
 
     @property
-    @pulumi.getter(name="stripComponents")
-    def strip_components(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def timestamping(self) -> pulumi.Output[bool]:
+        """
+        Corresponds to the --timestamping option.
+        """
+        return pulumi.get(self, "timestamping")
+
+    @property
+    @pulumi.getter
+    def url(self) -> pulumi.Output[str]:
         """
-        Corresponds to the --strip-components option.
+        Corresponse to the [URL] argument.
         """
-        return pulumi.get(self, "strip_components")
+        return pulumi.get(self, "url")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.11a1712023704
+Version: 0.0.11a1712103012
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.11a1712023704/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.11a1712103012/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-command>=0.9.0,<1.0.0", "pulumi-random>=4.0.0,<5.0.0", "pulumi-tls>=5.0.0,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.11a1712023704"
+  version = "0.0.11a1712103012"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

