# Comparing `tmp/zhmc_prometheus_exporter-1.5.1.tar.gz` & `tmp/zhmc_prometheus_exporter-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhmc_prometheus_exporter-1.5.1.tar", last modified: Sat Feb 24 17:06:31 2024, max compression
+gzip compressed data, was "zhmc_prometheus_exporter-1.5.2.tar", last modified: Wed Apr  3 05:46:21 2024, max compression
```

## Comparing `zhmc_prometheus_exporter-1.5.1.tar` & `zhmc_prometheus_exporter-1.5.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-24 17:06:22.000000 zhmc_prometheus_exporter-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/tests/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)    84453 2024-02-24 17:05:56.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:06:31.404330 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 17:06:31.000000 zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:46:15.000000 zhmc_prometheus_exporter-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18674 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/tests/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.262212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)    84417 2024-04-03 05:45:49.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:46:21.266212 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:46:21.000000 zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/zip-safe
```

### Comparing `zhmc_prometheus_exporter-1.5.1/LICENSE` & `zhmc_prometheus_exporter-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/PKG-INFO` & `zhmc_prometheus_exporter-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc_prometheus_exporter
-Version: 1.5.1
+Version: 1.5.2
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmc_prometheus_exporter-1.5.1/README.rst` & `zhmc_prometheus_exporter-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/requirements.txt` & `zhmc_prometheus_exporter-1.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/setup.py` & `zhmc_prometheus_exporter-1.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/tests/test_all.py` & `zhmc_prometheus_exporter-1.5.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/__init__.py` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/_version.py` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 #: The full version of this package including any development levels, as a
 #: :term:`string`.
 #:
 #: Possible formats for this version string are:
 #:
 #: * "M.N.P.dev1": A not yet released version M.N.P
 #: * "M.N.P": A released version M.N.P
-__version__ = '1.5.1'
+__version__ = '1.5.2'
```

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/hmccreds_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/schemas/metrics_schema.yaml` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/schemas/metrics_schema.yaml`

 * *Files identical despite different names*

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter/zhmc_prometheus_exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1629,17 +1629,17 @@
             self.resources, self.yaml_metric_groups,
             self.yaml_metrics, self.filename_metrics,
             self.extra_labels, self.hmc_version, self.se_versions,
             self.session, self.resource_cache, self.uri2resource))
 
         logprint(logging.DEBUG, None,
                  "Returning family objects")
+
         # Yield all family objects
-        for family_obj in family_objects.values():
-            yield family_obj
+        yield from family_objects.values()
 
         logprint(logging.INFO, None,
                  "Done collecting metrics")
 
 
 # Global variable with the verbosity level from the command line
 VERBOSE_LEVEL = 0
```

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/PKG-INFO` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhmc_prometheus_exporter
-Version: 1.5.1
+Version: 1.5.2
 Summary: IBM Z HMC Prometheus Exporter
 Home-page: https://github.com/zhmcclient/zhmc-prometheus-exporter
 Author: Jakob Naucke
 Author-email: jakob.naucke@ibm.com
 Maintainer: Andreas Maier, Kathir Velusamy
 Maintainer-email: maiera@de.ibm.com, kathir.velu@in.ibm.com
 License: Apache License, Version 2.0
```

### Comparing `zhmc_prometheus_exporter-1.5.1/zhmc_prometheus_exporter.egg-info/SOURCES.txt` & `zhmc_prometheus_exporter-1.5.2/zhmc_prometheus_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

