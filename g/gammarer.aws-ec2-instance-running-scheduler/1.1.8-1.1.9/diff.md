# Comparing `tmp/gammarer.aws-ec2-instance-running-scheduler-1.1.8.tar.gz` & `tmp/gammarer.aws-ec2-instance-running-scheduler-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-1.1.8.tar", last modified: Wed Feb 28 16:21:24 2024, max compression
+gzip compressed data, was "gammarer.aws-ec2-instance-running-scheduler-1.1.9.tar", last modified: Wed Mar  6 16:22:02 2024, max compression
```

## Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8.tar` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.930014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.930014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21401 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@1.1.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:21:14.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 16:21:24.934014 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-02-28 16:21:24.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-02-28 16:21:24.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 16:21:24.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-28 16:21:24.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-28 16:21:24.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.001782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.001782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21400 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@1.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 16:21:48.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 16:22:02.005782 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-03-06 16:22:01.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-06 16:22:01.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 16:22:01.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-06 16:22:01.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 16:22:01.000000 gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/LICENSE` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/gammarer/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/README.md` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/setup.py` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-ec2-instance-running-scheduler",
-    "version": "1.1.8",
+    "version": "1.1.9",
     "description": "AWS EC2 Instance Running Scheduler",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-ec2-instance-running-scheduler.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "gammarer.aws_ec2_instance_running_scheduler",
         "gammarer.aws_ec2_instance_running_scheduler._jsii"
     ],
     "package_data": {
         "gammarer.aws_ec2_instance_running_scheduler._jsii": [
-            "aws-ec2-instance-running-scheduler@1.1.8.jsii.tgz"
+            "aws-ec2-instance-running-scheduler@1.1.9.jsii.tgz"
         ],
         "gammarer.aws_ec2_instance_running_scheduler": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.80.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer/aws_ec2_instance_running_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-ec2-instance-running-scheduler
-Version: 1.1.8
+Version: 1.1.9
 Summary: AWS EC2 Instance Running Scheduler
 Home-page: https://github.com/gammarer/aws-ec2-instance-running-scheduler.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-ec2-instance-running-scheduler.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-ec2-instance-running-scheduler-1.1.8/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt` & `gammarer.aws-ec2-instance-running-scheduler-1.1.9/src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/SOURCES.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/dependency_links.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/requires.txt
 src/gammarer.aws_ec2_instance_running_scheduler.egg-info/top_level.txt
 src/gammarer/aws_ec2_instance_running_scheduler/__init__.py
 src/gammarer/aws_ec2_instance_running_scheduler/py.typed
 src/gammarer/aws_ec2_instance_running_scheduler/_jsii/__init__.py
-src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@1.1.8.jsii.tgz
+src/gammarer/aws_ec2_instance_running_scheduler/_jsii/aws-ec2-instance-running-scheduler@1.1.9.jsii.tgz
```

