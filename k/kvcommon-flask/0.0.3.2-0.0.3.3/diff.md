# Comparing `tmp/kvcommon_flask-0.0.3.2.tar.gz` & `tmp/kvcommon_flask-0.0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kvcommon_flask-0.0.3.2.tar", max compression
+gzip compressed data, was "kvcommon_flask-0.0.3.3.tar", max compression
```

## Comparing `kvcommon_flask-0.0.3.2.tar` & `kvcommon_flask-0.0.3.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1072 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/LICENSE
--rw-r--r--   0        0        0     1046 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/README.md
--rw-r--r--   0        0        0     1235 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1212 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/context.py
--rw-r--r--   0        0        0      100 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/exceptions.py
--rw-r--r--   0        0        0      601 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/metrics/__init__.py
--rw-r--r--   0        0        0     1182 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/metrics/metrics.py
--rw-r--r--   0        0        0     1727 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/middleware.py
--rw-r--r--   0        0        0     2562 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/scheduler.py
--rw-r--r--   0        0        0      106 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/traces/__init__.py
--rw-r--r--   0        0        0      302 2024-03-21 07:23:44.006333 kvcommon_flask-0.0.3.2/src/kvcommon_flask/vars.py
--rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/LICENSE
+-rw-r--r--   0        0        0     1046 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/README.md
+-rw-r--r--   0        0        0     1235 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1212 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/context.py
+-rw-r--r--   0        0        0      100 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/exceptions.py
+-rw-r--r--   0        0        0      601 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/metrics/__init__.py
+-rw-r--r--   0        0        0     1182 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/metrics/metrics.py
+-rw-r--r--   0        0        0     1727 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/middleware.py
+-rw-r--r--   0        0        0     2560 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/scheduler.py
+-rw-r--r--   0        0        0      106 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/traces/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-03 11:00:29.890209 kvcommon_flask-0.0.3.3/src/kvcommon_flask/vars.py
+-rw-r--r--   0        0        0     1677 1970-01-01 00:00:00.000000 kvcommon_flask-0.0.3.3/PKG-INFO
```

### Comparing `kvcommon_flask-0.0.3.2/LICENSE` & `kvcommon_flask-0.0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/README.md` & `kvcommon_flask-0.0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/pyproject.toml` & `kvcommon_flask-0.0.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kvcommon-flask"
-version = "0.0.3.2"
+version = "0.0.3.3"
 description = "Library of various Flask utils that aren't worthy of their own dedicated libs."
 authors = ["Rob Voigt <code@ravoigt.com>"]
 readme = "README.md"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `kvcommon_flask-0.0.3.2/src/kvcommon_flask/context.py` & `kvcommon_flask-0.0.3.3/src/kvcommon_flask/context.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/src/kvcommon_flask/metrics/__init__.py` & `kvcommon_flask-0.0.3.3/src/kvcommon_flask/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/src/kvcommon_flask/metrics/metrics.py` & `kvcommon_flask-0.0.3.3/src/kvcommon_flask/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/src/kvcommon_flask/middleware.py` & `kvcommon_flask-0.0.3.3/src/kvcommon_flask/middleware.py`

 * *Files identical despite different names*

### Comparing `kvcommon_flask-0.0.3.2/src/kvcommon_flask/scheduler.py` & `kvcommon_flask-0.0.3.3/src/kvcommon_flask/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class SchedulerEventTracker(object):
 
     @staticmethod
     def _job_event_track(job_id: str, event: str):
         LOG.debug(f"Scheduler Event Listener: {event}: Job <'{job_id}'>")
-        metrics.incr(metrics.SCHEDULER_JOB_EVENT.labels(job_id=job_id, eventnt=event.lower()))
+        metrics.incr(metrics.SCHEDULER_JOB_EVENT.labels(job_id=job_id, event=event.lower()))
 
     @staticmethod
     def event_listener(event):
         if isinstance(event, JobExecutionEvent):
             event_str = "Unknown"
             if event.exception or event.code == EVENT_JOB_ERROR:
                 event_str = "Error"
```

### Comparing `kvcommon_flask-0.0.3.2/PKG-INFO` & `kvcommon_flask-0.0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kvcommon-flask
-Version: 0.0.3.2
+Version: 0.0.3.3
 Summary: Library of various Flask utils that aren't worthy of their own dedicated libs.
 Author: Rob Voigt
 Author-email: code@ravoigt.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

