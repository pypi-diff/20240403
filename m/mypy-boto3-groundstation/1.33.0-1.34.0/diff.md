# Comparing `tmp/mypy-boto3-groundstation-1.33.0.tar.gz` & `tmp/mypy-boto3-groundstation-1.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-groundstation-1.33.0.tar", last modified: Tue Nov 28 18:29:26 2023, max compression
+gzip compressed data, was "mypy-boto3-groundstation-1.34.0.tar", last modified: Wed Dec 13 21:22:46 2023, max compression
```

## Comparing `mypy-boto3-groundstation-1.33.0.tar` & `mypy-boto3-groundstation-1.34.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:26.307151 mypy-boto3-groundstation-1.33.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2023-11-28 18:29:26.307151 mypy-boto3-groundstation-1.33.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:26.307151 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26811 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    26807 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11288 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    34462 2023-11-28 18:17:29.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34461 2023-11-28 18:17:29.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 18:29:26.307151 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14466 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-28 18:29:26.000000 mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 18:29:26.307151 mypy-boto3-groundstation-1.33.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-11-28 18:17:28.000000 mypy-boto3-groundstation-1.33.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:46.223227 mypy-boto3-groundstation-1.34.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14466 2023-12-13 21:22:46.219227 mypy-boto3-groundstation-1.34.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:46.219227 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26811 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26807 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11450 2023-12-13 21:11:13.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11448 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8948 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    34462 2023-12-13 21:11:13.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34461 2023-12-13 21:11:13.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 21:22:46.219227 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14466 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 21:22:46.000000 mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 21:22:46.223227 mypy-boto3-groundstation-1.34.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2023-12-13 21:11:12.000000 mypy-boto3-groundstation-1.34.0/setup.py
```

### Comparing `mypy-boto3-groundstation-1.33.0/LICENSE` & `mypy-boto3-groundstation-1.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/PKG-INFO` & `mypy-boto3-groundstation-1.34.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.33.0
-Summary: Type annotations for boto3.GroundStation 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.GroundStation 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.33.0/README.md` & `mypy-boto3-groundstation-1.34.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__init__.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__init__.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/__main__.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GroundStation 1.33.0\nVersion:         1.33.0\nBuilder version:"
-        " 7.20.3\nDocs:           "
+        "Type annotations for boto3.GroundStation 1.34.0\nVersion:         1.34.0\nBuilder version:"
+        " 7.21.0\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.33.0")
+    print("1.34.0")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/client.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/client.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/literals.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -148,26 +148,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -327,15 +330,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -383,14 +388,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/literals.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/literals.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -146,26 +146,29 @@
     "b2bi",
     "backup",
     "backup-gateway",
     "backupstorage",
     "batch",
     "bcm-data-exports",
     "bedrock",
+    "bedrock-agent",
+    "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
+    "cleanroomsml",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudfront-keyvaluestore",
     "cloudhsm",
@@ -325,15 +328,17 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
     "managedblockchain",
     "managedblockchain-query",
+    "marketplace-agreement",
     "marketplace-catalog",
+    "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
@@ -381,14 +386,16 @@
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
     "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
+    "qbusiness",
+    "qconnect",
     "qldb",
     "qldb-session",
     "quicksight",
     "ram",
     "rbin",
     "rds",
     "rds-data",
```

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/paginator.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/paginator.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/type_defs.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/type_defs.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/waiter.py` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation/waiter.pyi` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/PKG-INFO` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-groundstation
-Version: 1.33.0
-Summary: Type annotations for boto3.GroundStation 1.33.0 service generated with mypy-boto3-builder 7.20.3
+Version: 1.34.0
+Summary: Type annotations for boto3.GroundStation 1.34.0 service generated with mypy-boto3-builder 7.21.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-groundstation.svg?color=blue)](https://pypi.org/project/mypy-boto3-groundstation)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-groundstation)](https://pepy.tech/project/mypy-boto3-groundstation)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GroundStation 1.33.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
+[boto3.GroundStation 1.34.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.20.3](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-groundstation docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_groundstation/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-groundstation-1.33.0/mypy_boto3_groundstation.egg-info/SOURCES.txt` & `mypy-boto3-groundstation-1.34.0/mypy_boto3_groundstation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-groundstation-1.33.0/setup.py` & `mypy-boto3-groundstation-1.34.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-groundstation",
-    version="1.33.0",
+    version="1.34.0",
     packages=["mypy_boto3_groundstation"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GroundStation 1.33.0 service generated with mypy-boto3-builder"
-        " 7.20.3"
+        "Type annotations for boto3.GroundStation 1.34.0 service generated with mypy-boto3-builder"
+        " 7.21.0"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

