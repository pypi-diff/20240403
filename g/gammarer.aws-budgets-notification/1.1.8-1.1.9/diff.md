# Comparing `tmp/gammarer.aws-budgets-notification-1.1.8.tar.gz` & `tmp/gammarer.aws-budgets-notification-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-budgets-notification-1.1.8.tar", last modified: Wed Mar  6 19:13:44 2024, max compression
+gzip compressed data, was "gammarer.aws-budgets-notification-1.1.9.tar", last modified: Wed Mar 13 19:17:00 2024, max compression
```

## Comparing `gammarer.aws-budgets-notification-1.1.8.tar` & `gammarer.aws-budgets-notification-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74242 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 19:13:33.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:13:44.020233 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-06 19:13:43.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-06 19:13:43.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 19:13:43.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 19:13:43.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 19:13:43.000000 gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.717109 gammarer.aws-budgets-notification-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-13 19:17:00.717109 gammarer.aws-budgets-notification-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 19:17:00.717109 gammarer.aws-budgets-notification-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.713109 gammarer.aws-budgets-notification-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.713109 gammarer.aws-budgets-notification-1.1.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.713109 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.717109 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74241 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:16:49.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 19:17:00.713109 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-13 19:17:00.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-13 19:17:00.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 19:17:00.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-13 19:17:00.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 19:17:00.000000 gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/top_level.txt
```

### Comparing `gammarer.aws-budgets-notification-1.1.8/LICENSE` & `gammarer.aws-budgets-notification-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-1.1.8/PKG-INFO` & `gammarer.aws-budgets-notification-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-budgets-notification
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS Budgets Notification
 Home-page: https://github.com/gammarer/aws-budgets-notification.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-budgets-notification.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-budgets-notification-1.1.8/README.md` & `gammarer.aws-budgets-notification-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-1.1.8/setup.py` & `gammarer.aws-budgets-notification-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-budgets-notification",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "AWS Budgets Notification",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-budgets-notification.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_budgets_notification",
         "gammarer.aws_budgets_notification._jsii"
     ],
     "package_data": {
         "gammarer.aws_budgets_notification._jsii": [
-            "aws-budgets-notification@1.1.8.jsii.tgz"
+            "aws-budgets-notification@1.1.9.jsii.tgz"
         ],
         "gammarer.aws_budgets_notification": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-budgets-notification-1.1.8/src/gammarer/aws_budgets_notification/__init__.py` & `gammarer.aws-budgets-notification-1.1.9/src/gammarer/aws_budgets_notification/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO` & `gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-budgets-notification
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS Budgets Notification
 Home-page: https://github.com/gammarer/aws-budgets-notification.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-budgets-notification.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-budgets-notification-1.1.8/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt` & `gammarer.aws-budgets-notification-1.1.9/src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_budgets_notification.egg-info/SOURCES.txt
 src/gammarer.aws_budgets_notification.egg-info/dependency_links.txt
 src/gammarer.aws_budgets_notification.egg-info/requires.txt
 src/gammarer.aws_budgets_notification.egg-info/top_level.txt
 src/gammarer/aws_budgets_notification/__init__.py
 src/gammarer/aws_budgets_notification/py.typed
 src/gammarer/aws_budgets_notification/_jsii/__init__.py
-src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@1.1.8.jsii.tgz
+src/gammarer/aws_budgets_notification/_jsii/aws-budgets-notification@1.1.9.jsii.tgz
```

