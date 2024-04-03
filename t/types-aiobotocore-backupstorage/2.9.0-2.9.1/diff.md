# Comparing `tmp/types-aiobotocore-backupstorage-2.9.0.tar.gz` & `tmp/types-aiobotocore-backupstorage-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backupstorage-2.9.0.tar", last modified: Wed Dec 13 19:58:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-backupstorage-2.9.1.tar", last modified: Thu Jan 18 01:20:08 2024, max compression
```

## Comparing `types-aiobotocore-backupstorage-2.9.0.tar` & `types-aiobotocore-backupstorage-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.618045 types-aiobotocore-backupstorage-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2023-12-13 19:58:40.618045 types-aiobotocore-backupstorage-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:40.618045 types-aiobotocore-backupstorage-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:41:36.000000 types-aiobotocore-backupstorage-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.618045 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10962 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8855 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7215 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:37.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:40.618045 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12557 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      836 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:58:40.000000 types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.189495 types-aiobotocore-backupstorage-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-01-18 01:20:08.189495 types-aiobotocore-backupstorage-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:08.189495 types-aiobotocore-backupstorage-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.189495 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10962 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8855 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:35.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:08.189495 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12577 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:08.000000 types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/LICENSE` & `types-aiobotocore-backupstorage-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-backupstorage-2.9.0/PKG-INFO` & `types-aiobotocore-backupstorage-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BackupStorage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BackupStorage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
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
 
 <a id="types-aiobotocore-backupstorage"></a>
 
 # types-aiobotocore-backupstorage
 
 [![PyPI - types-aiobotocore-backupstorage](https://img.shields.io/pypi/v/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/README.md` & `types-aiobotocore-backupstorage-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/setup.py` & `types-aiobotocore-backupstorage-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backupstorage",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.BackupStorage 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.BackupStorage 2.9.1 service generated with"
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
     keywords="aiobotocore backupstorage type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backupstorage": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/__main__.py` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.BackupStorage 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.BackupStorage 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/client.py` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BackupStorageClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -157,15 +156,15 @@
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         CreatedBefore: TimestampTypeDef = ...,
-        CreatedAfter: TimestampTypeDef = ...
+        CreatedAfter: TimestampTypeDef = ...,
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_objects)
         """
@@ -177,15 +176,15 @@
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
         MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
-        MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
+        MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...,
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.notify_object_complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#notify_object_complete)
@@ -196,15 +195,15 @@
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
         Data: BlobTypeDef,
         Length: int,
         Checksum: str,
-        ChecksumAlgorithm: Literal["SHA256"]
+        ChecksumAlgorithm: Literal["SHA256"],
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_chunk)
         """
@@ -217,15 +216,15 @@
         MetadataString: str = ...,
         InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
-        ThrowOnDuplicate: bool = ...
+        ThrowOnDuplicate: bool = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Upload object that can store object metadata String and data blob in single API
         call using inline chunk
         field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_object)
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/client.pyi` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         CreatedBefore: TimestampTypeDef = ...,
-        CreatedAfter: TimestampTypeDef = ...
+        CreatedAfter: TimestampTypeDef = ...,
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_objects)
         """
@@ -173,15 +173,15 @@
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
         MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
-        MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
+        MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...,
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.notify_object_complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#notify_object_complete)
@@ -192,15 +192,15 @@
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
         Data: BlobTypeDef,
         Length: int,
         Checksum: str,
-        ChecksumAlgorithm: Literal["SHA256"]
+        ChecksumAlgorithm: Literal["SHA256"],
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_chunk)
         """
@@ -213,15 +213,15 @@
         MetadataString: str = ...,
         InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
-        ThrowOnDuplicate: bool = ...
+        ThrowOnDuplicate: bool = ...,
     ) -> PutObjectOutputTypeDef:
         """
         Upload object that can store object metadata String and data blob in single API
         call using inline chunk
         field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_object)
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/literals.py` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DataChecksumAlgorithmType",
     "SummaryChecksumAlgorithmType",
     "BackupStorageServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DataChecksumAlgorithmType = Literal["SHA256"]
 SummaryChecksumAlgorithmType = Literal["SUMMARY"]
 BackupStorageServiceName = Literal["backupstorage"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/literals.pyi` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/type_defs.py` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BackupObjectTypeDef",
     "BlobTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage/type_defs.pyi` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/PKG-INFO` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.BackupStorage 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.BackupStorage 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
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
 
 <a id="types-aiobotocore-backupstorage"></a>
 
 # types-aiobotocore-backupstorage
 
 [![PyPI - types-aiobotocore-backupstorage](https://img.shields.io/pypi/v/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.BackupStorage 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[aiobotocore.BackupStorage 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-backupstorage-2.9.0/types_aiobotocore_backupstorage.egg-info/SOURCES.txt` & `types-aiobotocore-backupstorage-2.9.1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

