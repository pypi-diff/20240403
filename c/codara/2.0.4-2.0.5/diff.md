# Comparing `tmp/codara-2.0.4.tar.gz` & `tmp/codara-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codara-2.0.4.tar", last modified: Wed Apr  3 19:17:57 2024, max compression
+gzip compressed data, was "codara-2.0.5.tar", last modified: Wed Apr  3 19:39:08 2024, max compression
```

## Comparing `codara-2.0.4.tar` & `codara-2.0.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:17:57.536394 codara-2.0.4/
--rw-r--r--   0 rafay826   (501) staff       (20)     4031 2024-04-03 19:17:57.536038 codara-2.0.4/PKG-INFO
--rw-r--r--   0 rafay826   (501) staff       (20)     2842 2024-04-03 19:15:26.000000 codara-2.0.4/README.md
-drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:17:57.535686 codara-2.0.4/codara.egg-info/
--rw-r--r--   0 rafay826   (501) staff       (20)     4031 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/PKG-INFO
--rw-r--r--   0 rafay826   (501) staff       (20)      535 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/SOURCES.txt
--rw-r--r--   0 rafay826   (501) staff       (20)        1 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/dependency_links.txt
--rw-r--r--   0 rafay826   (501) staff       (20)       44 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/entry_points.txt
--rw-r--r--   0 rafay826   (501) staff       (20)      548 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/requires.txt
--rw-r--r--   0 rafay826   (501) staff       (20)        8 2024-04-03 19:17:57.000000 codara-2.0.4/codara.egg-info/top_level.txt
-drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:17:57.534506 codara-2.0.4/package/
--rw-r--r--   0 rafay826   (501) staff       (20)        0 2023-11-28 04:19:00.000000 codara-2.0.4/package/__init__.py
--rw-r--r--   0 rafay826   (501) staff       (20)     7032 2024-01-19 17:31:00.000000 codara-2.0.4/package/app.py
--rw-r--r--   0 rafay826   (501) staff       (20)     4023 2024-01-19 17:31:00.000000 codara-2.0.4/package/auth.py
--rw-r--r--   0 rafay826   (501) staff       (20)      422 2024-04-03 19:17:57.000000 codara-2.0.4/package/config.py
--rw-r--r--   0 rafay826   (501) staff       (20)     2737 2024-01-22 19:55:03.000000 codara-2.0.4/package/diagnose.py
--rw-r--r--   0 rafay826   (501) staff       (20)     1905 2024-01-19 17:31:00.000000 codara-2.0.4/package/git_utils.py
--rwxr-xr-x   0 rafay826   (501) staff       (20)     2817 2024-03-12 16:33:22.000000 codara-2.0.4/package/review.py
--rw-r--r--   0 rafay826   (501) staff       (20)     3315 2024-01-19 17:31:00.000000 codara-2.0.4/package/server.py
-drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:17:57.535442 codara-2.0.4/package/tests/
--rw-r--r--   0 rafay826   (501) staff       (20)        0 2024-01-19 17:31:00.000000 codara-2.0.4/package/tests/__init__.py
--rw-r--r--   0 rafay826   (501) staff       (20)     2541 2024-01-19 17:31:00.000000 codara-2.0.4/package/tests/test_auth.py
--rw-r--r--   0 rafay826   (501) staff       (20)      860 2024-01-19 17:31:00.000000 codara-2.0.4/package/tests/test_git_utils.py
--rw-r--r--   0 rafay826   (501) staff       (20)     2634 2024-01-19 17:31:00.000000 codara-2.0.4/package/tests/test_review.py
--rw-r--r--   0 rafay826   (501) staff       (20)     2989 2024-01-19 17:31:00.000000 codara-2.0.4/package/token_utils.py
--rw-r--r--   0 rafay826   (501) staff       (20)     1895 2024-01-19 17:31:00.000000 codara-2.0.4/package/user.py
--rw-r--r--   0 rafay826   (501) staff       (20)     2128 2024-01-19 17:31:00.000000 codara-2.0.4/package/utils.py
--rw-r--r--   0 rafay826   (501) staff       (20)       18 2024-04-03 19:15:45.000000 codara-2.0.4/package/version.py
--rw-r--r--   0 rafay826   (501) staff       (20)       38 2024-04-03 19:17:57.536443 codara-2.0.4/setup.cfg
--rw-r--r--   0 rafay826   (501) staff       (20)      746 2024-01-19 17:31:00.000000 codara-2.0.4/setup.py
+drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:39:08.233051 codara-2.0.5/
+-rw-r--r--   0 rafay826   (501) staff       (20)     4271 2024-04-03 19:39:08.232802 codara-2.0.5/PKG-INFO
+-rw-r--r--   0 rafay826   (501) staff       (20)     3082 2024-04-03 19:38:26.000000 codara-2.0.5/README.md
+drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:39:08.232549 codara-2.0.5/codara.egg-info/
+-rw-r--r--   0 rafay826   (501) staff       (20)     4271 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/PKG-INFO
+-rw-r--r--   0 rafay826   (501) staff       (20)      535 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/SOURCES.txt
+-rw-r--r--   0 rafay826   (501) staff       (20)        1 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/dependency_links.txt
+-rw-r--r--   0 rafay826   (501) staff       (20)       44 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/entry_points.txt
+-rw-r--r--   0 rafay826   (501) staff       (20)      548 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/requires.txt
+-rw-r--r--   0 rafay826   (501) staff       (20)        8 2024-04-03 19:39:08.000000 codara-2.0.5/codara.egg-info/top_level.txt
+drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:39:08.231733 codara-2.0.5/package/
+-rw-r--r--   0 rafay826   (501) staff       (20)        0 2023-11-28 04:19:00.000000 codara-2.0.5/package/__init__.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     7032 2024-01-19 17:31:00.000000 codara-2.0.5/package/app.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     4023 2024-01-19 17:31:00.000000 codara-2.0.5/package/auth.py
+-rw-r--r--   0 rafay826   (501) staff       (20)      422 2024-04-03 19:39:07.000000 codara-2.0.5/package/config.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     2737 2024-01-22 19:55:03.000000 codara-2.0.5/package/diagnose.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     1905 2024-01-19 17:31:00.000000 codara-2.0.5/package/git_utils.py
+-rwxr-xr-x   0 rafay826   (501) staff       (20)     2817 2024-03-12 16:33:22.000000 codara-2.0.5/package/review.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     3315 2024-01-19 17:31:00.000000 codara-2.0.5/package/server.py
+drwxr-xr-x   0 rafay826   (501) staff       (20)        0 2024-04-03 19:39:08.232362 codara-2.0.5/package/tests/
+-rw-r--r--   0 rafay826   (501) staff       (20)        0 2024-01-19 17:31:00.000000 codara-2.0.5/package/tests/__init__.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     2541 2024-01-19 17:31:00.000000 codara-2.0.5/package/tests/test_auth.py
+-rw-r--r--   0 rafay826   (501) staff       (20)      860 2024-01-19 17:31:00.000000 codara-2.0.5/package/tests/test_git_utils.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     2634 2024-01-19 17:31:00.000000 codara-2.0.5/package/tests/test_review.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     2989 2024-01-19 17:31:00.000000 codara-2.0.5/package/token_utils.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     1895 2024-01-19 17:31:00.000000 codara-2.0.5/package/user.py
+-rw-r--r--   0 rafay826   (501) staff       (20)     2128 2024-01-19 17:31:00.000000 codara-2.0.5/package/utils.py
+-rw-r--r--   0 rafay826   (501) staff       (20)       18 2024-04-03 19:38:35.000000 codara-2.0.5/package/version.py
+-rw-r--r--   0 rafay826   (501) staff       (20)       38 2024-04-03 19:39:08.233090 codara-2.0.5/setup.cfg
+-rw-r--r--   0 rafay826   (501) staff       (20)      746 2024-01-19 17:31:00.000000 codara-2.0.5/setup.py
```

### Comparing `codara-2.0.4/PKG-INFO` & `codara-2.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codara
-Version: 2.0.4
+Version: 2.0.5
 Summary: AI Code Review Automation Tool
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: blinker==1.7.0
 Requires-Dist: certifi==2023.11.17
 Requires-Dist: cffi==1.16.0
