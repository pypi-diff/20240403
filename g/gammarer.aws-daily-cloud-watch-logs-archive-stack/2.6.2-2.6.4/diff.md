# Comparing `tmp/gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2.tar.gz` & `tmp/gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2.tar", last modified: Wed Mar 27 19:13:18 2024, max compression
+gzip compressed data, was "gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4.tar", last modified: Wed Apr  3 19:14:59 2024, max compression
```

## Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2.tar` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.667998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-27 19:13:18.667998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:13:18.667998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.663998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.663998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.663998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    28333 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.663998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45573 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.6.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:13:08.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:13:18.663998 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-03-27 19:13:18.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-27 19:13:18.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:13:18.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-27 19:13:18.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 19:13:18.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.747969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.747969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    28333 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45513 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.6.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:14:48.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:14:59.751969 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-04-03 19:14:59.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-03 19:14:59.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:14:59.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 19:14:59.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 19:14:59.000000 gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/LICENSE` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/PKG-INFO` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.6.2
+Version: 2.6.4
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarer/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/README.md` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/setup.py` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-daily-cloud-watch-logs-archive-stack",
-    "version": "2.6.2",
+    "version": "2.6.4",
     "description": "AWS CloudWatch Logs daily archive to s3 bucket",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-daily-cloud-watch-logs-archive-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_daily_cloud_watch_logs_archive_stack",
         "gammarer.aws_daily_cloud_watch_logs_archive_stack._jsii"
     ],
     "package_data": {
         "gammarer.aws_daily_cloud_watch_logs_archive_stack._jsii": [
-            "aws-daily-cloud-watch-logs-archive-stack@2.6.2.jsii.tgz"
+            "aws-daily-cloud-watch-logs-archive-stack@2.6.4.jsii.tgz"
         ],
         "gammarer.aws_daily_cloud_watch_logs_archive_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/__init__.py` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer/aws_daily_cloud_watch_logs_archive_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cloud-watch-logs-archive-stack
-Version: 2.6.2
+Version: 2.6.4
 Summary: AWS CloudWatch Logs daily archive to s3 bucket
 Home-page: https://github.com/gammarer/aws-daily-cloud-watch-logs-archive-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-daily-cloud-watch-logs-archive-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.2/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt` & `gammarer.aws-daily-cloud-watch-logs-archive-stack-2.6.4/src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/SOURCES.txt
 src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/dependency_links.txt
 src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/requires.txt
 src/gammarer.aws_daily_cloud_watch_logs_archive_stack.egg-info/top_level.txt
 src/gammarer/aws_daily_cloud_watch_logs_archive_stack/__init__.py
 src/gammarer/aws_daily_cloud_watch_logs_archive_stack/py.typed
 src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/__init__.py
-src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.6.2.jsii.tgz
+src/gammarer/aws_daily_cloud_watch_logs_archive_stack/_jsii/aws-daily-cloud-watch-logs-archive-stack@2.6.4.jsii.tgz
```

