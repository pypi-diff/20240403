# Comparing `tmp/types-aiobotocore-efs-2.9.0.tar.gz` & `tmp/types-aiobotocore-efs-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-efs-2.9.0.tar", last modified: Wed Dec 13 19:59:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-efs-2.9.1.tar", last modified: Thu Jan 18 01:20:37 2024, max compression
```

## Comparing `types-aiobotocore-efs-2.9.0.tar` & `types-aiobotocore-efs-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.689784 types-aiobotocore-efs-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2023-12-13 19:59:12.689784 types-aiobotocore-efs-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11908 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:12.689784 types-aiobotocore-efs-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.689784 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27088 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27084 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2023-12-13 19:45:32.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10881 2023-12-13 19:45:32.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2023-12-13 19:45:33.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24098 2023-12-13 19:45:33.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:31.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:12.689784 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:12.000000 types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.669357 types-aiobotocore-efs-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-01-18 01:20:37.669357 types-aiobotocore-efs-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:37.669357 types-aiobotocore-efs-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.665357 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27095 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27092 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10881 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24098 2024-01-18 01:07:29.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24098 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:28.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:37.669357 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13475 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:37.000000 types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-efs-2.9.0/LICENSE` & `types-aiobotocore-efs-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-efs-2.9.0/PKG-INFO` & `types-aiobotocore-efs-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EFS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EFS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
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
 
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-efs-2.9.0/README.md` & `types-aiobotocore-efs-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-efs-2.9.0/setup.py` & `types-aiobotocore-efs-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-efs",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.EFS 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.EFS 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore efs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_efs": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__init__.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     DescribeMountTargetsPaginator,
     DescribeReplicationConfigurationsPaginator,
     DescribeTagsPaginator,
 )
 
 Client = EFSClient
 
-
 __all__ = (
     "Client",
     "DescribeAccessPointsPaginator",
     "DescribeFileSystemsPaginator",
     "DescribeMountTargetsPaginator",
     "DescribeReplicationConfigurationsPaginator",
     "DescribeTagsPaginator",
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__init__.pyi` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/__main__.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EFS 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.EFS 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/client.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("EFSClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -150,15 +149,15 @@
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
         PosixUser: PosixUserTypeDef = ...,
-        RootDirectory: RootDirectoryTypeDef = ...
+        RootDirectory: RootDirectoryTypeDef = ...,
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
         """
@@ -170,30 +169,30 @@
         PerformanceMode: PerformanceModeType = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_file_system)
         """
 
     async def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
     ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_mount_target)
         """
@@ -274,15 +273,15 @@
 
     async def describe_access_points(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccessPointId: str = ...,
-        FileSystemId: str = ...
+        FileSystemId: str = ...,
     ) -> DescribeAccessPointsResponseTypeDef:
         """
         Returns the description of a specific Amazon EFS access point if the
         `AccessPointId` is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_access_points)
@@ -321,15 +320,15 @@
 
     async def describe_file_systems(
         self,
         *,
         MaxItems: int = ...,
         Marker: str = ...,
         CreationToken: str = ...,
-        FileSystemId: str = ...
+        FileSystemId: str = ...,
     ) -> DescribeFileSystemsResponseTypeDef:
         """
         Returns the description of a specific Amazon EFS file system if either the file
         system `CreationToken` or the `FileSystemId` is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_file_systems)
@@ -361,15 +360,15 @@
     async def describe_mount_targets(
         self,
         *,
         MaxItems: int = ...,
         Marker: str = ...,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
-        AccessPointId: str = ...
+        AccessPointId: str = ...,
     ) -> DescribeMountTargetsResponseTypeDef:
         """
         Returns the descriptions of all the current mount targets, or a specific mount
         target, for a file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_mount_targets)
@@ -494,30 +493,30 @@
         """
 
     async def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
-        ProvisionedThroughputInMibps: float = ...
+        ProvisionedThroughputInMibps: float = ...,
     ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system)
         """
 
     async def update_file_system_protection(
         self,
         *,
         FileSystemId: str,
-        ReplicationOverwriteProtection: ReplicationOverwriteProtectionType = ...
+        ReplicationOverwriteProtection: ReplicationOverwriteProtectionType = ...,
     ) -> FileSystemProtectionDescriptionResponseTypeDef:
         """
         Updates protection on the file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system_protection)
         """
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/client.pyi` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
         PosixUser: PosixUserTypeDef = ...,
-        RootDirectory: RootDirectoryTypeDef = ...
+        RootDirectory: RootDirectoryTypeDef = ...,
     ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
         """
@@ -166,30 +166,30 @@
         PerformanceMode: PerformanceModeType = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_file_system)
         """
 
     async def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
-        SecurityGroups: Sequence[str] = ...
+        SecurityGroups: Sequence[str] = ...,
     ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_mount_target)
         """
@@ -270,15 +270,15 @@
 
     async def describe_access_points(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         AccessPointId: str = ...,
-        FileSystemId: str = ...
+        FileSystemId: str = ...,
     ) -> DescribeAccessPointsResponseTypeDef:
         """
         Returns the description of a specific Amazon EFS access point if the
         `AccessPointId` is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_access_points)
