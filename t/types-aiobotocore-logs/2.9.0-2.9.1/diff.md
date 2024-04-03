# Comparing `tmp/types-aiobotocore-logs-2.9.0.tar.gz` & `tmp/types-aiobotocore-logs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-logs-2.9.0.tar", last modified: Wed Dec 13 19:59:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-logs-2.9.1.tar", last modified: Thu Jan 18 01:21:09 2024, max compression
```

## Comparing `types-aiobotocore-logs-2.9.0.tar` & `types-aiobotocore-logs-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.081515 types-aiobotocore-logs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2023-12-13 19:59:47.081515 types-aiobotocore-logs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:47.081515 types-aiobotocore-logs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.081515 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58406 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    58402 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18321 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18305 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    52228 2023-12-13 19:49:27.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    52227 2023-12-13 19:49:25.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:24.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:47.081515 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 19:59:47.000000 types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.481212 types-aiobotocore-logs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-01-18 01:21:09.481212 types-aiobotocore-logs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:09.481212 types-aiobotocore-logs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.477212 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58428 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58425 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-01-18 01:11:11.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-01-18 01:11:11.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18328 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18313 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    52227 2024-01-18 01:11:12.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52227 2024-01-18 01:11:11.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:10.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:09.481212 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15084 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:21:09.000000 types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-logs-2.9.0/LICENSE` & `types-aiobotocore-logs-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-logs-2.9.0/PKG-INFO` & `types-aiobotocore-logs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-logs"></a>
 
 # types-aiobotocore-logs
 
 [![PyPI - types-aiobotocore-logs](https://img.shields.io/pypi/v/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-logs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-logs-2.9.0/README.md` & `types-aiobotocore-logs-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-logs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-logs-2.9.0/setup.py` & `types-aiobotocore-logs-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-logs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_logs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudWatchLogs 2.9.1 service generated with"
+        " mypy-boto3-builder 7.23.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
-        "Typing :: Typed",
+        "Typing :: Stubs Only",
     ],
     keywords="aiobotocore logs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_logs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__init__.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,14 @@
     FilterLogEventsPaginator,
     ListAnomaliesPaginator,
     ListLogAnomalyDetectorsPaginator,
 )
 
 Client = CloudWatchLogsClient
 
