# Comparing `tmp/types-aiobotocore-rum-2.9.0.tar.gz` & `tmp/types-aiobotocore-rum-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rum-2.9.0.tar", last modified: Wed Dec 13 20:00:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-rum-2.9.1.tar", last modified: Thu Jan 18 01:21:41 2024, max compression
```

## Comparing `types-aiobotocore-rum-2.9.0.tar` & `types-aiobotocore-rum-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.253208 types-aiobotocore-rum-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-12-13 20:00:22.253208 types-aiobotocore-rum-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11902 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:22.253208 types-aiobotocore-rum-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-13 19:54:59.000000 types-aiobotocore-rum-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.253208 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18109 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9360 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9358 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15022 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:00.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:22.253208 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13459 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:22.000000 types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.397068 types-aiobotocore-rum-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-01-18 01:21:41.397068 types-aiobotocore-rum-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11902 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:41.397068 types-aiobotocore-rum-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.397068 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18121 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18118 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-01-18 01:16:34.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-01-18 01:16:34.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-01-18 01:16:34.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15022 2024-01-18 01:16:34.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:33.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:41.397068 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13479 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:41.000000 types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rum-2.9.0/LICENSE` & `types-aiobotocore-rum-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rum-2.9.0/PKG-INFO` & `types-aiobotocore-rum-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
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
 
 <a id="types-aiobotocore-rum"></a>
 
 # types-aiobotocore-rum
 
 [![PyPI - types-aiobotocore-rum](https://img.shields.io/pypi/v/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [types-aiobotocore-rum docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rum-2.9.0/README.md` & `types-aiobotocore-rum-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [types-aiobotocore-rum docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rum-2.9.0/setup.py` & `types-aiobotocore-rum-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rum",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudWatchRUM 2.9.1 service generated with"
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
     keywords="aiobotocore rum type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rum": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__init__.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     GetAppMonitorDataPaginator,
     ListAppMonitorsPaginator,
     ListRumMetricsDestinationsPaginator,
 )
 
 Client = CloudWatchRUMClient
 
-
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "Client",
     "CloudWatchRUMClient",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__init__.pyi` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/__main__.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatchRUM 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatchRUM 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/client.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudWatchRUMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -95,15 +94,15 @@
 
     async def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch
         RUM app monitor to send to a
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -112,15 +111,15 @@
 
     async def batch_delete_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinitionIds: Sequence[str],
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> BatchDeleteRumMetricDefinitionsResponseTypeDef:
         """
         Removes the specified metrics from being sent to an extended metrics
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_delete_rum_metric_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#batch_delete_rum_metric_definitions)
@@ -129,15 +128,15 @@
     async def batch_get_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> BatchGetRumMetricDefinitionsResponseTypeDef:
         """
         Retrieves the list of metrics and dimensions that a RUM app monitor is sending
         to a single
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_get_rum_metric_definitions)
@@ -164,15 +163,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.create_app_monitor)
@@ -224,15 +223,15 @@
     async def get_app_monitor_data(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAppMonitorDataResponseTypeDef:
         """
         Retrieves the raw performance events that RUM has collected from your web
         application, so that you can do your own processing or analysis of this
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.get_app_monitor_data)
@@ -274,15 +273,15 @@
     async def put_rum_events(
         self,
         *,
         AppMonitorDetails: AppMonitorDetailsTypeDef,
         BatchId: str,
         Id: str,
         RumEvents: Sequence[RumEventTypeDef],
-        UserDetails: UserDetailsTypeDef
+        UserDetails: UserDetailsTypeDef,
     ) -> Dict[str, Any]:
         """
         Sends telemetry events about your application performance and user behavior to
         CloudWatch
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.put_rum_events)
@@ -291,15 +290,15 @@
 
     async def put_rum_metrics_destination(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        IamRoleArn: str = ...
+        IamRoleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a destination to receive extended metrics from CloudWatch
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.put_rum_metrics_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#put_rum_metrics_destination)
@@ -325,15 +324,15 @@
     async def update_app_monitor(
         self,
         *,
         Name: str,
         AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_app_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#update_app_monitor)
         """
@@ -341,15 +340,15 @@
     async def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinition: MetricDefinitionRequestTypeDef,
         MetricDefinitionId: str,
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#update_rum_metric_definition)
         """
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/client.pyi` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 
     async def batch_create_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinitions: Sequence[MetricDefinitionRequestTypeDef],
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> BatchCreateRumMetricDefinitionsResponseTypeDef:
         """
         Specifies the extended metrics and custom metrics that you want a CloudWatch
         RUM app monitor to send to a
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_create_rum_metric_definitions)
@@ -108,15 +108,15 @@
 
     async def batch_delete_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinitionIds: Sequence[str],
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> BatchDeleteRumMetricDefinitionsResponseTypeDef:
         """
         Removes the specified metrics from being sent to an extended metrics
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_delete_rum_metric_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#batch_delete_rum_metric_definitions)
@@ -125,15 +125,15 @@
     async def batch_get_rum_metric_definitions(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> BatchGetRumMetricDefinitionsResponseTypeDef:
         """
         Retrieves the list of metrics and dimensions that a RUM app monitor is sending
         to a single
         destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.batch_get_rum_metric_definitions)
@@ -160,15 +160,15 @@
         self,
         *,
         Domain: str,
         Name: str,
         AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAppMonitorResponseTypeDef:
         """
         Creates a Amazon CloudWatch RUM app monitor, which collects telemetry data from
         your application and sends that data to
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.create_app_monitor)
@@ -220,15 +220,15 @@
     async def get_app_monitor_data(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> GetAppMonitorDataResponseTypeDef:
         """
         Retrieves the raw performance events that RUM has collected from your web
         application, so that you can do your own processing or analysis of this
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.get_app_monitor_data)
@@ -270,15 +270,15 @@
     async def put_rum_events(
         self,
         *,
         AppMonitorDetails: AppMonitorDetailsTypeDef,
         BatchId: str,
         Id: str,
         RumEvents: Sequence[RumEventTypeDef],
-        UserDetails: UserDetailsTypeDef
+        UserDetails: UserDetailsTypeDef,
     ) -> Dict[str, Any]:
         """
         Sends telemetry events about your application performance and user behavior to
         CloudWatch
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.put_rum_events)
@@ -287,15 +287,15 @@
 
     async def put_rum_metrics_destination(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        IamRoleArn: str = ...
+        IamRoleArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Creates or updates a destination to receive extended metrics from CloudWatch
         RUM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.put_rum_metrics_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#put_rum_metrics_destination)
@@ -321,15 +321,15 @@
     async def update_app_monitor(
         self,
         *,
         Name: str,
         AppMonitorConfiguration: AppMonitorConfigurationTypeDef = ...,
         CustomEvents: CustomEventsTypeDef = ...,
         CwLogEnabled: bool = ...,
-        Domain: str = ...
+        Domain: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of an existing app monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_app_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#update_app_monitor)
         """
@@ -337,15 +337,15 @@
     async def update_rum_metric_definition(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         MetricDefinition: MetricDefinitionRequestTypeDef,
         MetricDefinitionId: str,
-        DestinationArn: str = ...
+        DestinationArn: str = ...,
     ) -> Dict[str, Any]:
         """
         Modifies one existing metric definition for CloudWatch RUM extended metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Client.update_rum_metric_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/client/#update_rum_metric_definition)
         """
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/literals.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/literals.py`

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
     "BatchGetRumMetricDefinitionsPaginatorName",
     "CustomEventsStatusType",
     "GetAppMonitorDataPaginatorName",
     "ListAppMonitorsPaginatorName",
     "ListRumMetricsDestinationsPaginatorName",
     "MetricDestinationType",
@@ -32,15 +31,14 @@
     "CloudWatchRUMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchGetRumMetricDefinitionsPaginatorName = Literal["batch_get_rum_metric_definitions"]
 CustomEventsStatusType = Literal["DISABLED", "ENABLED"]
 GetAppMonitorDataPaginatorName = Literal["get_app_monitor_data"]
 ListAppMonitorsPaginatorName = Literal["list_app_monitors"]
 ListRumMetricsDestinationsPaginatorName = Literal["list_rum_metrics_destinations"]
 MetricDestinationType = Literal["CloudWatch", "Evidently"]
 StateEnumType = Literal["ACTIVE", "CREATED", "DELETING"]
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/literals.pyi` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/paginator.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 __all__ = (
     "BatchGetRumMetricDefinitionsPaginator",
     "GetAppMonitorDataPaginator",
     "ListAppMonitorsPaginator",
     "ListRumMetricsDestinationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -69,15 +68,15 @@
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
 
@@ -89,15 +88,15 @@
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/paginators/#getappmonitordatapaginator)
         """
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/paginator.pyi` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     def paginate(
         self,
         *,
         AppMonitorName: str,
         Destination: MetricDestinationType,
         DestinationArn: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[BatchGetRumMetricDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.BatchGetRumMetricDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/paginators/#batchgetrummetricdefinitionspaginator)
         """
 
 class GetAppMonitorDataPaginator(AioPaginator):
@@ -85,15 +85,15 @@
 
     def paginate(
         self,
         *,
         Name: str,
         TimeRange: TimeRangeTypeDef,
         Filters: Sequence[QueryFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAppMonitorDataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM.Paginator.GetAppMonitorData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/paginators/#getappmonitordatapaginator)
         """
 
 class ListAppMonitorsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/type_defs.py` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
     "CustomEventsTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum/type_defs.pyi` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/PKG-INFO` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rum
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudWatchRUM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudWatchRUM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/
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
 
 <a id="types-aiobotocore-rum"></a>
 
 # types-aiobotocore-rum
 
 [![PyPI - types-aiobotocore-rum](https://img.shields.io/pypi/v/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rum.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rum)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rum)](https://pepy.tech/project/types-aiobotocore-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudWatchRUM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[aiobotocore.CloudWatchRUM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [types-aiobotocore-rum docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rum/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rum-2.9.0/types_aiobotocore_rum.egg-info/SOURCES.txt` & `types-aiobotocore-rum-2.9.1/types_aiobotocore_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

