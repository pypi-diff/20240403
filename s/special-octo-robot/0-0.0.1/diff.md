# Comparing `tmp/special-octo-robot-0.tar.gz` & `tmp/special-octo-robot-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.tar", last modified: Tue Apr  2 13:36:46 2024, max compression
+gzip compressed data, was "special-octo-robot-0.0.1.tar", last modified: Wed Apr  3 14:59:19 2024, max compression
```

## Comparing `special-octo-robot-0.tar` & `special-octo-robot-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-02 13:36:46.592393 special-octo-robot-0/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0/LICENSE
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0/MANIFEST.in
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3378 2024-04-02 13:36:46.592393 special-octo-robot-0/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     2840 2024-03-18 09:00:15.000000 special-octo-robot-0/README.md
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-02 13:36:46.592393 special-octo-robot-0/app/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0/app/__init__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0/app/__main__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-03-17 04:42:07.000000 special-octo-robot-0/app/__version__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5672 2024-04-02 13:03:22.000000 special-octo-robot-0/app/application.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1086 2024-03-18 06:41:14.000000 special-octo-robot-0/app/console.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1949 2024-04-02 13:01:49.000000 special-octo-robot-0/app/database.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5279 2024-04-02 13:03:22.000000 special-octo-robot-0/devcord.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-02 13:36:46.592393 special-octo-robot-0/setup.cfg
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1239 2024-03-18 04:42:23.000000 special-octo-robot-0/setup.py
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-02 13:36:46.592393 special-octo-robot-0/special_octo_robot.egg-info/
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3378 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      404 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/entry_points.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/requires.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-02 13:36:46.000000 special-octo-robot-0/special_octo_robot.egg-info/top_level.txt
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/LICENSE
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/MANIFEST.in
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3382 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     2840 2024-03-18 09:00:15.000000 special-octo-robot-0.0.1/README.md
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/app/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/app/__init__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.1/app/__main__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-03 14:56:33.000000 special-octo-robot-0.0.1/app/__version__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     5661 2024-04-03 13:26:57.000000 special-octo-robot-0.0.1/app/application.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1676 2024-04-03 14:45:02.000000 special-octo-robot-0.0.1/app/console.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1949 2024-04-03 13:30:37.000000 special-octo-robot-0.0.1/app/database.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     5279 2024-04-02 13:03:22.000000 special-octo-robot-0.0.1/devcord.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/setup.cfg
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1053 2024-04-03 14:57:12.000000 special-octo-robot-0.0.1/setup.py
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-03 14:59:19.937482 special-octo-robot-0.0.1/special_octo_robot.egg-info/
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3382 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      404 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/entry_points.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/requires.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-03 14:59:19.000000 special-octo-robot-0.0.1/special_octo_robot.egg-info/top_level.txt
```

### Comparing `special-octo-robot-0/LICENSE` & `special-octo-robot-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0/PKG-INFO` & `special-octo-robot-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0
+Version: 0.0.1
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `special-octo-robot-0/README.md` & `special-octo-robot-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0/app/application.py` & `special-octo-robot-0.0.1/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
     List all the tasks based on the filters.
     """
     order_by = "completed ASC, priority DESC"
     where_clause = ["parent_id ISNULL"]
     if week:
         where_clause.append(
-            "(deadline >= date('now', 'weekday 1') AND deadline < date('now', 'weekday 1', '+7 days'))",
+            "(deadline >= date('now', 'weekday 0', '-7 days') AND deadline < date('now', 'weekday 1'))",
         )
     elif today:
         where_clause.append("(deadline = date('now'))")
     if inprogress or completed or pending:
         clause = []
         if inprogress:
             clause.append("'In Progress'")
@@ -102,15 +102,15 @@
         columns.append("priority")
         values.append(str(priority))
     if today:
         columns.append("deadline")
         values.append("date('now')")
     elif week:
         columns.append("deadline")
-        values.append("date('now', 'weekday 1', '+6 days')")
+        values.append("date('now', 'weekday 0')")
     elif deadline:
         columns.append("deadline")
         values.append(f"'{deadline}'")
     if inprogress:
         columns.append("status")
         values.append("'In Progress'")
     elif completed:
```

### Comparing `special-octo-robot-0/app/database.py` & `special-octo-robot-0.0.1/app/database.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0/devcord.py` & `special-octo-robot-0.0.1/devcord.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0/setup.py` & `special-octo-robot-0.0.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-from pathlib import Path
-
 from setuptools import find_packages
 from setuptools import setup
 
+from app.__version__ import VERSION
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 
 
-def get_version():
-    """Parse package __version__.py to get version."""
-    versionpy = (Path("app") / "__version__.py").read_text()
-    return versionpy.split(".")[1]
-
-
-VERSION = get_version()
-
 setup(
     name="special-octo-robot",
     version=VERSION,
     author="Jahan Chaware",
     author_email="sg550js@gmail.com",
     license="GNU GENERAL PUBLIC LICENSE",
     description="Creating my own version of what a CLI Task manager and To-do-list would look like",
```

### Comparing `special-octo-robot-0/special_octo_robot.egg-info/PKG-INFO` & `special-octo-robot-0.0.1/special_octo_robot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0
+Version: 0.0.1
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