-
 __all__ = (
     "Client",
     "CloudWatchLogsClient",
     "DescribeDeliveriesPaginator",
     "DescribeDeliveryDestinationsPaginator",
     "DescribeDeliverySourcesPaginator",
     "DescribeDestinationsPaginator",
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__init__.pyi` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/__main__.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchLogs 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchLogs 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.9.0")
+    print("2.9.1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/client.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchLogsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -209,15 +208,15 @@
         *,
         logGroupName: str,
         fromTime: int,
         to: int,
         destination: str,
         taskName: str = ...,
         logStreamNamePrefix: str = ...,
-        destinationPrefix: str = ...
+        destinationPrefix: str = ...,
     ) -> CreateExportTaskResponseTypeDef:
         """
         Creates an export task so that you can efficiently export data from a log group
         to an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_export_task)
@@ -229,15 +228,15 @@
         *,
         logGroupArnList: Sequence[str],
         detectorName: str = ...,
         evaluationFrequency: EvaluationFrequencyType = ...,
         filterPattern: str = ...,
         kmsKeyId: str = ...,
         anomalyVisibilityTime: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLogAnomalyDetectorResponseTypeDef:
         """
         Creates an *anomaly detector* that regularly scans one or more log groups and
         look for patterns and anomalies in the
         logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_anomaly_detector)
@@ -246,15 +245,15 @@
 
     async def create_log_group(
         self,
         *,
         logGroupName: str,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
-        logGroupClass: LogGroupClassType = ...
+        logGroupClass: LogGroupClassType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log group with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_group)
         """
@@ -414,15 +413,15 @@
         """
 
     async def describe_account_policies(
         self,
         *,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         policyName: str = ...,
-        accountIdentifiers: Sequence[str] = ...
+        accountIdentifiers: Sequence[str] = ...,
     ) -> DescribeAccountPoliciesResponseTypeDef:
         """
         Returns a list of all CloudWatch Logs account policies in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_account_policies)
         """
@@ -470,15 +469,15 @@
 
     async def describe_export_tasks(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Lists the specified export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_export_tasks)
         """
@@ -488,15 +487,15 @@
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         includeLinkedAccounts: bool = ...,
-        logGroupClass: LogGroupClassType = ...
+        logGroupClass: LogGroupClassType = ...,
     ) -> DescribeLogGroupsResponseTypeDef:
         """
         Lists the specified log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_groups)
         """
@@ -506,15 +505,15 @@
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeLogStreamsResponseTypeDef:
         """
         Lists the log streams for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_streams)
         """
@@ -523,30 +522,30 @@
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         metricName: str = ...,
-        metricNamespace: str = ...
+        metricNamespace: str = ...,
     ) -> DescribeMetricFiltersResponseTypeDef:
         """
         Lists the specified metric filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_metric_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_metric_filters)
         """
 
     async def describe_queries(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeQueriesResponseTypeDef:
         """
         Returns a list of CloudWatch Logs Insights queries that are scheduled, running,
         or have been run recently in this
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_queries)
@@ -577,15 +576,15 @@
 
     async def describe_subscription_filters(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeSubscriptionFiltersResponseTypeDef:
         """
         Lists the subscription filters for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_subscription_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_subscription_filters)
         """
@@ -611,15 +610,15 @@
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         interleaved: bool = ...,
-        unmask: bool = ...
+        unmask: bool = ...,
     ) -> FilterLogEventsResponseTypeDef:
         """
         Lists log events from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.filter_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#filter_log_events)
         """
@@ -701,15 +700,15 @@
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         nextToken: str = ...,
         limit: int = ...,
         startFromHead: bool = ...,
-        unmask: bool = ...
+        unmask: bool = ...,
     ) -> GetLogEventsResponseTypeDef:
         """
         Lists log events from the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_events)
         """
@@ -746,15 +745,15 @@
 
     async def list_anomalies(
         self,
         *,
         anomalyDetectorArn: str = ...,
         suppressionState: SuppressionStateType = ...,
         limit: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAnomaliesResponseTypeDef:
         """
         Returns a list of anomalies that log anomaly detectors have found.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_anomalies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_anomalies)
         """
@@ -789,15 +788,15 @@
 
     async def put_account_policy(
         self,
         *,
         policyName: str,
         policyDocument: str,
         policyType: Literal["DATA_PROTECTION_POLICY"],
-        scope: Literal["ALL"] = ...
+        scope: Literal["ALL"] = ...,
     ) -> PutAccountPolicyResponseTypeDef:
         """
         Creates an account-level data protection policy that applies to all log groups
         in the
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
@@ -816,15 +815,15 @@
 
     async def put_delivery_destination(
         self,
         *,
         name: str,
         deliveryDestinationConfiguration: DeliveryDestinationConfigurationTypeDef,
         outputFormat: OutputFormatType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutDeliveryDestinationResponseTypeDef:
         """
         Creates or updates a logical *delivery destination*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_delivery_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_delivery_destination)
         """
@@ -873,30 +872,30 @@
 
     async def put_log_events(
         self,
         *,
         logGroupName: str,
         logStreamName: str,
         logEvents: Sequence[InputLogEventTypeDef],
-        sequenceToken: str = ...
+        sequenceToken: str = ...,
     ) -> PutLogEventsResponseTypeDef:
         """
         Uploads a batch of log events to the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_log_events)
         """
 
     async def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationTypeDef]
+        metricTransformations: Sequence[MetricTransformationTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_metric_filter)
@@ -905,15 +904,15 @@
     async def put_query_definition(
         self,
         *,
         name: str,
         queryString: str,
         queryDefinitionId: str = ...,
         logGroupNames: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> PutQueryDefinitionResponseTypeDef:
         """
         Creates or updates a query definition for CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_query_definition)
         """
@@ -944,15 +943,15 @@
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
         destinationArn: str,
         roleArn: str = ...,
-        distribution: DistributionType = ...
+        distribution: DistributionType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a subscription filter and associates it with the specified
         log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_subscription_filter)
@@ -961,15 +960,15 @@
 
     async def start_live_tail(
         self,
         *,
         logGroupIdentifiers: Sequence[str],
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefixes: Sequence[str] = ...,
-        logEventFilterPattern: str = ...
+        logEventFilterPattern: str = ...,
     ) -> StartLiveTailResponseTypeDef:
         """
         Starts a Live Tail streaming session for one or more log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_live_tail)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_live_tail)
         """
@@ -979,15 +978,15 @@
         *,
         startTime: int,
         endTime: int,
         queryString: str,
         logGroupName: str = ...,
         logGroupNames: Sequence[str] = ...,
         logGroupIdentifiers: Sequence[str] = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> StartQueryResponseTypeDef:
         """
         Schedules a query of a log group using CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_query)
         """
@@ -1055,15 +1054,15 @@
     async def update_anomaly(
         self,
         *,
         anomalyDetectorArn: str,
         anomalyId: str = ...,
         patternId: str = ...,
         suppressionType: SuppressionTypeType = ...,
-        suppressionPeriod: SuppressionPeriodTypeDef = ...
+        suppressionPeriod: SuppressionPeriodTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Use this operation to *suppress* anomaly detection for a specified anomaly or
         pattern.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_anomaly)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#update_anomaly)
@@ -1072,15 +1071,15 @@
     async def update_log_anomaly_detector(
         self,
         *,
         anomalyDetectorArn: str,
         enabled: bool,
         evaluationFrequency: EvaluationFrequencyType = ...,
         filterPattern: str = ...,
-        anomalyVisibilityTime: int = ...
+        anomalyVisibilityTime: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing log anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_log_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#update_log_anomaly_detector)
         """
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/client.pyi` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
         *,
         logGroupName: str,
         fromTime: int,
         to: int,
         destination: str,
         taskName: str = ...,
         logStreamNamePrefix: str = ...,
-        destinationPrefix: str = ...
+        destinationPrefix: str = ...,
     ) -> CreateExportTaskResponseTypeDef:
         """
         Creates an export task so that you can efficiently export data from a log group
         to an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_export_task)
@@ -225,15 +225,15 @@
         *,
         logGroupArnList: Sequence[str],
         detectorName: str = ...,
         evaluationFrequency: EvaluationFrequencyType = ...,
         filterPattern: str = ...,
         kmsKeyId: str = ...,
         anomalyVisibilityTime: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateLogAnomalyDetectorResponseTypeDef:
         """
         Creates an *anomaly detector* that regularly scans one or more log groups and
         look for patterns and anomalies in the
         logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_anomaly_detector)
