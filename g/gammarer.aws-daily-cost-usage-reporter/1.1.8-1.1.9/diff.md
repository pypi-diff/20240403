# Comparing `tmp/gammarer.aws-daily-cost-usage-reporter-1.1.8.tar.gz` & `tmp/gammarer.aws-daily-cost-usage-reporter-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-1.1.8.tar", last modified: Wed Mar 20 19:19:46 2024, max compression
+gzip compressed data, was "gammarer.aws-daily-cost-usage-reporter-1.1.9.tar", last modified: Wed Mar 27 19:19:54 2024, max compression
```

## Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8.tar` & `gammarer.aws-daily-cost-usage-reporter-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.197850 gammarer.aws-daily-cost-usage-reporter-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-20 19:19:46.197850 gammarer.aws-daily-cost-usage-reporter-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 19:19:46.197850 gammarer.aws-daily-cost-usage-reporter-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.193850 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.193850 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.193850 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/
--rw-r--r--   0 runner    (1001) docker     (127)     6756 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.197850 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   270201 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:19:31.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 19:19:46.193850 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-20 19:19:46.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-20 19:19:46.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 19:19:46.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-20 19:19:46.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-20 19:19:46.000000 gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.047431 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.047431 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   270198 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:19:41.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 19:19:54.051431 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-03-27 19:19:54.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-27 19:19:54.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 19:19:54.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-27 19:19:54.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-27 19:19:54.000000 gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/LICENSE` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 1.1.8
+Version: 1.1.9
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/README.md` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/setup.py` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-daily-cost-usage-reporter",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "Cost & Usage Reports",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-daily-cost-usage-reporter.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_daily_cost_usage_reporter",
         "gammarer.aws_daily_cost_usage_reporter._jsii"
     ],
     "package_data": {
         "gammarer.aws_daily_cost_usage_reporter._jsii": [
-            "aws-daily-cost-usage-reporter@1.1.8.jsii.tgz"
+            "aws-daily-cost-usage-reporter@1.1.9.jsii.tgz"
         ],
         "gammarer.aws_daily_cost_usage_reporter": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer/aws_daily_cost_usage_reporter/__init__.py` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer/aws_daily_cost_usage_reporter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 });
 ```
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-daily-cost-usage-reporter
-Version: 1.1.8
+Version: 1.1.9
 Summary: Cost & Usage Reports
 Home-page: https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-daily-cost-usage-reporter.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-daily-cost-usage-reporter-1.1.8/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt` & `gammarer.aws-daily-cost-usage-reporter-1.1.9/src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/SOURCES.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/dependency_links.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/requires.txt
 src/gammarer.aws_daily_cost_usage_reporter.egg-info/top_level.txt
 src/gammarer/aws_daily_cost_usage_reporter/__init__.py
 src/gammarer/aws_daily_cost_usage_reporter/py.typed
 src/gammarer/aws_daily_cost_usage_reporter/_jsii/__init__.py
-src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@1.1.8.jsii.tgz
+src/gammarer/aws_daily_cost_usage_reporter/_jsii/aws-daily-cost-usage-reporter@1.1.9.jsii.tgz
```

