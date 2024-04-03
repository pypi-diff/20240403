# Comparing `tmp/types-aiobotocore-scheduler-2.9.0.tar.gz` & `tmp/types-aiobotocore-scheduler-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-scheduler-2.9.0.tar", last modified: Wed Dec 13 20:00:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-scheduler-2.9.1.tar", last modified: Thu Jan 18 01:21:45 2024, max compression
```

## Comparing `types-aiobotocore-scheduler-2.9.0.tar` & `types-aiobotocore-scheduler-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.845168 types-aiobotocore-scheduler-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2023-12-13 20:00:26.845168 types-aiobotocore-scheduler-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11784 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:26.845168 types-aiobotocore-scheduler-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.845168 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13261 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9739 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13677 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13676 2023-12-13 19:55:49.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:48.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.845168 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:26.000000 types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.581049 types-aiobotocore-scheduler-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-01-18 01:21:45.581049 types-aiobotocore-scheduler-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11784 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:45.581049 types-aiobotocore-scheduler-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.577049 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13263 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13260 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-01-18 01:17:20.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-01-18 01:17:20.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-01-18 01:17:20.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13676 2024-01-18 01:17:20.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:19.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.577049 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13386 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:45.000000 types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-scheduler-2.9.0/LICENSE` & `types-aiobotocore-scheduler-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-scheduler-2.9.0/PKG-INFO` & `types-aiobotocore-scheduler-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
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
 
 <a id="types-aiobotocore-scheduler"></a>
 
 # types-aiobotocore-scheduler
 
 [![PyPI - types-aiobotocore-scheduler](https://img.shields.io/pypi/v/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-scheduler-2.9.0/README.md` & `types-aiobotocore-scheduler-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-scheduler-2.9.0/setup.py` & `types-aiobotocore-scheduler-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-scheduler",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_scheduler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.9.1 service generated with"
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
     keywords="aiobotocore scheduler type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_scheduler": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__init__.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import EventBridgeSchedulerClient
 from .paginator import ListScheduleGroupsPaginator, ListSchedulesPaginator
 
 Client = EventBridgeSchedulerClient
 
-
 __all__ = (
     "Client",
     "EventBridgeSchedulerClient",
     "ListScheduleGroupsPaginator",
     "ListSchedulesPaginator",
 )
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__init__.pyi` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/__main__.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridgeScheduler 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EventBridgeScheduler 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler\nOther"
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

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/client.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EventBridgeSchedulerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -109,15 +108,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#create_schedule)
         """
@@ -193,15 +192,15 @@
     async def list_schedules(
         self,
         *,
         GroupName: str = ...,
         MaxResults: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> ListSchedulesOutputTypeDef:
         """
         Returns a paginated list of your EventBridge Scheduler schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#list_schedules)
         """
@@ -244,15 +243,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#update_schedule)
         """
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/client.pyi` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> CreateScheduleOutputTypeDef:
         """
         Creates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.create_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#create_schedule)
         """
@@ -189,15 +189,15 @@
     async def list_schedules(
         self,
         *,
         GroupName: str = ...,
         MaxResults: int = ...,
         NamePrefix: str = ...,
         NextToken: str = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> ListSchedulesOutputTypeDef:
         """
         Returns a paginated list of your EventBridge Scheduler schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.list_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#list_schedules)
         """
@@ -240,15 +240,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         EndDate: TimestampTypeDef = ...,
         GroupName: str = ...,
         KmsKeyArn: str = ...,
         ScheduleExpressionTimezone: str = ...,
         StartDate: TimestampTypeDef = ...,
-        State: ScheduleStateType = ...
+        State: ScheduleStateType = ...,
     ) -> UpdateScheduleOutputTypeDef:
         """
         Updates the specified schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Client.update_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/client/#update_schedule)
         """
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/literals.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/literals.py`

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
     "ActionAfterCompletionType",
     "AssignPublicIpType",
     "FlexibleTimeWindowModeType",
     "LaunchTypeType",
     "ListScheduleGroupsPaginatorName",
     "ListSchedulesPaginatorName",
@@ -35,15 +34,14 @@
     "EventBridgeSchedulerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionAfterCompletionType = Literal["DELETE", "NONE"]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 FlexibleTimeWindowModeType = Literal["FLEXIBLE", "OFF"]
 LaunchTypeType = Literal["EC2", "EXTERNAL", "FARGATE"]
 ListScheduleGroupsPaginatorName = Literal["list_schedule_groups"]
 ListSchedulesPaginatorName = Literal["list_schedules"]
 PlacementConstraintTypeType = Literal["distinctInstance", "memberOf"]
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/literals.pyi` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/paginator.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListScheduleGroupsOutputTypeDef,
     ListSchedulesOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListScheduleGroupsPaginator", "ListSchedulesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -71,13 +70,13 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/paginator.pyi` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -67,13 +67,13 @@
 
     def paginate(
         self,
         *,
         GroupName: str = ...,
         NamePrefix: str = ...,
         State: ScheduleStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchedulesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler.Paginator.ListSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/paginators/#listschedulespaginator)
         """
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/type_defs.py` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AwsVpcConfigurationTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "FlexibleTimeWindowTypeDef",
     "TimestampTypeDef",
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler/type_defs.pyi` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/PKG-INFO` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-scheduler
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EventBridgeScheduler 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/
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
 
 <a id="types-aiobotocore-scheduler"></a>
 
 # types-aiobotocore-scheduler
 
 [![PyPI - types-aiobotocore-scheduler](https://img.shields.io/pypi/v/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-scheduler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-scheduler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-scheduler)](https://pepy.tech/project/types-aiobotocore-scheduler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridgeScheduler 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
+[aiobotocore.EventBridgeScheduler 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#EventBridgeScheduler)
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
 [types-aiobotocore-scheduler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_scheduler/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-scheduler-2.9.0/types_aiobotocore_scheduler.egg-info/SOURCES.txt` & `types-aiobotocore-scheduler-2.9.1/types_aiobotocore_scheduler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

