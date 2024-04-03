# Comparing `tmp/taskara-0.1.1.tar.gz` & `tmp/taskara-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskara-0.1.1.tar", max compression
+gzip compressed data, was "taskara-0.1.2.tar", max compression
```

## Comparing `taskara-0.1.1.tar` & `taskara-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.1/LICENSE
--rw-r--r--   0        0        0      221 2024-04-02 20:40:49.884528 taskara-0.1.1/README.md
--rw-r--r--   0        0        0      392 2024-04-02 20:42:07.253730 taskara-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.1/taskara/__init__.py
--rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.1/taskara/db/conn.py
--rw-r--r--   0        0        0     1449 2024-04-02 20:36:27.320183 taskara-0.1.1/taskara/db/models.py
--rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.1/taskara/env.py
--rw-r--r--   0        0        0     1457 2024-04-02 20:34:08.999667 taskara-0.1.1/taskara/models.py
--rw-r--r--   0        0        0    20304 2024-04-02 20:38:39.122416 taskara-0.1.1/taskara/task.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 taskara-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-22 17:15:53.679144 taskara-0.1.2/LICENSE
+-rw-r--r--   0        0        0      221 2024-04-02 20:40:49.884528 taskara-0.1.2/README.md
+-rw-r--r--   0        0        0      392 2024-04-02 20:58:34.131602 taskara-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-04-02 20:42:34.072763 taskara-0.1.2/taskara/__init__.py
+-rw-r--r--   0        0        0     2001 2024-04-02 20:34:43.380692 taskara-0.1.2/taskara/db/conn.py
+-rw-r--r--   0        0        0     1449 2024-04-02 20:36:27.320183 taskara-0.1.2/taskara/db/models.py
+-rw-r--r--   0        0        0      195 2024-04-02 20:31:31.417190 taskara-0.1.2/taskara/env.py
+-rw-r--r--   0        0        0     1606 2024-04-02 20:58:29.041770 taskara-0.1.2/taskara/models.py
+-rw-r--r--   0        0        0    20304 2024-04-02 20:38:39.122416 taskara-0.1.2/taskara/task.py
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 taskara-0.1.2/PKG-INFO
```

### Comparing `taskara-0.1.1/LICENSE` & `taskara-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskara-0.1.1/taskara/db/conn.py` & `taskara-0.1.2/taskara/db/conn.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.1/taskara/db/models.py` & `taskara-0.1.2/taskara/db/models.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.1/taskara/models.py` & `taskara-0.1.2/taskara/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,7 +48,14 @@
     email: Optional[str] = None
     display_name: Optional[str] = None
     handle: Optional[str] = None
     picture: Optional[str] = None
     created: Optional[int] = None
     updated: Optional[int] = None
     token: Optional[str] = None
+
+
+class SolveTaskModel(BaseModel):
+    task: TaskModel
+    desktop_name: Optional[str] = None
+    max_steps: int = 20
+    site: Optional[str] = None
```

### Comparing `taskara-0.1.1/taskara/task.py` & `taskara-0.1.2/taskara/task.py`

 * *Files identical despite different names*

### Comparing `taskara-0.1.1/PKG-INFO` & `taskara-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskara
-Version: 0.1.1
+Version: 0.1.2
 Summary: Task management for AI agents
 License: Apache 2.0
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

