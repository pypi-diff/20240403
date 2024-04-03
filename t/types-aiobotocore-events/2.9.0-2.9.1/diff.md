# Comparing `tmp/types-aiobotocore-events-2.9.0.tar.gz` & `tmp/types-aiobotocore-events-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-events-2.9.0.tar", last modified: Wed Dec 13 19:59:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-events-2.9.1.tar", last modified: Thu Jan 18 01:20:42 2024, max compression
```

## Comparing `types-aiobotocore-events-2.9.0.tar` & `types-aiobotocore-events-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.917747 types-aiobotocore-events-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13313 2023-12-13 19:59:17.917747 types-aiobotocore-events-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:17.917747 types-aiobotocore-events-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.917747 types-aiobotocore-events-2.9.0/types_aiobotocore_events/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40296 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40292 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10843 2023-12-13 19:46:05.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2023-12-13 19:46:05.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51348 2023-12-13 19:46:07.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51347 2023-12-13 19:46:06.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:04.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:17.917747 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13313 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:17.000000 types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.501334 types-aiobotocore-events-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-01-18 01:20:42.501334 types-aiobotocore-events-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:42.501334 types-aiobotocore-events-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.501334 types-aiobotocore-events-2.9.1/types_aiobotocore_events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40312 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40309 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-01-18 01:08:00.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51347 2024-01-18 01:08:01.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51347 2024-01-18 01:08:01.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:59.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:42.501334 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13333 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:42.000000 types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-events-2.9.0/LICENSE` & `types-aiobotocore-events-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-events-2.9.0/PKG-INFO` & `types-aiobotocore-events-2.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-events
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EventBridge 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EventBridge 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/
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
 
 <a id="types-aiobotocore-events"></a>
 
 # types-aiobotocore-events
 
 [![PyPI - types-aiobotocore-events](https://img.shields.io/pypi/v/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [types-aiobotocore-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-events-2.9.0/README.md` & `types-aiobotocore-events-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [types-aiobotocore-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-events-2.9.0/setup.py` & `types-aiobotocore-events-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-events",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EventBridge 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.EventBridge 2.9.1 service generated with"
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
     keywords="aiobotocore events type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_events": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/__init__.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListRuleNamesByTargetPaginator,
     ListRulesPaginator,
     ListTargetsByRulePaginator,
 )
 
 Client = EventBridgeClient
 
-
 __all__ = (
     "Client",
     "EventBridgeClient",
     "ListRuleNamesByTargetPaginator",
     "ListRulesPaginator",
     "ListTargetsByRulePaginator",
 )
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/__init__.pyi` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/__main__.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridge 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EventBridge 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/client.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EventBridgeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -177,15 +176,15 @@
         self,
         *,
         Name: str,
         ConnectionArn: str,
         InvocationEndpoint: str,
         HttpMethod: ApiDestinationHttpMethodType,
         Description: str = ...,
-        InvocationRateLimitPerSecond: int = ...
+        InvocationRateLimitPerSecond: int = ...,
     ) -> CreateApiDestinationResponseTypeDef:
         """
         Creates an API destination, which is an HTTP invocation endpoint configured as
         a target for
         events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_api_destination)
@@ -195,30 +194,30 @@
     async def create_archive(
         self,
         *,
         ArchiveName: str,
         EventSourceArn: str,
         Description: str = ...,
         EventPattern: str = ...,
-        RetentionDays: int = ...
+        RetentionDays: int = ...,
     ) -> CreateArchiveResponseTypeDef:
         """
         Creates an archive of events with the specified settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_archive)
         """
 
     async def create_connection(
         self,
         *,
         Name: str,
         AuthorizationType: ConnectionAuthorizationTypeType,
         AuthParameters: CreateConnectionAuthRequestParametersTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Creates a connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_connection)
         """
@@ -227,15 +226,15 @@
         self,
         *,
         Name: str,
         RoutingConfig: RoutingConfigTypeDef,
         EventBuses: Sequence[EndpointEventBusTypeDef],
         Description: str = ...,
         ReplicationConfig: ReplicationConfigTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates a global endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_endpoint)
         """
@@ -456,15 +455,15 @@
 
     async def list_api_destinations(
         self,
         *,
         NamePrefix: str = ...,
         ConnectionArn: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListApiDestinationsResponseTypeDef:
         """
         Retrieves a list of API destination in the account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_api_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_api_destinations)
         """
@@ -472,45 +471,45 @@
     async def list_archives(
         self,
         *,
         NamePrefix: str = ...,
         EventSourceArn: str = ...,
         State: ArchiveStateType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListArchivesResponseTypeDef:
         """
         Lists your archives.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_archives)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_archives)
         """
 
     async def list_connections(
         self,
         *,
         NamePrefix: str = ...,
         ConnectionState: ConnectionStateType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListConnectionsResponseTypeDef:
         """
         Retrieves a list of connections from the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_connections)
         """
 
     async def list_endpoints(
         self,
         *,
         NamePrefix: str = ...,
         HomeRegion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEndpointsResponseTypeDef:
         """
         List the global endpoints associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_endpoints)
         """
@@ -566,15 +565,15 @@
     async def list_replays(
         self,
         *,
         NamePrefix: str = ...,
         State: ReplayStateType = ...,
         EventSourceArn: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListReplaysResponseTypeDef:
         """
         Lists your replays.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_replays)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_replays)
         """
@@ -591,15 +590,15 @@
 
     async def list_rules(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists your Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_rules)
         """
@@ -648,15 +647,15 @@
         self,
         *,
         EventBusName: str = ...,
         Action: str = ...,
         Principal: str = ...,
         StatementId: str = ...,
         Condition: ConditionTypeDef = ...,
-        Policy: str = ...
+        Policy: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Running `PutPermission` permits the specified Amazon Web Services account or
         Amazon Web Services organization to put events to the specified *event
         bus*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_permission)
@@ -669,15 +668,15 @@
         Name: str,
         ScheduleExpression: str = ...,
         EventPattern: str = ...,
         State: RuleStateType = ...,
         Description: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EventBusName: str = ...
+        EventBusName: str = ...,
     ) -> PutRuleResponseTypeDef:
         """
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_rule)
         """
@@ -720,15 +719,15 @@
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
         Destination: ReplayDestinationTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#start_replay)
         """
@@ -764,45 +763,45 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         ConnectionArn: str = ...,
         InvocationEndpoint: str = ...,
         HttpMethod: ApiDestinationHttpMethodType = ...,
-        InvocationRateLimitPerSecond: int = ...
+        InvocationRateLimitPerSecond: int = ...,
     ) -> UpdateApiDestinationResponseTypeDef:
         """
         Updates an API destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_api_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_api_destination)
         """
 
     async def update_archive(
         self,
         *,
         ArchiveName: str,
         Description: str = ...,
         EventPattern: str = ...,
-        RetentionDays: int = ...
+        RetentionDays: int = ...,
     ) -> UpdateArchiveResponseTypeDef:
         """
         Updates the specified archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_archive)
         """
 
     async def update_connection(
         self,
         *,
         Name: str,
         Description: str = ...,
         AuthorizationType: ConnectionAuthorizationTypeType = ...,
-        AuthParameters: UpdateConnectionAuthRequestParametersTypeDef = ...
+        AuthParameters: UpdateConnectionAuthRequestParametersTypeDef = ...,
     ) -> UpdateConnectionResponseTypeDef:
         """
         Updates settings for a connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_connection)
         """
@@ -811,15 +810,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         RoutingConfig: RoutingConfigTypeDef = ...,
         ReplicationConfig: ReplicationConfigTypeDef = ...,
         EventBuses: Sequence[EndpointEventBusTypeDef] = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateEndpointResponseTypeDef:
         """
         Update an existing endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_endpoint)
         """
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/client.pyi` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         self,
         *,
         Name: str,
         ConnectionArn: str,
         InvocationEndpoint: str,
         HttpMethod: ApiDestinationHttpMethodType,
         Description: str = ...,
-        InvocationRateLimitPerSecond: int = ...
+        InvocationRateLimitPerSecond: int = ...,
     ) -> CreateApiDestinationResponseTypeDef:
         """
         Creates an API destination, which is an HTTP invocation endpoint configured as
         a target for
         events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_api_destination)
@@ -191,30 +191,30 @@
     async def create_archive(
         self,
         *,
         ArchiveName: str,
         EventSourceArn: str,
         Description: str = ...,
         EventPattern: str = ...,
-        RetentionDays: int = ...
+        RetentionDays: int = ...,
     ) -> CreateArchiveResponseTypeDef:
         """
         Creates an archive of events with the specified settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_archive)
         """
 
     async def create_connection(
         self,
         *,
         Name: str,
         AuthorizationType: ConnectionAuthorizationTypeType,
         AuthParameters: CreateConnectionAuthRequestParametersTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> CreateConnectionResponseTypeDef:
         """
         Creates a connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_connection)
         """
@@ -223,15 +223,15 @@
         self,
         *,
         Name: str,
         RoutingConfig: RoutingConfigTypeDef,
         EventBuses: Sequence[EndpointEventBusTypeDef],
         Description: str = ...,
         ReplicationConfig: ReplicationConfigTypeDef = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates a global endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#create_endpoint)
         """