@@ -242,15 +242,15 @@
 
     async def create_log_group(
         self,
         *,
         logGroupName: str,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
-        logGroupClass: LogGroupClassType = ...
+        logGroupClass: LogGroupClassType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a log group with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.create_log_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#create_log_group)
         """
@@ -410,15 +410,15 @@
         """
 
     async def describe_account_policies(
         self,
         *,
         policyType: Literal["DATA_PROTECTION_POLICY"],
         policyName: str = ...,
-        accountIdentifiers: Sequence[str] = ...
+        accountIdentifiers: Sequence[str] = ...,
     ) -> DescribeAccountPoliciesResponseTypeDef:
         """
         Returns a list of all CloudWatch Logs account policies in the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_account_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_account_policies)
         """
@@ -466,15 +466,15 @@
 
     async def describe_export_tasks(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Lists the specified export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_export_tasks)
         """
@@ -484,15 +484,15 @@
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         includeLinkedAccounts: bool = ...,
-        logGroupClass: LogGroupClassType = ...
+        logGroupClass: LogGroupClassType = ...,
     ) -> DescribeLogGroupsResponseTypeDef:
         """
         Lists the specified log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_groups)
         """
@@ -502,15 +502,15 @@
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeLogStreamsResponseTypeDef:
         """
         Lists the log streams for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_log_streams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_log_streams)
         """
@@ -519,30 +519,30 @@
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         metricName: str = ...,
-        metricNamespace: str = ...
+        metricNamespace: str = ...,
     ) -> DescribeMetricFiltersResponseTypeDef:
         """
         Lists the specified metric filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_metric_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_metric_filters)
         """
 
     async def describe_queries(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeQueriesResponseTypeDef:
         """
         Returns a list of CloudWatch Logs Insights queries that are scheduled, running,
         or have been run recently in this
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_queries)
@@ -573,15 +573,15 @@
 
     async def describe_subscription_filters(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
         nextToken: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> DescribeSubscriptionFiltersResponseTypeDef:
         """
         Lists the subscription filters for the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.describe_subscription_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#describe_subscription_filters)
         """
@@ -607,15 +607,15 @@
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         nextToken: str = ...,
         limit: int = ...,
         interleaved: bool = ...,
-        unmask: bool = ...
+        unmask: bool = ...,
     ) -> FilterLogEventsResponseTypeDef:
         """
         Lists log events from the specified log group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.filter_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#filter_log_events)
         """