@@ -317,15 +317,15 @@
 
     async def describe_file_systems(
         self,
         *,
         MaxItems: int = ...,
         Marker: str = ...,
         CreationToken: str = ...,
-        FileSystemId: str = ...
+        FileSystemId: str = ...,
     ) -> DescribeFileSystemsResponseTypeDef:
         """
         Returns the description of a specific Amazon EFS file system if either the file
         system `CreationToken` or the `FileSystemId` is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_file_systems)
@@ -357,15 +357,15 @@
     async def describe_mount_targets(
         self,
         *,
         MaxItems: int = ...,
         Marker: str = ...,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
-        AccessPointId: str = ...
+        AccessPointId: str = ...,
     ) -> DescribeMountTargetsResponseTypeDef:
         """
         Returns the descriptions of all the current mount targets, or a specific mount
         target, for a file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.describe_mount_targets)
@@ -490,30 +490,30 @@
         """
 
     async def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
-        ProvisionedThroughputInMibps: float = ...
+        ProvisionedThroughputInMibps: float = ...,
     ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system)
         """
 
     async def update_file_system_protection(
         self,
         *,
         FileSystemId: str,
-        ReplicationOverwriteProtection: ReplicationOverwriteProtectionType = ...
+        ReplicationOverwriteProtection: ReplicationOverwriteProtectionType = ...,
     ) -> FileSystemProtectionDescriptionResponseTypeDef:
         """
         Updates protection on the file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system_protection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system_protection)
         """
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/literals.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/literals.py`

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
     "DescribeAccessPointsPaginatorName",
     "DescribeFileSystemsPaginatorName",
     "DescribeMountTargetsPaginatorName",
     "DescribeReplicationConfigurationsPaginatorName",
     "DescribeTagsPaginatorName",
     "LifeCycleStateType",
@@ -40,15 +39,14 @@
     "EFSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeAccessPointsPaginatorName = Literal["describe_access_points"]
 DescribeFileSystemsPaginatorName = Literal["describe_file_systems"]
 DescribeMountTargetsPaginatorName = Literal["describe_mount_targets"]
 DescribeReplicationConfigurationsPaginatorName = Literal["describe_replication_configurations"]
 DescribeTagsPaginatorName = Literal["describe_tags"]
 LifeCycleStateType = Literal["available", "creating", "deleted", "deleting", "error", "updating"]
 PerformanceModeType = Literal["generalPurpose", "maxIO"]
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/literals.pyi` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/paginator.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,98 +47,91 @@
     "DescribeAccessPointsPaginator",
     "DescribeFileSystemsPaginator",
     "DescribeMountTargetsPaginator",
     "DescribeReplicationConfigurationsPaginator",
     "DescribeTagsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAccessPointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeAccessPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describeaccesspointspaginator)
     """
 
     def paginate(
         self,
         *,
         AccessPointId: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAccessPointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeAccessPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describeaccesspointspaginator)
         """
 
-
 class DescribeFileSystemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
         """
 
-
 class DescribeMountTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
         """
 
-
 class DescribeReplicationConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeReplicationConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describereplicationconfigurationspaginator)
     """
 
     def paginate(
         self, *, FileSystemId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeReplicationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describereplicationconfigurationspaginator)
         """
 
-
 class DescribeTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/paginator.pyi` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,89 +49,95 @@
     "DescribeMountTargetsPaginator",
     "DescribeReplicationConfigurationsPaginator",
     "DescribeTagsPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAccessPointsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeAccessPoints)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describeaccesspointspaginator)
     """
 
     def paginate(
         self,
         *,
         AccessPointId: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAccessPointsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeAccessPoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describeaccesspointspaginator)
         """
 
+
 class DescribeFileSystemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
         """
 
+
 class DescribeMountTargetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
     """
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
         """
 
+
 class DescribeReplicationConfigurationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeReplicationConfigurations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describereplicationconfigurationspaginator)
     """
 
     def paginate(
         self, *, FileSystemId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeReplicationConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeReplicationConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describereplicationconfigurationspaginator)
         """
 
+
 class DescribeTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/type_defs.py` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PosixUserPaginatorTypeDef",
     "TagTypeDef",
     "PosixUserTypeDef",
     "ResponseMetadataTypeDef",
     "BackupPolicyTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs/type_defs.pyi` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/PKG-INFO` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.EFS 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.EFS 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
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
 
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.EFS 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
+[aiobotocore.EFS 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-efs-2.9.0/types_aiobotocore_efs.egg-info/SOURCES.txt` & `types-aiobotocore-efs-2.9.1/types_aiobotocore_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

