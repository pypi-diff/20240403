# Comparing `tmp/types-aiobotocore-ebs-2.9.0.tar.gz` & `tmp/types-aiobotocore-ebs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ebs-2.9.0.tar", last modified: Wed Dec 13 19:59:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-ebs-2.9.1.tar", last modified: Thu Jan 18 01:20:35 2024, max compression
```

## Comparing `types-aiobotocore-ebs-2.9.0.tar` & `types-aiobotocore-ebs-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.209804 types-aiobotocore-ebs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2023-12-13 19:59:10.209804 types-aiobotocore-ebs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:10.209804 types-aiobotocore-ebs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.209804 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8569 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8565 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5885 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:36.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:10.209804 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12017 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:10.000000 types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.345368 types-aiobotocore-ebs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-01-18 01:20:35.345368 types-aiobotocore-ebs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:35.345368 types-aiobotocore-ebs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.345368 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8573 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8570 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:31.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.345368 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12037 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:35.000000 types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ebs-2.9.0/LICENSE` & `types-aiobotocore-ebs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ebs-2.9.0/PKG-INFO` & `types-aiobotocore-ebs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EBS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EBS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
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
 
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ebs-2.9.0/README.md` & `types-aiobotocore-ebs-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ebs-2.9.0/setup.py` & `types-aiobotocore-ebs-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ebs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EBS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.EBS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ebs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ebs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/__main__.py` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EBS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EBS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/client.py` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,38 +33,34 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EBSClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentLimitExceededException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class EBSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/)
     """
 
     meta: ClientMeta
@@ -97,15 +93,15 @@
     async def complete_snapshot(
         self,
         *,
         SnapshotId: str,
         ChangedBlocksCount: int,
         Checksum: str = ...,
         ChecksumAlgorithm: Literal["SHA256"] = ...,
-        ChecksumAggregationMethod: Literal["LINEAR"] = ...
+        ChecksumAggregationMethod: Literal["LINEAR"] = ...,
     ) -> CompleteSnapshotResponseTypeDef:
         """
         Seals and completes the snapshot after all of the required blocks of data have
         been written to
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.complete_snapshot)
@@ -139,15 +135,15 @@
     async def list_changed_blocks(
         self,
         *,
         SecondSnapshotId: str,
         FirstSnapshotId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartingBlockIndex: int = ...
+        StartingBlockIndex: int = ...,
     ) -> ListChangedBlocksResponseTypeDef:
         """
         Returns information about the blocks that are different between two Amazon
         Elastic Block Store snapshots of the same volume/snapshot
         lineage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.list_changed_blocks)
@@ -156,15 +152,15 @@
 
     async def list_snapshot_blocks(
         self,
         *,
         SnapshotId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartingBlockIndex: int = ...
+        StartingBlockIndex: int = ...,
     ) -> ListSnapshotBlocksResponseTypeDef:
         """
         Returns information about the blocks in an Amazon Elastic Block Store snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.list_snapshot_blocks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#list_snapshot_blocks)
         """
@@ -174,15 +170,15 @@
         *,
         SnapshotId: str,
         BlockIndex: int,
         BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
-        Progress: int = ...
+        Progress: int = ...,
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.put_snapshot_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#put_snapshot_block)
         """
@@ -193,15 +189,15 @@
         VolumeSize: int,
         ParentSnapshotId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         Encrypted: bool = ...,
         KmsKeyArn: str = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> StartSnapshotResponseTypeDef:
         """
         Creates a new Amazon EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.start_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#start_snapshot)
         """
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/client.pyi` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,32 +35,35 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("EBSClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentLimitExceededException: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     RequestThrottledException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class EBSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/)
     """
 
     meta: ClientMeta
@@ -93,15 +96,15 @@
     async def complete_snapshot(
         self,
         *,
         SnapshotId: str,
         ChangedBlocksCount: int,
         Checksum: str = ...,
         ChecksumAlgorithm: Literal["SHA256"] = ...,
-        ChecksumAggregationMethod: Literal["LINEAR"] = ...
+        ChecksumAggregationMethod: Literal["LINEAR"] = ...,
     ) -> CompleteSnapshotResponseTypeDef:
         """
         Seals and completes the snapshot after all of the required blocks of data have
         been written to
         it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.complete_snapshot)
@@ -135,15 +138,15 @@
     async def list_changed_blocks(
         self,
         *,
         SecondSnapshotId: str,
         FirstSnapshotId: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartingBlockIndex: int = ...
+        StartingBlockIndex: int = ...,
     ) -> ListChangedBlocksResponseTypeDef:
         """
         Returns information about the blocks that are different between two Amazon
         Elastic Block Store snapshots of the same volume/snapshot
         lineage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.list_changed_blocks)
@@ -152,15 +155,15 @@
 
     async def list_snapshot_blocks(
         self,
         *,
         SnapshotId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StartingBlockIndex: int = ...
+        StartingBlockIndex: int = ...,
     ) -> ListSnapshotBlocksResponseTypeDef:
         """
         Returns information about the blocks in an Amazon Elastic Block Store snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.list_snapshot_blocks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#list_snapshot_blocks)
         """
@@ -170,15 +173,15 @@
         *,
         SnapshotId: str,
         BlockIndex: int,
         BlockData: BlobTypeDef,
         DataLength: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"],
-        Progress: int = ...
+        Progress: int = ...,
     ) -> PutSnapshotBlockResponseTypeDef:
         """
         Writes a block of data to a snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.put_snapshot_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#put_snapshot_block)
         """
@@ -189,15 +192,15 @@
         VolumeSize: int,
         ParentSnapshotId: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         Description: str = ...,
         ClientToken: str = ...,
         Encrypted: bool = ...,
         KmsKeyArn: str = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> StartSnapshotResponseTypeDef:
         """
         Creates a new Amazon EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS.Client.start_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/client/#start_snapshot)
         """
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/literals.py` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ChecksumAggregationMethodType",
     "ChecksumAlgorithmType",
     "SSETypeType",
     "StatusType",
     "EBSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ChecksumAggregationMethodType = Literal["LINEAR"]
 ChecksumAlgorithmType = Literal["SHA256"]
 SSETypeType = Literal["none", "sse-ebs", "sse-kms"]
 StatusType = Literal["completed", "error", "pending"]
 EBSServiceName = Literal["ebs"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/literals.pyi` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/type_defs.py` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "BlockTypeDef",
     "ChangedBlockTypeDef",
     "CompleteSnapshotRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetSnapshotBlockRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs/type_defs.pyi` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/PKG-INFO` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EBS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EBS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
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
 
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ebs)](https://pepy.tech/project/types-aiobotocore-ebs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EBS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
+[aiobotocore.EBS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS)
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ebs-2.9.0/types_aiobotocore_ebs.egg-info/SOURCES.txt` & `types-aiobotocore-ebs-2.9.1/types_aiobotocore_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