@@ -697,15 +697,15 @@
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         nextToken: str = ...,
         limit: int = ...,
         startFromHead: bool = ...,
-        unmask: bool = ...
+        unmask: bool = ...,
     ) -> GetLogEventsResponseTypeDef:
         """
         Lists log events from the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.get_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#get_log_events)
         """
@@ -742,15 +742,15 @@
 
     async def list_anomalies(
         self,
         *,
         anomalyDetectorArn: str = ...,
         suppressionState: SuppressionStateType = ...,
         limit: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListAnomaliesResponseTypeDef:
         """
         Returns a list of anomalies that log anomaly detectors have found.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.list_anomalies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#list_anomalies)
         """
@@ -785,15 +785,15 @@
 
     async def put_account_policy(
         self,
         *,
         policyName: str,
         policyDocument: str,
         policyType: Literal["DATA_PROTECTION_POLICY"],
-        scope: Literal["ALL"] = ...
+        scope: Literal["ALL"] = ...,
     ) -> PutAccountPolicyResponseTypeDef:
         """
         Creates an account-level data protection policy that applies to all log groups
         in the
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_account_policy)
@@ -812,15 +812,15 @@
 
     async def put_delivery_destination(
         self,
         *,
         name: str,
         deliveryDestinationConfiguration: DeliveryDestinationConfigurationTypeDef,
         outputFormat: OutputFormatType = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> PutDeliveryDestinationResponseTypeDef:
         """
         Creates or updates a logical *delivery destination*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_delivery_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_delivery_destination)
         """
@@ -869,30 +869,30 @@
 
     async def put_log_events(
         self,
         *,
         logGroupName: str,
         logStreamName: str,
         logEvents: Sequence[InputLogEventTypeDef],
-        sequenceToken: str = ...
+        sequenceToken: str = ...,
     ) -> PutLogEventsResponseTypeDef:
         """
         Uploads a batch of log events to the specified log stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_log_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_log_events)
         """
 
     async def put_metric_filter(
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
-        metricTransformations: Sequence[MetricTransformationTypeDef]
+        metricTransformations: Sequence[MetricTransformationTypeDef],
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a metric filter and associates it with the specified log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_metric_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_metric_filter)
@@ -901,15 +901,15 @@
     async def put_query_definition(
         self,
         *,
         name: str,
         queryString: str,
         queryDefinitionId: str = ...,
         logGroupNames: Sequence[str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> PutQueryDefinitionResponseTypeDef:
         """
         Creates or updates a query definition for CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_query_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#put_query_definition)
         """
@@ -940,15 +940,15 @@
         self,
         *,
         logGroupName: str,
         filterName: str,
         filterPattern: str,
         destinationArn: str,
         roleArn: str = ...,
-        distribution: DistributionType = ...
+        distribution: DistributionType = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates a subscription filter and associates it with the specified
         log
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.put_subscription_filter)
@@ -957,15 +957,15 @@
 
     async def start_live_tail(
         self,
         *,
         logGroupIdentifiers: Sequence[str],
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefixes: Sequence[str] = ...,
-        logEventFilterPattern: str = ...
+        logEventFilterPattern: str = ...,
     ) -> StartLiveTailResponseTypeDef:
         """
         Starts a Live Tail streaming session for one or more log groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_live_tail)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_live_tail)
         """
@@ -975,15 +975,15 @@
         *,
         startTime: int,
         endTime: int,
         queryString: str,
         logGroupName: str = ...,
         logGroupNames: Sequence[str] = ...,
         logGroupIdentifiers: Sequence[str] = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> StartQueryResponseTypeDef:
         """
         Schedules a query of a log group using CloudWatch Logs Insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.start_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#start_query)
         """
@@ -1051,15 +1051,15 @@
     async def update_anomaly(
         self,
         *,
         anomalyDetectorArn: str,
         anomalyId: str = ...,
         patternId: str = ...,
         suppressionType: SuppressionTypeType = ...,
-        suppressionPeriod: SuppressionPeriodTypeDef = ...
+        suppressionPeriod: SuppressionPeriodTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Use this operation to *suppress* anomaly detection for a specified anomaly or
         pattern.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_anomaly)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#update_anomaly)
@@ -1068,15 +1068,15 @@
     async def update_log_anomaly_detector(
         self,
         *,
         anomalyDetectorArn: str,
         enabled: bool,
         evaluationFrequency: EvaluationFrequencyType = ...,
         filterPattern: str = ...,
-        anomalyVisibilityTime: int = ...
+        anomalyVisibilityTime: int = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates an existing log anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Client.update_log_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/client/#update_log_anomaly_detector)
         """
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/literals.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AnomalyDetectorStatusType",
     "DataProtectionStatusType",
     "DeliveryDestinationTypeType",
     "DescribeDeliveriesPaginatorName",
     "DescribeDeliveryDestinationsPaginatorName",
     "DescribeDeliverySourcesPaginatorName",
