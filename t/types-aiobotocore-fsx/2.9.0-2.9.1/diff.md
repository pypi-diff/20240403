# Comparing `tmp/types-aiobotocore-fsx-2.9.0.tar.gz` & `tmp/types-aiobotocore-fsx-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fsx-2.9.0.tar", last modified: Wed Dec 13 19:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-fsx-2.9.1.tar", last modified: Thu Jan 18 01:20:46 2024, max compression
```

## Comparing `types-aiobotocore-fsx-2.9.0.tar` & `types-aiobotocore-fsx-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.001740 types-aiobotocore-fsx-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13435 2023-12-13 19:59:22.001740 types-aiobotocore-fsx-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11888 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:22.001740 types-aiobotocore-fsx-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.001740 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44412 2023-12-13 19:46:31.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    44408 2023-12-13 19:46:31.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16454 2023-12-13 19:46:32.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    16452 2023-12-13 19:46:32.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2023-12-13 19:46:31.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2023-12-13 19:46:31.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    76771 2023-12-13 19:46:33.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    76770 2023-12-13 19:46:32.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:30.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.001740 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13435 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:21.000000 types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.241317 types-aiobotocore-fsx-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-01-18 01:20:46.241317 types-aiobotocore-fsx-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11888 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:46.241317 types-aiobotocore-fsx-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.237317 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44440 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44437 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    76770 2024-01-18 01:08:27.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76770 2024-01-18 01:08:27.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:24.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.241317 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:46.000000 types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fsx-2.9.0/LICENSE` & `types-aiobotocore-fsx-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-fsx-2.9.0/PKG-INFO` & `types-aiobotocore-fsx-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fsx
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FSx 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FSx 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/
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
 
 <a id="types-aiobotocore-fsx"></a>
 
 # types-aiobotocore-fsx
 
 [![PyPI - types-aiobotocore-fsx](https://img.shields.io/pypi/v/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [types-aiobotocore-fsx docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fsx-2.9.0/README.md` & `types-aiobotocore-fsx-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [types-aiobotocore-fsx docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fsx-2.9.0/setup.py` & `types-aiobotocore-fsx-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fsx",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_fsx"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.FSx 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.FSx 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore fsx type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_fsx": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__init__.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     DescribeStorageVirtualMachinesPaginator,
     DescribeVolumesPaginator,
     ListTagsForResourcePaginator,
 )
 
 Client = FSxClient
 
-
 __all__ = (
     "Client",
     "DescribeBackupsPaginator",
     "DescribeFileSystemsPaginator",
     "DescribeStorageVirtualMachinesPaginator",
     "DescribeVolumesPaginator",
     "FSxClient",
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__init__.pyi` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/__main__.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FSx 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.FSx 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx\nOther"
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

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/client.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("FSxClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -232,15 +231,15 @@
         self,
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyBackupResponseTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to
         another Amazon Web Services Region (cross-Region copy) or within the same
         Amazon Web Services Region (in-Region
         copy).
 
@@ -251,15 +250,15 @@
     async def copy_snapshot_and_update_volume(
         self,
         *,
         VolumeId: str,
         SourceSnapshotARN: str,
         ClientRequestToken: str = ...,
         CopyStrategy: OpenZFSCopyStrategyType = ...,
-        Options: Sequence[UpdateOpenZFSVolumeOptionType] = ...
+        Options: Sequence[UpdateOpenZFSVolumeOptionType] = ...,
     ) -> CopySnapshotAndUpdateVolumeResponseTypeDef:
         """
         Updates an existing volume by using a snapshot from another Amazon FSx for
         OpenZFS file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_snapshot_and_update_volume)
@@ -268,15 +267,15 @@
 
     async def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VolumeId: str = ...
+        VolumeId: str = ...,
     ) -> CreateBackupResponseTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or
         Amazon FSx for OpenZFS file
         system.
 
@@ -290,15 +289,15 @@
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_data_repository_association)
         """
@@ -309,15 +308,15 @@
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...,
-        ReleaseConfiguration: ReleaseConfigurationTypeDef = ...
+        ReleaseConfiguration: ReleaseConfigurationTypeDef = ...,
     ) -> CreateDataRepositoryTaskResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_data_repository_task)
         """
@@ -331,15 +330,15 @@
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
-        DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
+        DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...,
     ) -> CreateFileCacheResponseTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_file_cache)
         """
@@ -355,15 +354,15 @@
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
-        OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
     ) -> CreateFileSystemResponseTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_file_system)
         """
@@ -378,15 +377,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
-        StorageCapacity: int = ...
+        StorageCapacity: int = ...,
     ) -> CreateFileSystemFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
@@ -395,15 +394,15 @@
 
     async def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_snapshot)
         """
@@ -413,15 +412,15 @@
         *,
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
+        RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...,
     ) -> CreateStorageVirtualMachineResponseTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_storage_virtual_machine)
         """
@@ -430,15 +429,15 @@
         self,
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
+        OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...,
     ) -> CreateVolumeResponseTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_volume)
         """
@@ -446,15 +445,15 @@
     async def create_volume_from_backup(
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVolumeFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
@@ -472,15 +471,15 @@
         """
 
     async def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
-        DeleteDataInFileSystem: bool = ...
+        DeleteDataInFileSystem: bool = ...,
     ) -> DeleteDataRepositoryAssociationResponseTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_data_repository_association)
         """
@@ -498,15 +497,15 @@
     async def delete_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
-        OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...,
     ) -> DeleteFileSystemResponseTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_file_system)
         """
@@ -533,30 +532,30 @@
 
     async def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
-        OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...,
     ) -> DeleteVolumeResponseTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_volume)
         """
 
     async def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
@@ -565,15 +564,15 @@
 
     async def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the
         request.
 
@@ -583,15 +582,15 @@
 
     async def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDataRepositoryTasksResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the
         request.
 
@@ -613,15 +612,15 @@
 
     async def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFileSystemAliasesResponseTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
@@ -655,15 +654,15 @@
 
     async def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
@@ -672,15 +671,15 @@
 
     async def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageVirtualMachinesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#describe_storage_virtual_machines)
@@ -688,15 +687,15 @@
 
     async def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeVolumesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#describe_volumes)
@@ -750,15 +749,15 @@
 
     async def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
-        Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
+        Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...,
     ) -> RestoreVolumeFromSnapshotResponseTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#restore_volume_from_snapshot)
@@ -795,15 +794,15 @@
 
     async def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationTypeDef = ...
+        S3: S3DataRepositoryConfigurationTypeDef = ...,
     ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
@@ -811,15 +810,15 @@
         """
 
     async def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
-        LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
+        LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...,
     ) -> UpdateFileCacheResponseTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_file_cache)
         """
@@ -830,29 +829,29 @@
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...,
-        StorageType: StorageTypeType = ...
+        StorageType: StorageTypeType = ...,
     ) -> UpdateFileSystemResponseTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_file_system)
         """
 
     async def update_shared_vpc_configuration(
         self,
         *,
         EnableFsxRouteTableUpdatesFromParticipantAccounts: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> UpdateSharedVpcConfigurationResponseTypeDef:
         """
         Configures whether participant accounts in your organization can create Amazon
         FSx for NetApp ONTAP Multi-AZ file systems in subnets that are shared by a
         virtual private cloud (VPC)
         owner.
 
@@ -872,15 +871,15 @@
 
     async def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
-        SvmAdminPassword: str = ...
+        SvmAdminPassword: str = ...,
     ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_storage_virtual_machine)
         """
@@ -888,15 +887,15 @@
     async def update_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
-        OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
+        OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...,
     ) -> UpdateVolumeResponseTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS
         volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/client.pyi` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -228,15 +228,15 @@
         self,
         *,
         SourceBackupId: str,
         ClientRequestToken: str = ...,
         SourceRegion: str = ...,
         KmsKeyId: str = ...,
         CopyTags: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyBackupResponseTypeDef:
         """
         Copies an existing backup within the same Amazon Web Services account to
         another Amazon Web Services Region (cross-Region copy) or within the same
         Amazon Web Services Region (in-Region
         copy).
 
@@ -247,15 +247,15 @@
     async def copy_snapshot_and_update_volume(
         self,
         *,
         VolumeId: str,
         SourceSnapshotARN: str,
         ClientRequestToken: str = ...,
         CopyStrategy: OpenZFSCopyStrategyType = ...,
-        Options: Sequence[UpdateOpenZFSVolumeOptionType] = ...
+        Options: Sequence[UpdateOpenZFSVolumeOptionType] = ...,
     ) -> CopySnapshotAndUpdateVolumeResponseTypeDef:
         """
         Updates an existing volume by using a snapshot from another Amazon FSx for
         OpenZFS file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.copy_snapshot_and_update_volume)
@@ -264,15 +264,15 @@
 
     async def create_backup(
         self,
         *,
         FileSystemId: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        VolumeId: str = ...
+        VolumeId: str = ...,
     ) -> CreateBackupResponseTypeDef:
         """
         Creates a backup of an existing Amazon FSx for Windows File Server file system,
         Amazon FSx for Lustre file system, Amazon FSx for NetApp ONTAP volume, or
         Amazon FSx for OpenZFS file
         system.
 
@@ -286,15 +286,15 @@
         FileSystemId: str,
         DataRepositoryPath: str,
         FileSystemPath: str = ...,
         BatchImportMetaDataOnCreate: bool = ...,
         ImportedFileChunkSize: int = ...,
         S3: S3DataRepositoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataRepositoryAssociationResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository association (DRA).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_data_repository_association)
         """
@@ -305,15 +305,15 @@
         Type: DataRepositoryTaskTypeType,
         FileSystemId: str,
         Report: CompletionReportTypeDef,
         Paths: Sequence[str] = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CapacityToRelease: int = ...,
-        ReleaseConfiguration: ReleaseConfigurationTypeDef = ...
+        ReleaseConfiguration: ReleaseConfigurationTypeDef = ...,
     ) -> CreateDataRepositoryTaskResponseTypeDef:
         """
         Creates an Amazon FSx for Lustre data repository task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_data_repository_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_data_repository_task)
         """
