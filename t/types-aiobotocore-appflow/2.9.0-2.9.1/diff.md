# Comparing `tmp/types-aiobotocore-appflow-2.9.0.tar.gz` & `tmp/types-aiobotocore-appflow-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appflow-2.9.0.tar", last modified: Wed Dec 13 19:58:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-appflow-2.9.1.tar", last modified: Thu Jan 18 01:20:02 2024, max compression
```

## Comparing `types-aiobotocore-appflow-2.9.0.tar` & `types-aiobotocore-appflow-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.234099 types-aiobotocore-appflow-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2023-12-13 19:58:34.234099 types-aiobotocore-appflow-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10674 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:34.234099 types-aiobotocore-appflow-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.230099 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21174 2023-12-13 19:41:02.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21170 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18930 2023-12-13 19:41:02.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18928 2023-12-13 19:41:02.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    60940 2023-12-13 19:41:03.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    60939 2023-12-13 19:41:02.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:01.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:34.234099 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12237 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:34.000000 types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.357518 types-aiobotocore-appflow-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-01-18 01:20:02.357518 types-aiobotocore-appflow-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10674 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:02.357518 types-aiobotocore-appflow-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.353518 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21184 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21181 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-01-18 01:03:01.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18928 2024-01-18 01:03:01.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    60939 2024-01-18 01:03:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60939 2024-01-18 01:03:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:00.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:02.357518 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:02.000000 types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appflow-2.9.0/LICENSE` & `types-aiobotocore-appflow-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appflow-2.9.0/PKG-INFO` & `types-aiobotocore-appflow-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Appflow 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Appflow 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
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
 
 <a id="types-aiobotocore-appflow"></a>
 
 # types-aiobotocore-appflow
 
 [![PyPI - types-aiobotocore-appflow](https://img.shields.io/pypi/v/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appflow-2.9.0/README.md` & `types-aiobotocore-appflow-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appflow-2.9.0/setup.py` & `types-aiobotocore-appflow-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appflow",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Appflow 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Appflow 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appflow type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appflow": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/__main__.py` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Appflow 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Appflow 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow\nOther"
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

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/client.py` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppflowClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -130,15 +129,15 @@
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         kmsArn: str = ...,
         connectorLabel: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateConnectorProfileResponseTypeDef:
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
@@ -152,15 +151,15 @@
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_flow)
         """
@@ -196,15 +195,15 @@
 
     async def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
-        apiVersion: str = ...
+        apiVersion: str = ...,
     ) -> DescribeConnectorEntityResponseTypeDef:
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that
         entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
@@ -214,15 +213,15 @@
     async def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeConnectorProfilesResponseTypeDef:
         """
         Returns a list of `connector-profile` details matching the provided
         `connector-profile` names and
         `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
@@ -230,15 +229,15 @@
         """
 
     async def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#describe_connectors)
         """
@@ -279,15 +278,15 @@
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#list_connector_entities)
         """
@@ -327,15 +326,15 @@
     async def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#register_connector)
         """
@@ -343,15 +342,15 @@
     async def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
-        apiVersion: str = ...
+        apiVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#reset_connector_metadata_cache)
@@ -405,30 +404,30 @@
 
     async def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_profile)
         """
 
     async def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
@@ -439,15 +438,15 @@
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_flow)
         """
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/client.pyi` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         *,
         connectorProfileName: str,
         connectorType: ConnectorTypeType,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
         kmsArn: str = ...,
         connectorLabel: str = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateConnectorProfileResponseTypeDef:
         """
         Creates a new connector profile associated with your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_connector_profile)
@@ -148,15 +148,15 @@
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         kmsArn: str = ...,
         tags: Mapping[str, str] = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateFlowResponseTypeDef:
         """
         Enables your application to create a new flow using Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.create_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#create_flow)
         """
@@ -192,15 +192,15 @@
 
     async def describe_connector_entity(
         self,
         *,
         connectorEntityName: str,
         connectorType: ConnectorTypeType = ...,
         connectorProfileName: str = ...,
-        apiVersion: str = ...
+        apiVersion: str = ...,
     ) -> DescribeConnectorEntityResponseTypeDef:
         """
         Provides details regarding the entity used with the connector, with a
         description of the data model for each field in that
         entity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_entity)
@@ -210,15 +210,15 @@
     async def describe_connector_profiles(
         self,
         *,
         connectorProfileNames: Sequence[str] = ...,
         connectorType: ConnectorTypeType = ...,
         connectorLabel: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeConnectorProfilesResponseTypeDef:
         """
         Returns a list of `connector-profile` details matching the provided
         `connector-profile` names and
         `connector-types`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connector_profiles)
@@ -226,15 +226,15 @@
         """
 
     async def describe_connectors(
         self,
         *,
         connectorTypes: Sequence[ConnectorTypeType] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeConnectorsResponseTypeDef:
         """
         Describes the connectors vended by Amazon AppFlow for specified connector types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.describe_connectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#describe_connectors)
         """
@@ -275,15 +275,15 @@
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         entitiesPath: str = ...,
         apiVersion: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListConnectorEntitiesResponseTypeDef:
         """
         Returns the list of available connector entities supported by Amazon AppFlow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.list_connector_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#list_connector_entities)
         """
@@ -323,15 +323,15 @@
     async def register_connector(
         self,
         *,
         connectorLabel: str = ...,
         description: str = ...,
         connectorProvisioningType: Literal["LAMBDA"] = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> RegisterConnectorResponseTypeDef:
         """
         Registers a new custom connector with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.register_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#register_connector)
         """
@@ -339,15 +339,15 @@
     async def reset_connector_metadata_cache(
         self,
         *,
         connectorProfileName: str = ...,
         connectorType: ConnectorTypeType = ...,
         connectorEntityName: str = ...,
         entitiesPath: str = ...,
-        apiVersion: str = ...
+        apiVersion: str = ...,
     ) -> Dict[str, Any]:
         """
         Resets metadata about your connector entities that Amazon AppFlow stored in its
         cache.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.reset_connector_metadata_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#reset_connector_metadata_cache)
@@ -401,30 +401,30 @@
 
     async def update_connector_profile(
         self,
         *,
         connectorProfileName: str,
         connectionMode: ConnectionModeType,
         connectorProfileConfig: ConnectorProfileConfigTypeDef,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateConnectorProfileResponseTypeDef:
         """
         Updates a given connector profile associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_profile)
         """
 
     async def update_connector_registration(
         self,
         *,
         connectorLabel: str,
         description: str = ...,
         connectorProvisioningConfig: ConnectorProvisioningConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateConnectorRegistrationResponseTypeDef:
         """
         Updates a custom connector that you've previously registered.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_connector_registration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_connector_registration)
         """
@@ -435,15 +435,15 @@
         flowName: str,
         triggerConfig: TriggerConfigTypeDef,
         sourceFlowConfig: SourceFlowConfigTypeDef,
         destinationFlowConfigList: Sequence[DestinationFlowConfigTypeDef],
         tasks: Sequence[TaskTypeDef],
         description: str = ...,
         metadataCatalogConfig: MetadataCatalogConfigTypeDef = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates an existing flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow.Client.update_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/client/#update_flow)
         """
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/literals.py` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/literals.py`

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
     "AggregationTypeType",
     "AmplitudeConnectorOperatorType",
     "AuthenticationTypeType",
     "CatalogTypeType",
     "ConnectionModeType",
     "ConnectorProvisioningTypeType",
@@ -67,15 +66,14 @@
     "ZendeskConnectorOperatorType",
     "AppflowServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AggregationTypeType = Literal["None", "SingleFile"]
 AmplitudeConnectorOperatorType = Literal["BETWEEN"]
 AuthenticationTypeType = Literal["APIKEY", "BASIC", "CUSTOM", "OAUTH2"]
 CatalogTypeType = Literal["GLUE"]
 ConnectionModeType = Literal["Private", "Public"]
 ConnectorProvisioningTypeType = Literal["LAMBDA"]
 ConnectorTypeType = Literal[
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/literals.pyi` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/type_defs.py` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AggregationConfigTypeDef",
     "AmplitudeConnectorProfileCredentialsTypeDef",
     "AmplitudeSourcePropertiesTypeDef",
     "ApiKeyCredentialsTypeDef",
     "AuthParameterTypeDef",
     "BasicAuthCredentialsTypeDef",
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow/type_defs.pyi` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/PKG-INFO` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appflow
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Appflow 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Appflow 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/
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
 
 <a id="types-aiobotocore-appflow"></a>
 
 # types-aiobotocore-appflow
 
 [![PyPI - types-aiobotocore-appflow](https://img.shields.io/pypi/v/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appflow.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appflow)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appflow)](https://pepy.tech/project/types-aiobotocore-appflow)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Appflow 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
+[aiobotocore.Appflow 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#Appflow)
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
 [types-aiobotocore-appflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appflow/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appflow-2.9.0/types_aiobotocore_appflow.egg-info/SOURCES.txt` & `types-aiobotocore-appflow-2.9.1/types_aiobotocore_appflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