@@ -40,17 +40,17 @@
 
 # Codara Code Review and Diagnostics Tool
 
 This script assists in AI code review and diagnosis by using tailored AI models to intelligently provide suggestions and improvements. Purchase a subscription at [codara.io](https://codara.io)
 
 ## Subscribe to use this tool: [codara.io](https://codara.io)
 
-| Plan      | Price     | Description                                                                                            | Link            |
-|-----------|-----------|--------------------------------------------------------------------------------------------------------|-----------------|
-| Basic     | $10/month | - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Sign Up](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI)     |
+| Plan      | Price     | Description                                                                                                                | Link                                                                                                    |
+|-----------|-----------|----------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
+| Basic     | $10/month | - 14 day free trial<br/> - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Free Trial](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI) |
 
 [//]: # (| Pro       | $30/month | Access to all basic features plus more.      | [Sign Up]&#40;#&#41;    |)
 
 [//]: # (| Ultimate  | $60/month | All features from Pro, plus premium support. | [Sign Up]&#40;#&#41;    |)
 
 
 ## Features
```

### Comparing `codara-2.0.4/README.md` & `codara-2.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Codara Code Review and Diagnostics Tool
 
 This script assists in AI code review and diagnosis by using tailored AI models to intelligently provide suggestions and improvements. Purchase a subscription at [codara.io](https://codara.io)
 
 ## Subscribe to use this tool: [codara.io](https://codara.io)
 
-| Plan      | Price     | Description                                                                                            | Link            |
-|-----------|-----------|--------------------------------------------------------------------------------------------------------|-----------------|
-| Basic     | $10/month | - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Sign Up](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI)     |
+| Plan      | Price     | Description                                                                                                                | Link                                                                                                    |
+|-----------|-----------|----------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
+| Basic     | $10/month | - 14 day free trial<br/> - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Free Trial](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI) |
 
 [//]: # (| Pro       | $30/month | Access to all basic features plus more.      | [Sign Up]&#40;#&#41;    |)
 
 [//]: # (| Ultimate  | $60/month | All features from Pro, plus premium support. | [Sign Up]&#40;#&#41;    |)
 
 
 ## Features
```

### Comparing `codara-2.0.4/codara.egg-info/PKG-INFO` & `codara-2.0.5/codara.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codara
-Version: 2.0.4
+Version: 2.0.5
 Summary: AI Code Review Automation Tool
 Description-Content-Type: text/markdown
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: blinker==1.7.0
 Requires-Dist: certifi==2023.11.17
 Requires-Dist: cffi==1.16.0
@@ -40,17 +40,17 @@
 
 # Codara Code Review and Diagnostics Tool
 
 This script assists in AI code review and diagnosis by using tailored AI models to intelligently provide suggestions and improvements. Purchase a subscription at [codara.io](https://codara.io)
 
 ## Subscribe to use this tool: [codara.io](https://codara.io)
 
-| Plan      | Price     | Description                                                                                            | Link            |
-|-----------|-----------|--------------------------------------------------------------------------------------------------------|-----------------|
-| Basic     | $10/month | - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Sign Up](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI)     |
+| Plan      | Price     | Description                                                                                                                | Link                                                                                                    |
+|-----------|-----------|----------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------|
+| Basic     | $10/month | - 14 day free trial<br/> - unlimited reviews<br/> - diagnostic feature<br/> - review unstaged code<br/> - locally saved reviews | [Free Trial](https://www.paypal.com/webapps/billing/plans/subscribe?plan_id=P-2YR33470WV105614YMXX5QQI) |
 
 [//]: # (| Pro       | $30/month | Access to all basic features plus more.      | [Sign Up]&#40;#&#41;    |)
 
 [//]: # (| Ultimate  | $60/month | All features from Pro, plus premium support. | [Sign Up]&#40;#&#41;    |)
 
 
 ## Features
```

### Comparing `codara-2.0.4/codara.egg-info/SOURCES.txt` & `codara-2.0.5/codara.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/codara.egg-info/requires.txt` & `codara-2.0.5/codara.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/app.py` & `codara-2.0.5/package/app.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/auth.py` & `codara-2.0.5/package/auth.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/diagnose.py` & `codara-2.0.5/package/diagnose.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/git_utils.py` & `codara-2.0.5/package/git_utils.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/review.py` & `codara-2.0.5/package/review.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/server.py` & `codara-2.0.5/package/server.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/tests/test_auth.py` & `codara-2.0.5/package/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/tests/test_git_utils.py` & `codara-2.0.5/package/tests/test_git_utils.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/tests/test_review.py` & `codara-2.0.5/package/tests/test_review.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/token_utils.py` & `codara-2.0.5/package/token_utils.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/user.py` & `codara-2.0.5/package/user.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/package/utils.py` & `codara-2.0.5/package/utils.py`

 * *Files identical despite different names*

### Comparing `codara-2.0.4/setup.py` & `codara-2.0.5/setup.py`

 * *Files identical despite different names*