@@ -327,15 +327,15 @@
         SubnetIds: Sequence[str],
         ClientRequestToken: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToDataRepositoryAssociations: bool = ...,
         KmsKeyId: str = ...,
         LustreConfiguration: CreateFileCacheLustreConfigurationTypeDef = ...,
-        DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...
+        DataRepositoryAssociations: Sequence[FileCacheDataRepositoryAssociationTypeDef] = ...,
     ) -> CreateFileCacheResponseTypeDef:
         """
         Creates a new Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_file_cache)
         """
@@ -351,15 +351,15 @@
         SecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: CreateFileSystemOntapConfigurationTypeDef = ...,
         FileSystemTypeVersion: str = ...,
-        OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
     ) -> CreateFileSystemResponseTypeDef:
         """
         Creates a new, empty Amazon FSx file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_file_system)
         """
@@ -374,15 +374,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         WindowsConfiguration: CreateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: CreateFileSystemLustreConfigurationTypeDef = ...,
         StorageType: StorageTypeType = ...,
         KmsKeyId: str = ...,
         FileSystemTypeVersion: str = ...,
         OpenZFSConfiguration: CreateFileSystemOpenZFSConfigurationTypeDef = ...,
-        StorageCapacity: int = ...
+        StorageCapacity: int = ...,
     ) -> CreateFileSystemFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for Lustre, Amazon FSx for Windows File Server, or
         Amazon FSx for OpenZFS file system from an existing Amazon FSx
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_file_system_from_backup)
@@ -391,15 +391,15 @@
 
     async def create_snapshot(
         self,
         *,
         Name: str,
         VolumeId: str,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a snapshot of an existing Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_snapshot)
         """
@@ -409,15 +409,15 @@
         *,
         FileSystemId: str,
         Name: str,
         ActiveDirectoryConfiguration: CreateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
         SvmAdminPassword: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...
+        RootVolumeSecurityStyle: StorageVirtualMachineRootVolumeSecurityStyleType = ...,
     ) -> CreateStorageVirtualMachineResponseTypeDef:
         """
         Creates a storage virtual machine (SVM) for an Amazon FSx for ONTAP file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_storage_virtual_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_storage_virtual_machine)
         """
@@ -426,15 +426,15 @@
         self,
         *,
         VolumeType: VolumeTypeType,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...
+        OpenZFSConfiguration: CreateOpenZFSVolumeConfigurationTypeDef = ...,
     ) -> CreateVolumeResponseTypeDef:
         """
         Creates an FSx for ONTAP or Amazon FSx for OpenZFS storage volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#create_volume)
         """
@@ -442,15 +442,15 @@
     async def create_volume_from_backup(
         self,
         *,
         BackupId: str,
         Name: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: CreateOntapVolumeConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateVolumeFromBackupResponseTypeDef:
         """
         Creates a new Amazon FSx for NetApp ONTAP volume from an existing Amazon FSx
         volume
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.create_volume_from_backup)
@@ -468,15 +468,15 @@
         """
 
     async def delete_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
-        DeleteDataInFileSystem: bool = ...
+        DeleteDataInFileSystem: bool = ...,
     ) -> DeleteDataRepositoryAssociationResponseTypeDef:
         """
         Deletes a data repository association on an Amazon FSx for Lustre file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_data_repository_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_data_repository_association)
         """
@@ -494,15 +494,15 @@
     async def delete_file_system(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         WindowsConfiguration: DeleteFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: DeleteFileSystemLustreConfigurationTypeDef = ...,
-        OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: DeleteFileSystemOpenZFSConfigurationTypeDef = ...,
     ) -> DeleteFileSystemResponseTypeDef:
         """
         Deletes a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_file_system)
         """
@@ -529,30 +529,30 @@
 
     async def delete_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: DeleteVolumeOntapConfigurationTypeDef = ...,
-        OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...
+        OpenZFSConfiguration: DeleteVolumeOpenZFSConfigurationTypeDef = ...,
     ) -> DeleteVolumeResponseTypeDef:
         """
         Deletes an Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.delete_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#delete_volume)
         """
 
     async def describe_backups(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBackupsResponseTypeDef:
         """
         Returns the description of a specific Amazon FSx backup, if a `BackupIds` value
         is provided for that
         backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_backups)
