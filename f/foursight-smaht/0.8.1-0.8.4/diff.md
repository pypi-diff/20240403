# Comparing `tmp/foursight_smaht-0.8.1.tar.gz` & `tmp/foursight_smaht-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_smaht-0.8.1.tar", max compression
+gzip compressed data, was "foursight_smaht-0.8.4.tar", max compression
```

## Comparing `foursight_smaht-0.8.1.tar` & `foursight_smaht-0.8.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/LICENSE.txt
--rw-r--r--   0        0        0        0 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/__init__.py
--rw-r--r--   0        0        0     1030 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/app_utils.py
--rw-r--r--   0        0        0      873 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/buckets.py
--rw-r--r--   0        0        0     4805 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/check_schedules.py
--rw-r--r--   0        0        0    13247 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json
--rw-r--r--   0        0        0     6530 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json-local
--rw-r--r--   0        0        0    13660 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json-smaht-wolf
--rw-r--r--   0        0        0      249 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/__init__.py
--rw-r--r--   0        0        0     3205 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/audit_checks.py
--rw-r--r--   0        0        0     2883 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/es_checks.py
--rw-r--r--   0        0        0      262 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/constants.py
--rw-r--r--   0        0        0    12321 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     3993 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/utils.py
--rw-r--r--   0        0        0     1598 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2572 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    22420 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/system_checks.py
--rw-r--r--   0        0        0    34795 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/wfr_checks.py
--rw-r--r--   0        0        0     2595 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/checks/wrangler_checks.py
--rw-r--r--   0        0        0      773 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/deploy.py
--rw-r--r--   0        0        0      131 2024-03-08 15:09:44.452886 foursight_smaht-0.8.1/chalicelib_smaht/gitinfo.json
--rw-r--r--   0        0        0      601 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/package.py
--rw-r--r--   0        0        0      323 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/scripts/local_check_execution.py
--rw-r--r--   0        0        0      253 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/chalicelib_smaht/vars.py
--rw-r--r--   0        0        0     1566 2024-03-08 15:09:33.728852 foursight_smaht-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 foursight_smaht-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/LICENSE.txt
+-rw-r--r--   0        0        0        0 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/app_utils.py
+-rw-r--r--   0        0        0      873 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/buckets.py
+-rw-r--r--   0        0        0     4960 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/check_schedules.py
+-rw-r--r--   0        0        0    14108 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json
+-rw-r--r--   0        0        0     6530 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json-local
+-rw-r--r--   0        0        0    13660 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json-smaht-wolf
+-rw-r--r--   0        0        0      249 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/__init__.py
+-rw-r--r--   0        0        0     5682 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/audit_checks.py
+-rw-r--r--   0        0        0     2883 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/es_checks.py
+-rw-r--r--   0        0        0      262 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/constants.py
+-rw-r--r--   0        0        0    12321 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     3993 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/utils.py
+-rw-r--r--   0        0        0     1598 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2572 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    22420 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/system_checks.py
+-rw-r--r--   0        0        0    34795 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/wfr_checks.py
+-rw-r--r--   0        0        0     2595 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      773 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/deploy.py
+-rw-r--r--   0        0        0      131 2024-04-03 16:47:14.047808 foursight_smaht-0.8.4/chalicelib_smaht/gitinfo.json
+-rw-r--r--   0        0        0      601 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/package.py
+-rw-r--r--   0        0        0      323 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/scripts/local_check_execution.py
+-rw-r--r--   0        0        0      253 2024-04-03 16:47:01.723889 foursight_smaht-0.8.4/chalicelib_smaht/vars.py
+-rw-r--r--   0        0        0     1566 2024-04-03 16:47:01.727889 foursight_smaht-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 foursight_smaht-0.8.4/PKG-INFO
```

### Comparing `foursight_smaht-0.8.1/LICENSE.txt` & `foursight_smaht-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/app_utils.py` & `foursight_smaht-0.8.4/chalicelib_smaht/app_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/buckets.py` & `foursight_smaht-0.8.4/chalicelib_smaht/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/check_schedules.py` & `foursight_smaht-0.8.4/chalicelib_smaht/check_schedules.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
 @schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
 def hourly_checks_2(event):
     app.core.queue_scheduled_checks('all', 'hourly_checks_2')
 
 
 @schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