@@ -452,15 +452,15 @@
 
     async def list_api_destinations(
         self,
         *,
         NamePrefix: str = ...,
         ConnectionArn: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListApiDestinationsResponseTypeDef:
         """
         Retrieves a list of API destination in the account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_api_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_api_destinations)
         """
@@ -468,45 +468,45 @@
     async def list_archives(
         self,
         *,
         NamePrefix: str = ...,
         EventSourceArn: str = ...,
         State: ArchiveStateType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListArchivesResponseTypeDef:
         """
         Lists your archives.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_archives)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_archives)
         """
 
     async def list_connections(
         self,
         *,
         NamePrefix: str = ...,
         ConnectionState: ConnectionStateType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListConnectionsResponseTypeDef:
         """
         Retrieves a list of connections from the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_connections)
         """
 
     async def list_endpoints(
         self,
         *,
         NamePrefix: str = ...,
         HomeRegion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEndpointsResponseTypeDef:
         """
         List the global endpoints associated with this account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_endpoints)
         """
@@ -562,15 +562,15 @@
     async def list_replays(
         self,
         *,
         NamePrefix: str = ...,
         State: ReplayStateType = ...,
         EventSourceArn: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListReplaysResponseTypeDef:
         """
         Lists your replays.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_replays)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_replays)
         """
@@ -587,15 +587,15 @@
 
     async def list_rules(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists your Amazon EventBridge rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#list_rules)
         """
@@ -644,15 +644,15 @@
         self,
         *,
         EventBusName: str = ...,
         Action: str = ...,
         Principal: str = ...,
         StatementId: str = ...,
         Condition: ConditionTypeDef = ...,
-        Policy: str = ...
+        Policy: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Running `PutPermission` permits the specified Amazon Web Services account or
         Amazon Web Services organization to put events to the specified *event
         bus*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_permission)
@@ -665,15 +665,15 @@
         Name: str,
         ScheduleExpression: str = ...,
         EventPattern: str = ...,
         State: RuleStateType = ...,
         Description: str = ...,
         RoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EventBusName: str = ...
+        EventBusName: str = ...,
     ) -> PutRuleResponseTypeDef:
         """
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_rule)
         """
@@ -716,15 +716,15 @@
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
         Destination: ReplayDestinationTypeDef,
-        Description: str = ...
+        Description: str = ...,
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#start_replay)
         """
@@ -760,45 +760,45 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         ConnectionArn: str = ...,
         InvocationEndpoint: str = ...,
         HttpMethod: ApiDestinationHttpMethodType = ...,
-        InvocationRateLimitPerSecond: int = ...
+        InvocationRateLimitPerSecond: int = ...,
     ) -> UpdateApiDestinationResponseTypeDef:
         """
         Updates an API destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_api_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_api_destination)
         """
 
     async def update_archive(
         self,
         *,
         ArchiveName: str,
         Description: str = ...,
         EventPattern: str = ...,
-        RetentionDays: int = ...
+        RetentionDays: int = ...,
     ) -> UpdateArchiveResponseTypeDef:
         """
         Updates the specified archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_archive)
         """
 
     async def update_connection(
         self,
         *,
         Name: str,
         Description: str = ...,
         AuthorizationType: ConnectionAuthorizationTypeType = ...,
-        AuthParameters: UpdateConnectionAuthRequestParametersTypeDef = ...
+        AuthParameters: UpdateConnectionAuthRequestParametersTypeDef = ...,
     ) -> UpdateConnectionResponseTypeDef:
         """
         Updates settings for a connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_connection)
         """
@@ -807,15 +807,15 @@
         self,
         *,
         Name: str,
         Description: str = ...,
         RoutingConfig: RoutingConfigTypeDef = ...,
         ReplicationConfig: ReplicationConfigTypeDef = ...,
         EventBuses: Sequence[EndpointEventBusTypeDef] = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateEndpointResponseTypeDef:
         """
         Update an existing endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#update_endpoint)
         """
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/literals.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/literals.py`

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
     "ApiDestinationHttpMethodType",
     "ApiDestinationStateType",
     "ArchiveStateType",
     "AssignPublicIpType",
     "ConnectionAuthorizationTypeType",
     "ConnectionOAuthHttpMethodType",
@@ -43,15 +42,14 @@
     "EventBridgeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiDestinationHttpMethodType = Literal["DELETE", "GET", "HEAD", "OPTIONS", "PATCH", "POST", "PUT"]
 ApiDestinationStateType = Literal["ACTIVE", "INACTIVE"]
 ArchiveStateType = Literal[
     "CREATE_FAILED", "CREATING", "DISABLED", "ENABLED", "UPDATE_FAILED", "UPDATING"
 ]
 AssignPublicIpType = Literal["DISABLED", "ENABLED"]
 ConnectionAuthorizationTypeType = Literal["API_KEY", "BASIC", "OAUTH_CLIENT_CREDENTIALS"]
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/literals.pyi` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/paginator.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListRulesResponseTypeDef,
     ListTargetsByRuleResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListRuleNamesByTargetPaginator", "ListRulesPaginator", "ListTargetsByRulePaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -57,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 
@@ -76,15 +75,15 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/paginators/#listrulespaginator)
         """
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/paginator.pyi` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """
 
     def paginate(
         self,
         *,
         TargetArn: str,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRuleNamesByTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRuleNamesByTarget.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/paginators/#listrulenamesbytargetpaginator)
         """
 
 class ListRulesPaginator(AioPaginator):
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         NamePrefix: str = ...,
         EventBusName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/paginators/#listrulespaginator)
         """
 
 class ListTargetsByRulePaginator(AioPaginator):
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/type_defs.py` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events/type_defs.pyi` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/PKG-INFO` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-events
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EventBridge 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EventBridge 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/
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
 
 <a id="types-aiobotocore-events"></a>
 
 # types-aiobotocore-events
 
 [![PyPI - types-aiobotocore-events](https://img.shields.io/pypi/v/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-events.svg?color=blue)](https://pypi.org/project/types-aiobotocore-events)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-events)](https://pepy.tech/project/types-aiobotocore-events)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EventBridge 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
+[aiobotocore.EventBridge 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge)
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
 [types-aiobotocore-events docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-events-2.9.0/types_aiobotocore_events.egg-info/SOURCES.txt` & `types-aiobotocore-events-2.9.1/types_aiobotocore_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

