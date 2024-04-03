# Comparing `tmp/taskara-0.1.3.tar.gz` & `tmp/taskara-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.3.tar", max compression
+gzip compressed data, was "taskara-0.1.4.tar", max compression
```

## Comparing `taskara-0.1.3.tar` & `taskara-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.3/LICENSE
--rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.3/README.md
--rw-r--r--   0        0        0      392 2024-04-03 02:47:06.328910 taskara-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.3/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.3/taskara/db/conn.py
--rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.3/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.3/taskara/env.py
--rw-r--r--   0        0        0     1513 2024-04-03 02:25:02.082624 taskara-0.1.3/taskara/models.py
--rw-r--r--   0        0        0    18840 2024-04-03 02:34:10.525445 taskara-0.1.3/taskara/task.py
--rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.4/LICENSE
+-rw-r--r--   0        0        0      753 2024-04-03 02:46:31.154602 taskara-0.1.4/README.md
+-rw-r--r--   0        0        0      392 2024-04-03 04:00:12.289320 taskara-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.4/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.4/taskara/db/conn.py
+-rw-r--r--   0        0        0     1352 2024-04-03 02:34:26.057465 taskara-0.1.4/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.4/taskara/env.py
+-rw-r--r--   0        0        0     1513 2024-04-03 02:25:02.082624 taskara-0.1.4/taskara/models.py
+-rw-r--r--   0        0        0    18840 2024-04-03 02:34:10.525445 taskara-0.1.4/taskara/task.py
+-rw-r--r--   0        0        0     1324 1970-01-01 00:00:00.000000 taskara-0.1.4/PKG-INFO
```

### Comparing `taskara-0.1.3/LICENSE` & `taskara-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/README.md` & `taskara-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/taskara/db/conn.py` & `taskara-0.1.4/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/taskara/db/models.py` & `taskara-0.1.4/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/taskara/models.py` & `taskara-0.1.4/taskara/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/taskara/task.py` & `taskara-0.1.4/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.3/PKG-INFO` & `taskara-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.3
+Version: 0.1.4
 Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

