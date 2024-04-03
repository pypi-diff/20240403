# Comparing `tmp/types-aiobotocore-iotevents-2.9.0.tar.gz` & `tmp/types-aiobotocore-iotevents-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-2.9.0.tar", last modified: Wed Dec 13 19:59:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-2.9.1.tar", last modified: Thu Jan 18 01:20:56 2024, max compression
```

## Comparing `types-aiobotocore-iotevents-2.9.0.tar` & `types-aiobotocore-iotevents-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.265644 types-aiobotocore-iotevents-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2023-12-13 19:59:33.265644 types-aiobotocore-iotevents-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10784 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:33.265644 types-aiobotocore-iotevents-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.265644 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20392 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20389 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9322 2023-12-13 19:47:55.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30136 2023-12-13 19:47:57.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30135 2023-12-13 19:47:55.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:54.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:33.265644 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:33.000000 types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.709269 types-aiobotocore-iotevents-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-01-18 01:20:56.709269 types-aiobotocore-iotevents-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10784 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:56.709269 types-aiobotocore-iotevents-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.709269 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20396 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30135 2024-01-18 01:09:46.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30135 2024-01-18 01:09:46.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:45.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:56.709269 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12375 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:56.000000 types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-2.9.0/LICENSE` & `types-aiobotocore-iotevents-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-iotevents-2.9.0/PKG-INFO` & `types-aiobotocore-iotevents-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTEvents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTEvents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
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
 
 <a id="types-aiobotocore-iotevents"></a>
 
 # types-aiobotocore-iotevents
 
 [![PyPI - types-aiobotocore-iotevents](https://img.shields.io/pypi/v/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotevents-2.9.0/README.md` & `types-aiobotocore-iotevents-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotevents-2.9.0/setup.py` & `types-aiobotocore-iotevents-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.IoTEvents 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.IoTEvents 2.9.1 service generated with mypy-boto3-builder"
+        " 7.23.1"
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
     keywords="aiobotocore iotevents type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotevents": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/__main__.py` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTEvents 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.IoTEvents 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/client.py` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,36 +52,33 @@
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
 __all__ = ("IoTEventsClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class IoTEventsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
     """
 
     meta: ClientMeta
@@ -119,15 +116,15 @@
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
         alarmNotification: AlarmNotificationTypeDef = ...,
         alarmEventActions: AlarmEventActionsTypeDef = ...,
-        alarmCapabilities: AlarmCapabilitiesTypeDef = ...
+        alarmCapabilities: AlarmCapabilitiesTypeDef = ...,
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
@@ -137,30 +134,30 @@
         *,
         detectorModelName: str,
         detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        evaluationMethod: EvaluationMethodType = ...
+        evaluationMethod: EvaluationMethodType = ...,
     ) -> CreateDetectorModelResponseTypeDef:
         """
         Creates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
 
     async def create_input(
         self,
         *,
         inputName: str,
         inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_input)
         """
@@ -300,15 +297,15 @@
         """
 
     async def list_input_routings(
         self,
         *,
         inputIdentifier: InputIdentifierTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListInputRoutingsResponseTypeDef:
         """
         Lists one or more input routings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_input_routings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_input_routings)
         """
@@ -375,15 +372,15 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
         alarmNotification: AlarmNotificationTypeDef = ...,
         alarmEventActions: AlarmEventActionsTypeDef = ...,
-        alarmCapabilities: AlarmCapabilitiesTypeDef = ...
+        alarmCapabilities: AlarmCapabilitiesTypeDef = ...,
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
@@ -391,29 +388,29 @@
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
         detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
-        evaluationMethod: EvaluationMethodType = ...
+        evaluationMethod: EvaluationMethodType = ...,
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
 
     async def update_input(
         self,
         *,
         inputName: str,
         inputDefinition: InputDefinitionTypeDef,
-        inputDescription: str = ...
+        inputDescription: str = ...,
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
         """
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/client.pyi` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,33 +52,36 @@
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
 __all__ = ("IoTEventsClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InvalidRequestException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class IoTEventsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/)
     """
 
     meta: ClientMeta
@@ -116,15 +119,15 @@
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
         alarmNotification: AlarmNotificationTypeDef = ...,
         alarmEventActions: AlarmEventActionsTypeDef = ...,
-        alarmCapabilities: AlarmCapabilitiesTypeDef = ...
+        alarmCapabilities: AlarmCapabilitiesTypeDef = ...,
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
@@ -134,30 +137,30 @@
         *,
         detectorModelName: str,
         detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        evaluationMethod: EvaluationMethodType = ...
+        evaluationMethod: EvaluationMethodType = ...,
     ) -> CreateDetectorModelResponseTypeDef:
         """
         Creates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
 
     async def create_input(
         self,
         *,
         inputName: str,
         inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_input)
         """
@@ -297,15 +300,15 @@
         """
 
     async def list_input_routings(
         self,
         *,
         inputIdentifier: InputIdentifierTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListInputRoutingsResponseTypeDef:
         """
         Lists one or more input routings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_input_routings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_input_routings)
         """
@@ -372,15 +375,15 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
         alarmNotification: AlarmNotificationTypeDef = ...,
         alarmEventActions: AlarmEventActionsTypeDef = ...,
-        alarmCapabilities: AlarmCapabilitiesTypeDef = ...
+        alarmCapabilities: AlarmCapabilitiesTypeDef = ...,
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
@@ -388,29 +391,29 @@
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
         detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
-        evaluationMethod: EvaluationMethodType = ...
+        evaluationMethod: EvaluationMethodType = ...,
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
 
     async def update_input(
         self,
         *,
         inputName: str,
         inputDefinition: InputDefinitionTypeDef,
-        inputDescription: str = ...
+        inputDescription: str = ...,
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
         """
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/literals.py` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlarmModelVersionStatusType",
     "AnalysisResultLevelType",
     "AnalysisStatusType",
     "ComparisonOperatorType",
     "DetectorModelVersionStatusType",
     "EvaluationMethodType",
@@ -32,15 +31,14 @@
     "PayloadTypeType",
     "IoTEventsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AlarmModelVersionStatusType = Literal["ACTIVATING", "ACTIVE", "FAILED", "INACTIVE"]
 AnalysisResultLevelType = Literal["ERROR", "INFO", "WARNING"]
 AnalysisStatusType = Literal["COMPLETE", "FAILED", "RUNNING"]
 ComparisonOperatorType = Literal[
     "EQUAL", "GREATER", "GREATER_OR_EQUAL", "LESS", "LESS_OR_EQUAL", "NOT_EQUAL"
 ]
 DetectorModelVersionStatusType = Literal[
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/literals.pyi` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/type_defs.py` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcknowledgeFlowTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
     "InitializationConfigurationTypeDef",
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents/type_defs.pyi` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/PKG-INFO` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotevents
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.IoTEvents 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.IoTEvents 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/
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
 
 <a id="types-aiobotocore-iotevents"></a>
 
 # types-aiobotocore-iotevents
 
 [![PyPI - types-aiobotocore-iotevents](https://img.shields.io/pypi/v/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotevents.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotevents)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotevents)](https://pepy.tech/project/types-aiobotocore-iotevents)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.IoTEvents 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
+[aiobotocore.IoTEvents 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents)
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
 [types-aiobotocore-iotevents docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-iotevents-2.9.0/types_aiobotocore_iotevents.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-2.9.1/types_aiobotocore_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