+def monday_checks(event):
+    app.core.queue_scheduled_checks('all', 'monday_checks')
+
+
+@schedule(SCHEDULES, stage=STAGE, disabled_stages=DISABLED_STAGES)
 def monthly_checks(event):
     app.core.queue_scheduled_checks('all', 'monthly_checks')
 
 
 @app.lambda_function()
 def check_runner(event, context):
     """
```

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json` & `foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.935546875%*

 * *Differences: {"'check_for_new_submissions'": "OrderedDict([('title', 'Checks For New Submissions'), ('group', "*

 * *                                "'Audit Checks'), ('schedule', OrderedDict([('monday_checks', "*

 * *                                "OrderedDict([('data', OrderedDict([('kwargs', "*

 * *                                "OrderedDict([('primary', True)])), ('dependencies', [])]))]))])), "*

 * *                                "('display', ['staging'])])",*

 * * "'check_submitted_md5'": "OrderedDict([('title', 'Checks Submitted MD5 C […]*

```diff
@@ -53,14 +53,31 @@
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "Check for files that require lifecycle updates"
     },
+    "check_for_new_submissions": {
+        "display": [
+            "staging"
+        ],
+        "group": "Audit Checks",
+        "schedule": {
+            "monday_checks": {
+                "data": {
+                    "dependencies": [],
+                    "kwargs": {
+                        "primary": true
+                    }
+                }
+            }
+        },
+        "title": "Checks For New Submissions"
+    },
     "check_long_running_ec2s": {
         "display": [
             "staging"
         ],
         "group": "System Checks",
         "schedule": {
             "morning_checks": {
@@ -70,14 +87,31 @@
                         "primary": true
                     }
                 }
             }
         },
         "title": "Check Long-Running EC2s"
     },
+    "check_submitted_md5": {
+        "display": [
+            "staging"
+        ],
+        "group": "Audit Checks",
+        "schedule": {
+            "morning_checks_1": {
+                "data": {
+                    "dependencies": [],
+                    "kwargs": {
+                        "primary": true
+                    }
+                }
+            }
+        },
+        "title": "Checks Submitted MD5 Consistency"
+    },
     "check_validation_errors": {
         "display": [
             "staging"
         ],
         "group": "Audit Checks",
         "schedule": {
             "monthly_checks": {
@@ -297,19 +331,19 @@
     "md5run_status": {
         "display": [
             "staging",
             "data"
         ],
         "group": "Pipeline Checks",
         "schedule": {
-            "hourly_checks": {
+            "thirty_min_checks": {
                 "data": {
                     "dependencies": [],
                     "kwargs": {
-                        "max_files": 50,
+                        "max_files": 100,
                         "primary": true,
                         "queue_action": "prod"
                     }
                 }
             }
         },
         "title": "MD5 runs"
```

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json-local` & `foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/check_setup.json-smaht-wolf` & `foursight_smaht-0.8.4/chalicelib_smaht/check_setup.json-smaht-wolf`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/ecs_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/es_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/lifecycle_utils.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/linecount_dicts.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/utils.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/wfr_utils.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/helpers/wfrset_utils.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/lifecycle_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/system_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/wfr_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/checks/wrangler_checks.py` & `foursight_smaht-0.8.4/chalicelib_smaht/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/deploy.py` & `foursight_smaht-0.8.4/chalicelib_smaht/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/chalicelib_smaht/package.py` & `foursight_smaht-0.8.4/chalicelib_smaht/package.py`

 * *Files identical despite different names*

### Comparing `foursight_smaht-0.8.1/pyproject.toml` & `foursight_smaht-0.8.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-smaht"
-version = "0.8.1"
+version = "0.8.4"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_smaht" }
 ]
```

### Comparing `foursight_smaht-0.8.1/PKG-INFO` & `foursight_smaht-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-smaht
-Version: 0.8.1
+Version: 0.8.4
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