@@ -561,15 +561,15 @@
 
     async def describe_data_repository_associations(
         self,
         *,
         AssociationIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDataRepositoryAssociationsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository associations, if one or more `AssociationIds` values are
         provided in the request, or if filters are used in the
         request.
 
@@ -579,15 +579,15 @@
 
     async def describe_data_repository_tasks(
         self,
         *,
         TaskIds: Sequence[str] = ...,
         Filters: Sequence[DataRepositoryTaskFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeDataRepositoryTasksResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for Lustre or Amazon File Cache
         data repository tasks, if one or more `TaskIds` values are provided in the
         request, or if filters are used in the
         request.
 
@@ -609,15 +609,15 @@
 
     async def describe_file_system_aliases(
         self,
         *,
         FileSystemId: str,
         ClientRequestToken: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeFileSystemAliasesResponseTypeDef:
         """
         Returns the DNS aliases that are associated with the specified Amazon FSx for
         Windows File Server file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_file_system_aliases)
@@ -651,15 +651,15 @@
 
     async def describe_snapshots(
         self,
         *,
         SnapshotIds: Sequence[str] = ...,
         Filters: Sequence[SnapshotFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns the description of specific Amazon FSx for OpenZFS snapshots, if a
         `SnapshotIds` value is
         provided.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_snapshots)
@@ -668,15 +668,15 @@
 
     async def describe_storage_virtual_machines(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeStorageVirtualMachinesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP storage virtual machines
         (SVMs).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_storage_virtual_machines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#describe_storage_virtual_machines)
@@ -684,15 +684,15 @@
 
     async def describe_volumes(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeVolumesResponseTypeDef:
         """
         Describes one or more Amazon FSx for NetApp ONTAP or Amazon FSx for OpenZFS
         volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.describe_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#describe_volumes)
@@ -746,15 +746,15 @@
 
     async def restore_volume_from_snapshot(
         self,
         *,
         VolumeId: str,
         SnapshotId: str,
         ClientRequestToken: str = ...,
-        Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...
+        Options: Sequence[RestoreOpenZFSVolumeOptionType] = ...,
     ) -> RestoreVolumeFromSnapshotResponseTypeDef:
         """
         Returns an Amazon FSx for OpenZFS volume to the state saved by the specified
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.restore_volume_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#restore_volume_from_snapshot)
@@ -791,15 +791,15 @@
 
     async def update_data_repository_association(
         self,
         *,
         AssociationId: str,
         ClientRequestToken: str = ...,
         ImportedFileChunkSize: int = ...,
-        S3: S3DataRepositoryConfigurationTypeDef = ...
+        S3: S3DataRepositoryConfigurationTypeDef = ...,
     ) -> UpdateDataRepositoryAssociationResponseTypeDef:
         """
         Updates the configuration of an existing data repository association on an
         Amazon FSx for Lustre file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_data_repository_association)
@@ -807,15 +807,15 @@
         """
 
     async def update_file_cache(
         self,
         *,
         FileCacheId: str,
         ClientRequestToken: str = ...,
-        LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...
+        LustreConfiguration: UpdateFileCacheLustreConfigurationTypeDef = ...,
     ) -> UpdateFileCacheResponseTypeDef:
         """
         Updates the configuration of an existing Amazon File Cache resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_file_cache)
         """
@@ -826,29 +826,29 @@
         FileSystemId: str,
         ClientRequestToken: str = ...,
         StorageCapacity: int = ...,
         WindowsConfiguration: UpdateFileSystemWindowsConfigurationTypeDef = ...,
         LustreConfiguration: UpdateFileSystemLustreConfigurationTypeDef = ...,
         OntapConfiguration: UpdateFileSystemOntapConfigurationTypeDef = ...,
         OpenZFSConfiguration: UpdateFileSystemOpenZFSConfigurationTypeDef = ...,
-        StorageType: StorageTypeType = ...
+        StorageType: StorageTypeType = ...,
     ) -> UpdateFileSystemResponseTypeDef:
         """
         Use this operation to update the configuration of an existing Amazon FSx file
         system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_file_system)
         """
 
     async def update_shared_vpc_configuration(
         self,
         *,
         EnableFsxRouteTableUpdatesFromParticipantAccounts: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> UpdateSharedVpcConfigurationResponseTypeDef:
         """
         Configures whether participant accounts in your organization can create Amazon
         FSx for NetApp ONTAP Multi-AZ file systems in subnets that are shared by a
         virtual private cloud (VPC)
         owner.
 
@@ -868,15 +868,15 @@
 
     async def update_storage_virtual_machine(
         self,
         *,
         StorageVirtualMachineId: str,
         ActiveDirectoryConfiguration: UpdateSvmActiveDirectoryConfigurationTypeDef = ...,
         ClientRequestToken: str = ...,
-        SvmAdminPassword: str = ...
+        SvmAdminPassword: str = ...,
     ) -> UpdateStorageVirtualMachineResponseTypeDef:
         """
         Updates an FSx for ONTAP storage virtual machine (SVM).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_storage_virtual_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/client/#update_storage_virtual_machine)
         """
@@ -884,15 +884,15 @@
     async def update_volume(
         self,
         *,
         VolumeId: str,
         ClientRequestToken: str = ...,
         OntapConfiguration: UpdateOntapVolumeConfigurationTypeDef = ...,
         Name: str = ...,
-        OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...
+        OpenZFSConfiguration: UpdateOpenZFSVolumeConfigurationTypeDef = ...,
     ) -> UpdateVolumeResponseTypeDef:
         """
         Updates the configuration of an Amazon FSx for NetApp ONTAP or Amazon FSx for
         OpenZFS
         volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Client.update_volume)
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/literals.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/literals.py`

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
     "AdministrativeActionTypeType",
     "AliasLifecycleType",
     "AutoImportPolicyTypeType",
     "AutocommitPeriodTypeType",
     "BackupLifecycleType",
     "BackupTypeType",
@@ -88,15 +87,14 @@
     "FSxServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdministrativeActionTypeType = Literal[
     "FILE_SYSTEM_ALIAS_ASSOCIATION",
     "FILE_SYSTEM_ALIAS_DISASSOCIATION",
     "FILE_SYSTEM_UPDATE",
     "IOPS_OPTIMIZATION",
     "MISCONFIGURED_STATE_RECOVERY",
     "RELEASE_NFS_V3_LOCKS",
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/literals.pyi` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/paginator.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,97 +50,90 @@
     "DescribeBackupsPaginator",
     "DescribeFileSystemsPaginator",
     "DescribeStorageVirtualMachinesPaginator",
     "DescribeVolumesPaginator",
     "ListTagsForResourcePaginator",
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
 class DescribeBackupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describebackupspaginator)
     """
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describebackupspaginator)
         """
 
-
 class DescribeFileSystemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
         self, *, FileSystemIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describefilesystemspaginator)
         """
 
