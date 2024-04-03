# Comparing `tmp/cronken-0.1.6.tar.gz` & `tmp/cronken-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronken-0.1.6.tar", max compression
+gzip compressed data, was "cronken-0.1.7.tar", max compression
```

## Comparing `cronken-0.1.6.tar` & `cronken-0.1.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2023-09-11 22:56:01.438050 cronken-0.1.6/LICENSE
--rw-r--r--   0        0        0     1075 2023-09-29 22:54:42.604867 cronken-0.1.6/README.md
--rw-r--r--   0        0        0       52 2023-09-30 03:24:14.205325 cronken-0.1.6/cronken/__init__.py
--rw-r--r--   0        0        0    26984 2023-09-29 21:54:03.146524 cronken-0.1.6/cronken/cronken.py
--rw-r--r--   0        0        0      415 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/instance_heartbeat.lua
--rw-r--r--   0        0        0      536 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/instance_reap.lua
--rw-r--r--   0        0        0     2704 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/run_finalize.lua
--rw-r--r--   0        0        0     1295 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/run_get_expired.lua
--rw-r--r--   0        0        0      349 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/run_heartbeat.lua
--rw-r--r--   0        0        0      692 2023-08-09 23:48:24.741638 cronken-0.1.6/cronken/run_init.lua
--rw-r--r--   0        0        0      353 2023-09-30 03:24:32.877823 cronken-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1687 1970-01-01 00:00:00.000000 cronken-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-09-11 22:56:01.438050 cronken-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1167 2023-09-30 03:45:43.174609 cronken-0.1.7/README.md
+-rw-r--r--   0        0        0       52 2023-09-30 03:46:04.641667 cronken-0.1.7/cronken/__init__.py
+-rw-r--r--   0        0        0    26984 2023-09-29 21:54:03.146524 cronken-0.1.7/cronken/cronken.py
+-rw-r--r--   0        0        0      415 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/instance_heartbeat.lua
+-rw-r--r--   0        0        0      536 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/instance_reap.lua
+-rw-r--r--   0        0        0     2704 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/run_finalize.lua
+-rw-r--r--   0        0        0     1295 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/run_get_expired.lua
+-rw-r--r--   0        0        0      349 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/run_heartbeat.lua
+-rw-r--r--   0        0        0      692 2023-08-09 23:48:24.741638 cronken-0.1.7/cronken/run_init.lua
+-rw-r--r--   0        0        0      353 2023-09-30 03:45:53.286158 cronken-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 cronken-0.1.7/PKG-INFO
```

### Comparing `cronken-0.1.6/LICENSE` & `cronken-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/README.md` & `cronken-0.1.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Cronken
 [![GitHub license](https://img.shields.io/github/license/Populi/cronken.svg)](https://github.com/Populi/cronken/blob/master/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/cronken)](https://pypi.org/project/cronken/)
 
 ![Cronken logo](cronken-logo.png)
 
 ## What is Cronken?
 Cronken is a Redis-backed distributed cron system which allows running cronjobs across a set of servers without
 risking double-running them on multiple boxes at once.  To facilitate this, it uses Redis locks to ensure that
 only one server at a time runs any particular job.  It also uses Redis for all of its input and output,
```

### Comparing `cronken-0.1.6/cronken/cronken.py` & `cronken-0.1.7/cronken/cronken.py`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/cronken/instance_reap.lua` & `cronken-0.1.7/cronken/instance_reap.lua`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/cronken/run_finalize.lua` & `cronken-0.1.7/cronken/run_finalize.lua`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/cronken/run_get_expired.lua` & `cronken-0.1.7/cronken/run_get_expired.lua`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/cronken/run_init.lua` & `cronken-0.1.7/cronken/run_init.lua`

 * *Files identical despite different names*

### Comparing `cronken-0.1.6/PKG-INFO` & `cronken-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronken
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Home-page: https://github.com/populi/cronken
 Author: Clint Olson
 Author-email: clint@populi.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +14,15 @@
 Requires-Dist: apscheduler (<4.0.0)
 Requires-Dist: coredis (>=4.14.0,<5.0.0)
 Project-URL: Repository, https://github.com/populi/cronken
 Description-Content-Type: text/markdown
 
 # Cronken
 [![GitHub license](https://img.shields.io/github/license/Populi/cronken.svg)](https://github.com/Populi/cronken/blob/master/LICENSE)
+[![PyPI version](https://img.shields.io/pypi/v/cronken)](https://pypi.org/project/cronken/)
 
 ![Cronken logo](cronken-logo.png)
 
 ## What is Cronken?
 Cronken is a Redis-backed distributed cron system which allows running cronjobs across a set of servers without
 risking double-running them on multiple boxes at once.  To facilitate this, it uses Redis locks to ensure that
 only one server at a time runs any particular job.  It also uses Redis for all of its input and output,
```

