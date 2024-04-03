# Comparing `tmp/opower-0.4.2.tar.gz` & `tmp/opower-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opower-0.4.2.tar", last modified: Mon Apr  1 06:23:51 2024, max compression
+gzip compressed data, was "opower-0.4.3.tar", last modified: Wed Apr  3 19:15:47 2024, max compression
```

## Comparing `opower-0.4.2.tar` & `opower-0.4.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.542333 opower-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-01 06:23:47.000000 opower-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-01 06:23:51.542333 opower-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-01 06:23:47.000000 opower-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-01 06:23:47.000000 opower-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-01 06:23:51.542333 opower-0.4.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.534333 opower-0.4.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-01 06:23:47.000000 opower-0.4.2/src/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.534333 opower-0.4.2/src/opower/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/opower.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.538334 opower-0.4.2/src/opower/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/aepbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/aepohio.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/aeptexas.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/appalachianpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/atlanticcityelectric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/bge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/coautilities.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/comed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/coned.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/delmarva.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/duquesnelight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/enmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/evergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/exelon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/indianamichiganpower.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/kentuckypower.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/oru.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/peco.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/pepco.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/pge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/portlandgeneral.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/pse.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/psoklahoma.py
--rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/scl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9864 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/smud.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-01 06:23:47.000000 opower-0.4.2/src/opower/utilities/swepco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.538334 opower-0.4.2/src/opower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-01 06:23:51.000000 opower-0.4.2/src/opower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-01 06:23:51.000000 opower-0.4.2/src/opower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 06:23:51.000000 opower-0.4.2/src/opower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-01 06:23:51.000000 opower-0.4.2/src/opower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 06:23:51.000000 opower-0.4.2/src/opower.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 06:23:51.538334 opower-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-01 06:23:47.000000 opower-0.4.2/tests/test_opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 19:15:42.000000 opower-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-03 19:15:47.551893 opower-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-03 19:15:42.000000 opower-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 19:15:42.000000 opower-0.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-03 19:15:47.551893 opower-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.547893 opower-0.4.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-04-03 19:15:42.000000 opower-0.4.3/src/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.547893 opower-0.4.3/src/opower/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21364 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/opower.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/src/opower/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aepbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aepohio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/aeptexas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/appalachianpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/atlanticcityelectric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/bge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/coautilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/comed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4599 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/coned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/delmarva.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/duquesnelight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/enmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/evergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/exelon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/indianamichiganpower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/kentuckypower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/oru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/peco.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pepco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/portlandgeneral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/pse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/psoklahoma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8885 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/scl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/smud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 19:15:42.000000 opower-0.4.3/src/opower/utilities/swepco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/src/opower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 19:15:47.000000 opower-0.4.3/src/opower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:15:47.551893 opower-0.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 19:15:42.000000 opower-0.4.3/tests/test_opower.py
```

### Comparing `opower-0.4.2/LICENSE` & `opower-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/PKG-INFO` & `opower-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.4.2/README.md` & `opower-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/pyproject.toml` & `opower-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "opower"
-version = "0.4.2"
+version = "0.4.3"
 license = {text = "Apache-2.0"}
 authors = [
     { name="tronikos", email="tronikos@gmail.com" },
 ]
 description = "A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `opower-0.4.2/src/demo.py` & `opower-0.4.3/src/demo.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/__init__.py` & `opower-0.4.3/src/opower/__init__.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/opower.py` & `opower-0.4.3/src/opower/opower.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/aepbase.py` & `opower-0.4.3/src/opower/utilities/aepbase.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/atlanticcityelectric.py` & `opower-0.4.3/src/opower/utilities/atlanticcityelectric.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/base.py` & `opower-0.4.3/src/opower/utilities/base.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/bge.py` & `opower-0.4.3/src/opower/utilities/bge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/coautilities.py` & `opower-0.4.3/src/opower/utilities/coautilities.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/comed.py` & `opower-0.4.3/src/opower/utilities/comed.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/coned.py` & `opower-0.4.3/src/opower/utilities/coned.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/delmarva.py` & `opower-0.4.3/src/opower/utilities/delmarva.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/duquesnelight.py` & `opower-0.4.3/src/opower/utilities/duquesnelight.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/enmax.py` & `opower-0.4.3/src/opower/utilities/enmax.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/evergy.py` & `opower-0.4.3/src/opower/utilities/evergy.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/exelon.py` & `opower-0.4.3/src/opower/utilities/exelon.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/helpers.py` & `opower-0.4.3/src/opower/utilities/helpers.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/oru.py` & `opower-0.4.3/src/opower/utilities/oru.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/peco.py` & `opower-0.4.3/src/opower/utilities/peco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/pepco.py` & `opower-0.4.3/src/opower/utilities/pepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/pge.py` & `opower-0.4.3/src/opower/utilities/pge.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/portlandgeneral.py` & `opower-0.4.3/src/opower/utilities/portlandgeneral.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/pse.py` & `opower-0.4.3/src/opower/utilities/pse.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/psoklahoma.py` & `opower-0.4.3/src/opower/utilities/psoklahoma.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/scl.py` & `opower-0.4.3/src/opower/utilities/scl.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower/utilities/smud.py` & `opower-0.4.3/src/opower/utilities/smud.py`

 * *Files 25% similar despite different names*

