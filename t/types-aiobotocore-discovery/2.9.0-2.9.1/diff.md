# Comparing `tmp/types-aiobotocore-discovery-2.9.0.tar.gz` & `tmp/types-aiobotocore-discovery-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-discovery-2.9.0.tar", last modified: Wed Dec 13 19:59:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-discovery-2.9.1.tar", last modified: Thu Jan 18 01:20:32 2024, max compression
```

## Comparing `types-aiobotocore-discovery-2.9.0.tar` & `types-aiobotocore-discovery-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.837832 types-aiobotocore-discovery-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2023-12-13 19:59:06.837832 types-aiobotocore-discovery-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12676 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:06.837832 types-aiobotocore-discovery-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.833832 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27418 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27414 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9948 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26858 2023-12-13 19:44:11.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26857 2023-12-13 19:44:10.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:09.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.837832 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14265 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:06.000000 types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.209385 types-aiobotocore-discovery-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-01-18 01:20:32.209385 types-aiobotocore-discovery-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:32.209385 types-aiobotocore-discovery-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.209385 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27421 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9953 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-01-18 01:06:05.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26857 2024-01-18 01:06:05.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:04.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:32.209385 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:32.000000 types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-discovery-2.9.0/LICENSE` & `types-aiobotocore-discovery-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-discovery-2.9.0/PKG-INFO` & `types-aiobotocore-discovery-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
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
 
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-discovery-2.9.0/README.md` & `types-aiobotocore-discovery-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-discovery-2.9.0/setup.py` & `types-aiobotocore-discovery-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-discovery",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.1 service generated with"
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
     keywords="aiobotocore discovery type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_discovery": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__init__.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     DescribeImportTasksPaginator,
     DescribeTagsPaginator,
     ListConfigurationsPaginator,
 )
 
 Client = ApplicationDiscoveryServiceClient
 
-
 __all__ = (
     "ApplicationDiscoveryServiceClient",
     "Client",
     "DescribeAgentsPaginator",
     "DescribeContinuousExportsPaginator",
     "DescribeExportConfigurationsPaginator",
     "DescribeExportTasksPaginator",
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__init__.pyi` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/__main__.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/client.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApplicationDiscoveryServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -199,15 +198,15 @@
 
     async def describe_agents(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAgentsResponseTypeDef:
         """
         Lists agents or collectors as specified by ID or other filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_agents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#describe_agents)
         """
@@ -256,29 +255,29 @@
 
     async def describe_export_tasks(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Retrieve status of one or more export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#describe_export_tasks)
         """
 
     async def describe_import_tasks(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeImportTasksResponseTypeDef:
         """
         Returns an array of import tasks for your account, including status
         information, times, IDs, the Amazon S3 Object URL for the import file, and
         more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_import_tasks)
@@ -286,15 +285,15 @@
         """
 
     async def describe_tags(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeTagsResponseTypeDef:
         """
         Retrieves a list of configuration items that have tags as specified by the
         key-value pairs, name and value, passed to the optional parameter
         `filters`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_tags)
@@ -344,15 +343,15 @@
     async def list_configurations(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: Sequence[OrderByElementTypeDef] = ...
+        orderBy: Sequence[OrderByElementTypeDef] = ...,
     ) -> ListConfigurationsResponseTypeDef:
         """
         Retrieves a list of configuration items as specified by the value passed to the
         required parameter
         `configurationType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_configurations)
@@ -362,15 +361,15 @@
     async def list_server_neighbors(
         self,
         *,
         configurationId: str,
         portInformationNeeded: bool = ...,
         neighborConfigurationIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServerNeighborsResponseTypeDef:
         """
         Retrieves a list of servers that are one network hop away from a specified
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_server_neighbors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#list_server_neighbors)
@@ -409,15 +408,15 @@
     async def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        preferences: ExportPreferencesTypeDef = ...
+        preferences: ExportPreferencesTypeDef = ...,
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/client.pyi` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
     async def describe_agents(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAgentsResponseTypeDef:
         """
         Lists agents or collectors as specified by ID or other filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_agents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#describe_agents)
         """
@@ -252,29 +252,29 @@
 
     async def describe_export_tasks(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeExportTasksResponseTypeDef:
         """
         Retrieve status of one or more export tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_export_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#describe_export_tasks)
         """
 
     async def describe_import_tasks(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeImportTasksResponseTypeDef:
         """
         Returns an array of import tasks for your account, including status
         information, times, IDs, the Amazon S3 Object URL for the import file, and
         more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_import_tasks)