@@ -56,15 +55,14 @@
     "CloudWatchLogsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnomalyDetectorStatusType = Literal[
     "ANALYZING", "DELETED", "FAILED", "INITIALIZING", "PAUSED", "TRAINING"
 ]
 DataProtectionStatusType = Literal["ACTIVATED", "ARCHIVED", "DELETED", "DISABLED"]
 DeliveryDestinationTypeType = Literal["CWL", "FH", "S3"]
 DescribeDeliveriesPaginatorName = Literal["describe_deliveries"]
 DescribeDeliveryDestinationsPaginatorName = Literal["describe_delivery_destinations"]
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/literals.pyi` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/paginator.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,14 @@
     "DescribeResourcePoliciesPaginator",
     "DescribeSubscriptionFiltersPaginator",
     "FilterLogEventsPaginator",
     "ListAnomaliesPaginator",
     "ListLogAnomalyDetectorsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -172,15 +171,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -194,15 +193,15 @@
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
         logGroupClass: LogGroupClassType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describeloggroupspaginator)
         """
 
 
@@ -216,15 +215,15 @@
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describelogstreamspaginator)
         """
 
 
@@ -237,15 +236,15 @@
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describemetricfilterspaginator)
         """
 
 
@@ -256,15 +255,15 @@
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describequeriespaginator)
         """
 
 
@@ -290,15 +289,15 @@
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
 
@@ -316,15 +315,15 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#filterlogeventspaginator)
         """
 
 
@@ -335,15 +334,15 @@
     """
 
     def paginate(
         self,
         *,
         anomalyDetectorArn: str = ...,
         suppressionState: SuppressionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnomaliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.ListAnomalies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#listanomaliespaginator)
         """
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/paginator.pyi` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str = ...,
         statusCode: ExportTaskStatusCodeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeLogGroupsPaginator(AioPaginator):