```diff
@@ -40,21 +40,54 @@
 class SMUDLoginParser(HTMLParser):
     """HTML parser to extract login verification token from SMUD Login page."""
 
     def __init__(self) -> None:
         """Initialize."""
         super().__init__()
         self.verification_token: Optional[str] = None
+        self.ocis_req_sp: Optional[str] = None
+        self.relay_state: Optional[str] = None
 
     def handle_starttag(self, tag: str, attrs: list[tuple[str, Optional[str]]]) -> None:
         """Try to extract the verification token from the login input."""
         if tag == "input" and ("name", "__RequestVerificationToken") in attrs:
             _, token = next(filter(lambda attr: attr[0] == "value", attrs))
-            _LOGGER.debug("SMUD self verify token: %s", token)
+            if token is None:
+                return
+            _LOGGER.debug(
+                "SMUD self verify token: %s...%s (%d characters)",
+                token[0:5],
+                token[-5:],
+                len(token),
+            )
             self.verification_token = token
+        """Try to extract the OCIS_REQ_SP input value from the identity.oraclecloud.com sso HTML"""
+        if tag == "input" and ("name", "OCIS_REQ_SP") in attrs:
+            _, token = next(filter(lambda attr: attr[0] == "value", attrs))
+            if token is None:
+                return
+            _LOGGER.debug(
+                "OCIS_REQ_SP self verify token: %s...%s (%d characters)",
+                token[0:5],
+                token[-5:],
+                len(token),
+            )
+            self.ocis_req_sp = token
+        """Try to extract the RelayState input value from the smud.okta.com HTML"""
+        if tag == "input" and ("name", "RelayState") in attrs:
+            _, token = next(filter(lambda attr: attr[0] == "value", attrs))
+            if token is None:
+                return
+            _LOGGER.debug(
+                "RelayState value: %s...%s (%d characters)",
+                token[0:5],
+                token[-5:],
+                len(token),
+            )
+            self.relay_state = token
 
 
 class SMUDOktaResponseSamlResponseValueParser(HTMLParser):
     """HTML parser to extract SAMLResponse token from OKTA response for Opower SSO."""
 
     # <input name="SAMLResponse" type="hidden" value="..."/>
     def handle_starttag(self, tag: str, attrs: list[tuple[str, Optional[str]]]) -> None:
@@ -100,14 +133,16 @@
                 async with session.get(
                     "https://smud.opower.com/ei/edge/apis/multi-account-v1/cws/smud/customers",
                     headers={"User-Agent": USER_AGENT},
                     raise_for_status=True,
                 ):
                     return
             except ClientResponseError:
+                _LOGGER.debug("Failed to login to SMUD with existing cookies")
+                session.cookie_jar.clear()
                 pass
 
         smud_login_page_url = "https://myaccount.smud.org/"
 
         _LOGGER.debug("Fetching SMUD login page: %s", smud_login_page_url)
 
         myaccount_response = await session.get(
@@ -184,42 +219,109 @@
             "Parsed SAMLResponse: %s...%s (%d characters)",
             saml_response[0:5],
             saml_response[-5:],
             len(saml_response),
         )
 
         # This step is done in the web browser but doesn't seem to matter here.
-        #
-        # smud_ssotransition_url = "https://myaccount.smud.org/signin/ssotransition"
-        #
-        # _LOGGER.debug("Fetching SMUD ssotransition page: %s", smud_ssotransition_url)
-        # smud_ssotransition_response = await session.get(
-        #     smud_ssotransition_url,
-        #     headers={"User-Agent": USER_AGENT},
-        #     raise_for_status=True,
-        # )
-        #
-        # SMUD.print_redirects_cookies_response(smud_ssotransition_response, session)
+        smud_ssotransition_url = "https://myaccount.smud.org/signin/ssotransition"
+
+        _LOGGER.debug("Fetching SMUD ssotransition page: %s", smud_ssotransition_url)
+        smud_ssotransition_response = await session.get(
+            smud_ssotransition_url,
+            headers={"User-Agent": USER_AGENT},
+            raise_for_status=True,
+        )
 
-        opower_sso_url = "https://sso.opower.com/sp/ACS.saml2"
+        await SMUD.log_response(smud_ssotransition_response, session)
+
+        # This is the action of the #appForm form in the smud_okta_response HTML.
+        opower_sso_url = "https://idcs-8d184356671642c58ea38b42e6420ed2.identity.oraclecloud.com/fed/v1/sp/sso"
 
         _LOGGER.debug("POSTing opower sso page with SAMLResponse: %s", opower_sso_url)
 
         opower_sso_response = await session.post(
             opower_sso_url,
             data={
                 "SAMLResponse": saml_response,
                 "RelayState": "https://smud.opower.com/ei/app/myEnergyUse",
             },
             headers={"User-Agent": USER_AGENT},
             raise_for_status=True,
+            allow_redirects=True,
         )
-
         await SMUD.log_response(opower_sso_response, session)
 
+        login_parser.feed(await opower_sso_response.text())
+        ocis_req_sp = login_parser.ocis_req_sp
+
+        identity_oraclecloud_login_url = "https://idcs-8d184356671642c58ea38b42e6420ed2.identity.oraclecloud.com/sso/v1/user/login"
+
+        _LOGGER.debug(
+            "POSTing opower sso login page with OCIS_REQ_SP: %s",
+            identity_oraclecloud_login_url,
+        )
+
+        identity_oraclecloud_login_response = await session.post(
+            identity_oraclecloud_login_url,
+            data={
+                "OCIS_REQ_SP": ocis_req_sp,
+            },
+            headers={"User-Agent": USER_AGENT},
+            raise_for_status=True,
+            allow_redirects=True,
+            max_redirects=10,
+        )
+
+        await SMUD.log_response(identity_oraclecloud_login_response, session)
+
+        okta_saml_request_url = identity_oraclecloud_login_response.real_url
+
+        _LOGGER.debug(
+            "Fetching okta saml page with SAMLRequest, RelayState: %s",
+            okta_saml_request_url,
+        )
+
+        okta_saml_request_response = await session.get(
+            okta_saml_request_url,
+            headers={"User-Agent": USER_AGENT},
+            raise_for_status=True,
+        )
+
+        await SMUD.log_response(okta_saml_request_response, session)
+
+        parser2 = SMUDOktaResponseSamlResponseValueParser()
+        parser2.feed(await okta_saml_request_response.text())
+        saml_response = parser2.saml_response
+        assert saml_response
+
+        login_parser.feed(await okta_saml_request_response.text())
+        relay_state = login_parser.relay_state
+
+        opower_sso_acs_url = "https://sso.opower.com/sp/ACS.saml2"
+
+        _LOGGER.debug(
+            "POSTing opower ACS sso page with SAMLResponse: %s", opower_sso_acs_url
+        )
+
+        opower_sso_acs_response = await session.post(
+            opower_sso_acs_url,
+            data={
+                "SAMLResponse": saml_response,
+                "RelayState": relay_state,
+            },
+            headers={"User-Agent": USER_AGENT},
+            raise_for_status=True,
+            allow_redirects=True,
+        )
+
+        await SMUD.log_response(opower_sso_acs_response, session)
+
+        _LOGGER.debug("End of SMUD login process")
+
         return
 
     @classmethod
     def get_okta_url_from_response_redirect(
         cls, energyusage_response: ClientResponse
     ) -> str:
         """Get the OKTA URL to open next from the last redirect of the previous response."""
```

### Comparing `opower-0.4.2/src/opower/utilities/swepco.py` & `opower-0.4.3/src/opower/utilities/swepco.py`

 * *Files identical despite different names*

### Comparing `opower-0.4.2/src/opower.egg-info/PKG-INFO` & `opower-0.4.3/src/opower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opower
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Python library for getting historical and forecasted usage/cost from utilities that use opower.com such as PG&E
 Author-email: tronikos <tronikos@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/tronikos/opower
 Project-URL: Bug Tracker, https://github.com/tronikos/opower/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `opower-0.4.2/src/opower.egg-info/SOURCES.txt` & `opower-0.4.3/src/opower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

