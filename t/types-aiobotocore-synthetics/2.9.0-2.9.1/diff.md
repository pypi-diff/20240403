# Comparing `tmp/types-aiobotocore-synthetics-2.9.0.tar.gz` & `tmp/types-aiobotocore-synthetics-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-synthetics-2.9.0.tar", last modified: Wed Dec 13 20:00:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-synthetics-2.9.1.tar", last modified: Thu Jan 18 01:21:57 2024, max compression
```

## Comparing `types-aiobotocore-synthetics-2.9.0.tar` & `types-aiobotocore-synthetics-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.017056 types-aiobotocore-synthetics-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2023-12-13 20:00:40.017056 types-aiobotocore-synthetics-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10841 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:40.017056 types-aiobotocore-synthetics-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.013056 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17095 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    17092 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16304 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16303 2023-12-13 19:57:15.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:14.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.017056 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12416 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:39.000000 types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.512995 types-aiobotocore-synthetics-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-01-18 01:21:57.512995 types-aiobotocore-synthetics-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10841 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:57.512995 types-aiobotocore-synthetics-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.512995 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17097 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17094 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16303 2024-01-18 01:18:43.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16303 2024-01-18 01:18:43.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:42.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.512995 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:57.000000 types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-synthetics-2.9.0/LICENSE` & `types-aiobotocore-synthetics-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-synthetics-2.9.0/PKG-INFO` & `types-aiobotocore-synthetics-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-synthetics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Synthetics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Synthetics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
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
 
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Synthetics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[aiobotocore.Synthetics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-synthetics-2.9.0/README.md` & `types-aiobotocore-synthetics-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Synthetics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[aiobotocore.Synthetics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-synthetics-2.9.0/setup.py` & `types-aiobotocore-synthetics-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-synthetics",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_synthetics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Synthetics 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Synthetics 2.9.1 service generated with"
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
     keywords="aiobotocore synthetics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_synthetics": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/__main__.py` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Synthetics 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Synthetics 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics\nOther"
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

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/client.py` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -39,37 +39,34 @@
     ListTagsForResourceResponseTypeDef,
     VisualReferenceInputTypeDef,
     VpcConfigInputTypeDef,
 )
 
 __all__ = ("SyntheticsClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     RequestEntityTooLargeException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class SyntheticsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/)
     """
 
     meta: ClientMeta
@@ -117,15 +114,15 @@
         Schedule: CanaryScheduleInputTypeDef,
         RuntimeVersion: str,
         RunConfig: CanaryRunConfigInputTypeDef = ...,
         SuccessRetentionPeriodInDays: int = ...,
         FailureRetentionPeriodInDays: int = ...,
         VpcConfig: VpcConfigInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        ArtifactConfig: ArtifactConfigInputTypeDef = ...
+        ArtifactConfig: ArtifactConfigInputTypeDef = ...,
     ) -> CreateCanaryResponseTypeDef:
         """
         Creates a canary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.create_canary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/#create_canary)
         """
@@ -328,15 +325,15 @@
         Schedule: CanaryScheduleInputTypeDef = ...,
         RunConfig: CanaryRunConfigInputTypeDef = ...,
         SuccessRetentionPeriodInDays: int = ...,
         FailureRetentionPeriodInDays: int = ...,
         VpcConfig: VpcConfigInputTypeDef = ...,
         VisualReference: VisualReferenceInputTypeDef = ...,
         ArtifactS3Location: str = ...,
-        ArtifactConfig: ArtifactConfigInputTypeDef = ...
+        ArtifactConfig: ArtifactConfigInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of a canary that has already been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.update_canary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/#update_canary)
         """
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/client.pyi` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,34 +39,37 @@
     ListTagsForResourceResponseTypeDef,
     VisualReferenceInputTypeDef,
     VpcConfigInputTypeDef,
 )
 
 __all__ = ("SyntheticsClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     RequestEntityTooLargeException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class SyntheticsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/)
     """
 
     meta: ClientMeta
@@ -114,15 +117,15 @@
         Schedule: CanaryScheduleInputTypeDef,
         RuntimeVersion: str,
         RunConfig: CanaryRunConfigInputTypeDef = ...,
         SuccessRetentionPeriodInDays: int = ...,
         FailureRetentionPeriodInDays: int = ...,
         VpcConfig: VpcConfigInputTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        ArtifactConfig: ArtifactConfigInputTypeDef = ...
+        ArtifactConfig: ArtifactConfigInputTypeDef = ...,
     ) -> CreateCanaryResponseTypeDef:
         """
         Creates a canary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.create_canary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/#create_canary)
         """
@@ -325,15 +328,15 @@
         Schedule: CanaryScheduleInputTypeDef = ...,
         RunConfig: CanaryRunConfigInputTypeDef = ...,
         SuccessRetentionPeriodInDays: int = ...,
         FailureRetentionPeriodInDays: int = ...,
         VpcConfig: VpcConfigInputTypeDef = ...,
         VisualReference: VisualReferenceInputTypeDef = ...,
         ArtifactS3Location: str = ...,
-        ArtifactConfig: ArtifactConfigInputTypeDef = ...
+        ArtifactConfig: ArtifactConfigInputTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration of a canary that has already been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics.Client.update_canary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/client/#update_canary)
         """
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/literals.py` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "CanaryRunStateReasonCodeType",
     "CanaryRunStateType",
     "CanaryStateReasonCodeType",
     "CanaryStateType",
     "EncryptionModeType",
     "SyntheticsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 CanaryRunStateReasonCodeType = Literal["CANARY_FAILURE", "EXECUTION_FAILURE"]
 CanaryRunStateType = Literal["FAILED", "PASSED", "RUNNING"]
 CanaryStateReasonCodeType = Literal[
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_PENDING",
     "DELETE_FAILED",
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/literals.pyi` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/type_defs.py` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "S3EncryptionConfigTypeDef",
     "AssociateResourceRequestRequestTypeDef",
     "BaseScreenshotTypeDef",
     "BlobTypeDef",
     "CanaryCodeOutputTypeDef",
     "CanaryRunConfigInputTypeDef",
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics/type_defs.pyi` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/PKG-INFO` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-synthetics
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Synthetics 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Synthetics 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/
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
 
 <a id="types-aiobotocore-synthetics"></a>
 
 # types-aiobotocore-synthetics
 
 [![PyPI - types-aiobotocore-synthetics](https://img.shields.io/pypi/v/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-synthetics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-synthetics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-synthetics)](https://pepy.tech/project/types-aiobotocore-synthetics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Synthetics 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
+[aiobotocore.Synthetics 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#Synthetics)
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
 [types-aiobotocore-synthetics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_synthetics/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-synthetics-2.9.0/types_aiobotocore_synthetics.egg-info/SOURCES.txt` & `types-aiobotocore-synthetics-2.9.1/types_aiobotocore_synthetics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