@@ -186,15 +186,15 @@
         self,
         *,
         accountIdentifiers: Sequence[str] = ...,
         logGroupNamePrefix: str = ...,
         logGroupNamePattern: str = ...,
         includeLinkedAccounts: bool = ...,
         logGroupClass: LogGroupClassType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describeloggroupspaginator)
         """
 
 class DescribeLogStreamsPaginator(AioPaginator):
@@ -207,15 +207,15 @@
         self,
         *,
         logGroupName: str = ...,
         logGroupIdentifier: str = ...,
         logStreamNamePrefix: str = ...,
         orderBy: OrderByType = ...,
         descending: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeLogStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeLogStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describelogstreamspaginator)
         """
 
 class DescribeMetricFiltersPaginator(AioPaginator):
@@ -227,15 +227,15 @@
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         filterNamePrefix: str = ...,
         metricName: str = ...,
         metricNamespace: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMetricFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeMetricFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describemetricfilterspaginator)
         """
 
 class DescribeQueriesPaginator(AioPaginator):
@@ -245,15 +245,15 @@
     """
 
     def paginate(
         self,
         *,
         logGroupName: str = ...,
         status: QueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describequeriespaginator)
         """
 
 class DescribeResourcePoliciesPaginator(AioPaginator):
@@ -277,15 +277,15 @@
     """
 
     def paginate(
         self,
         *,
         logGroupName: str,
         filterNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubscriptionFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#describesubscriptionfilterspaginator)
         """
 
 class FilterLogEventsPaginator(AioPaginator):
@@ -302,15 +302,15 @@
         logStreamNames: Sequence[str] = ...,
         logStreamNamePrefix: str = ...,
         startTime: int = ...,
         endTime: int = ...,
         filterPattern: str = ...,
         interleaved: bool = ...,
         unmask: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[FilterLogEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.FilterLogEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#filterlogeventspaginator)
         """
 
 class ListAnomaliesPaginator(AioPaginator):
@@ -320,15 +320,15 @@
     """
 
     def paginate(
         self,
         *,
         anomalyDetectorArn: str = ...,
         suppressionState: SuppressionStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAnomaliesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs.Paginator.ListAnomalies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/paginators/#listanomaliespaginator)
         """
 
 class ListLogAnomalyDetectorsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/type_defs.py` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountPolicyTypeDef",
     "AnomalyDetectorTypeDef",
     "PatternTokenTypeDef",
     "AssociateKmsKeyRequestRequestTypeDef",
     "CancelExportTaskRequestRequestTypeDef",
     "CreateDeliveryRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs/type_defs.pyi` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/PKG-INFO` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-logs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchLogs 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchLogs 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -13,50 +13,50 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
+Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: typing-extensions>=4.1.0; python_version < "3.12"
 
 <a id="types-aiobotocore-logs"></a>
 
 # types-aiobotocore-logs
 
 [![PyPI - types-aiobotocore-logs](https://img.shields.io/pypi/v/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-logs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-logs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-logs)](https://pepy.tech/project/types-aiobotocore-logs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchLogs 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
+[aiobotocore.CloudWatchLogs 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#CloudWatchLogs)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-logs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_logs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-logs-2.9.0/types_aiobotocore_logs.egg-info/SOURCES.txt` & `types-aiobotocore-logs-2.9.1/types_aiobotocore_logs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