-
 class DescribeStorageVirtualMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describestoragevirtualmachinespaginator)
     """
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
-
 class DescribeVolumesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describevolumespaginator)
     """
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describevolumespaginator)
         """
 
-
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/paginator.pyi` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,88 +52,94 @@
     "DescribeStorageVirtualMachinesPaginator",
     "DescribeVolumesPaginator",
     "ListTagsForResourcePaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeBackupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describebackupspaginator)
     """
 
     def paginate(
         self,
         *,
         BackupIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describebackupspaginator)
         """
 
+
 class DescribeFileSystemsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describefilesystemspaginator)
     """
 
     def paginate(
         self, *, FileSystemIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describefilesystemspaginator)
         """
 
+
 class DescribeStorageVirtualMachinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describestoragevirtualmachinespaginator)
     """
 
     def paginate(
         self,
         *,
         StorageVirtualMachineIds: Sequence[str] = ...,
         Filters: Sequence[StorageVirtualMachineFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStorageVirtualMachinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeStorageVirtualMachines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describestoragevirtualmachinespaginator)
         """
 
+
 class DescribeVolumesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describevolumespaginator)
     """
 
     def paginate(
         self,
         *,
         VolumeIds: Sequence[str] = ...,
         Filters: Sequence[VolumeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVolumesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.DescribeVolumes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#describevolumespaginator)
         """
 
+
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/type_defs.py` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveDirectoryBackupAttributesTypeDef",
     "AdministrativeActionFailureDetailsTypeDef",
     "AggregateConfigurationTypeDef",
     "AliasTypeDef",
     "AssociateFileSystemAliasesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx/type_defs.pyi` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/PKG-INFO` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fsx
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.FSx 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.FSx 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/
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
 
 <a id="types-aiobotocore-fsx"></a>
 
 # types-aiobotocore-fsx
 
 [![PyPI - types-aiobotocore-fsx](https://img.shields.io/pypi/v/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fsx.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fsx)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fsx)](https://pepy.tech/project/types-aiobotocore-fsx)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.FSx 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
+[aiobotocore.FSx 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#FSx)
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
 [types-aiobotocore-fsx docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fsx/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-fsx-2.9.0/types_aiobotocore_fsx.egg-info/SOURCES.txt` & `types-aiobotocore-fsx-2.9.1/types_aiobotocore_fsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

