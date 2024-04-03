# Comparing `tmp/mypy-boto3-lambda-1.34.58.tar.gz` & `tmp/mypy-boto3-lambda-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.34.58.tar", last modified: Thu Mar  7 20:22:52 2024, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.34.77.tar", last modified: Wed Apr  3 19:32:39 2024, max compression
```

## Comparing `mypy-boto3-lambda-1.34.58.tar` & `mypy-boto3-lambda-1.34.77.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.802007 mypy-boto3-lambda-1.34.58/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-03-07 20:22:52.802007 mypy-boto3-lambda-1.34.58/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14532 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.802007 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-03-07 20:22:17.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    59784 2024-03-07 20:22:17.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    72445 2024-03-07 20:22:19.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    72445 2024-03-07 20:22:19.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-03-07 20:22:18.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 20:22:52.802007 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-07 20:22:52.000000 mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 20:22:52.802007 mypy-boto3-lambda-1.34.58/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-07 20:22:16.000000 mypy-boto3-lambda-1.34.58/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.864160 mypy-boto3-lambda-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-04-03 19:32:39.864160 mypy-boto3-lambda-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14532 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.860160 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59787 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59784 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13808 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    72445 2024-04-03 19:32:16.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72445 2024-04-03 19:32:15.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6154 2024-04-03 19:32:14.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:39.864160 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16083 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 19:32:39.000000 mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:39.864160 mypy-boto3-lambda-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-03 19:32:13.000000 mypy-boto3-lambda-1.34.77/setup.py
```

### Comparing `mypy-boto3-lambda-1.34.58/LICENSE` & `mypy-boto3-lambda-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/PKG-INFO` & `mypy-boto3-lambda-1.34.77/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.34.58
-Summary: Type annotations for boto3.Lambda 1.34.58 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.Lambda 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-lambda-1.34.58/README.md` & `mypy-boto3-lambda-1.34.77/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.34.58\n"
-        "Version:         1.34.58\n"
+        "Type annotations for boto3.Lambda 1.34.77\n"
+        "Version:         1.34.77\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.58")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     "python3.6",
     "python3.7",
     "python3.8",
     "python3.9",
     "ruby2.5",
     "ruby2.7",
     "ruby3.2",
+    "ruby3.3",
 ]
 SnapStartApplyOnType = Literal["None", "PublishedVersions"]
 SnapStartOptimizationStatusType = Literal["Off", "On"]
 SourceAccessTypeType = Literal[
     "BASIC_AUTH",
     "CLIENT_CERTIFICATE_TLS_AUTH",
     "SASL_SCRAM_256_AUTH",
@@ -278,14 +279,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -308,14 +310,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -376,15 +379,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -564,14 +566,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
     "python3.6",
     "python3.7",
     "python3.8",
     "python3.9",
     "ruby2.5",
     "ruby2.7",
     "ruby3.2",
+    "ruby3.3",
 ]
 SnapStartApplyOnType = Literal["None", "PublishedVersions"]
 SnapStartOptimizationStatusType = Literal["Off", "On"]
 SourceAccessTypeType = Literal[
     "BASIC_AUTH",
     "CLIENT_CERTIFICATE_TLS_AUTH",
     "SASL_SCRAM_256_AUTH",
@@ -278,14 +279,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -308,14 +310,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -376,15 +379,14 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
-    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -564,14 +566,15 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
+    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
```

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.34.58
-Summary: Type annotations for boto3.Lambda 1.34.58 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.Lambda 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.34.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-lambda-1.34.58/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.34.77/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.34.58/setup.py` & `mypy-boto3-lambda-1.34.77/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.34.58",
+    version="1.34.77",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Lambda 1.34.58 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.Lambda 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