@@ -282,15 +282,15 @@
         """
 
     async def describe_tags(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeTagsResponseTypeDef:
         """
         Retrieves a list of configuration items that have tags as specified by the
         key-value pairs, name and value, passed to the optional parameter
         `filters`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.describe_tags)
@@ -340,15 +340,15 @@
     async def list_configurations(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: Sequence[OrderByElementTypeDef] = ...
+        orderBy: Sequence[OrderByElementTypeDef] = ...,
     ) -> ListConfigurationsResponseTypeDef:
         """
         Retrieves a list of configuration items as specified by the value passed to the
         required parameter
         `configurationType`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_configurations)
@@ -358,15 +358,15 @@
     async def list_server_neighbors(
         self,
         *,
         configurationId: str,
         portInformationNeeded: bool = ...,
         neighborConfigurationIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListServerNeighborsResponseTypeDef:
         """
         Retrieves a list of servers that are one network hop away from a specified
         server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.list_server_neighbors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/client/#list_server_neighbors)
@@ -405,15 +405,15 @@
     async def start_export_task(
         self,
         *,
         exportDataFormat: Sequence[Literal["CSV"]] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
         startTime: TimestampTypeDef = ...,
         endTime: TimestampTypeDef = ...,
-        preferences: ExportPreferencesTypeDef = ...
+        preferences: ExportPreferencesTypeDef = ...,
     ) -> StartExportTaskResponseTypeDef:
         """
         Begins the export of a discovered data report to an Amazon S3 bucket managed by
         Amazon Web
         Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Client.start_export_task)
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/literals.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/literals.py`

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
     "AgentStatusType",
     "BatchDeleteConfigurationTaskStatusType",
     "BatchDeleteImportDataErrorCodeType",
     "ConfigurationItemTypeType",
     "ContinuousExportStatusType",
     "DataSourceType",
@@ -48,15 +47,14 @@
     "ApplicationDiscoveryServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AgentStatusType = Literal["BLACKLISTED", "HEALTHY", "RUNNING", "SHUTDOWN", "UNHEALTHY", "UNKNOWN"]
 BatchDeleteConfigurationTaskStatusType = Literal[
     "COMPLETED", "DELETING", "FAILED", "INITIALIZING", "VALIDATING"
 ]
 BatchDeleteImportDataErrorCodeType = Literal["INTERNAL_SERVER_ERROR", "NOT_FOUND", "OVER_LIMIT"]
 ConfigurationItemTypeType = Literal["APPLICATION", "CONNECTION", "PROCESS", "SERVER"]
 ContinuousExportStatusType = Literal[
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/literals.pyi` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/paginator.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "DescribeExportConfigurationsPaginator",
     "DescribeExportTasksPaginator",
     "DescribeImportTasksPaginator",
     "DescribeTagsPaginator",
     "ListConfigurationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -83,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeagentspaginator)
         """
 
 
@@ -132,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -150,15 +149,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeimporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeImportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeimporttaskspaginator)
         """
 
 
@@ -168,15 +167,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
         """
 
 
@@ -188,13 +187,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/paginator.pyi` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeagentspaginator)
         """
 
 class DescribeContinuousExportsPaginator(AioPaginator):
@@ -126,15 +126,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeImportTasksPaginator(AioPaginator):
@@ -143,15 +143,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeimporttaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[ImportTaskFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeImportTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describeimporttaskspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
@@ -160,15 +160,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#describetagspaginator)
         """
 
 class ListConfigurationsPaginator(AioPaginator):
@@ -179,13 +179,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/type_defs.py` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteAgentErrorTypeDef",
     "DeleteAgentTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery/type_defs.pyi` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/PKG-INFO` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-discovery
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApplicationDiscoveryService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/
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
 
 <a id="types-aiobotocore-discovery"></a>
 
 # types-aiobotocore-discovery
 
 [![PyPI - types-aiobotocore-discovery](https://img.shields.io/pypi/v/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-discovery.svg?color=blue)](https://pypi.org/project/types-aiobotocore-discovery)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-discovery)](https://pepy.tech/project/types-aiobotocore-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApplicationDiscoveryService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[aiobotocore.ApplicationDiscoveryService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [types-aiobotocore-discovery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_discovery/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-discovery-2.9.0/types_aiobotocore_discovery.egg-info/SOURCES.txt` & `types-aiobotocore-discovery-2.9.1/types_aiobotocore_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

