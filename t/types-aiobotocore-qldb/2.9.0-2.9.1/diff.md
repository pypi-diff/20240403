# Comparing `tmp/types-aiobotocore-qldb-2.9.0.tar.gz` & `tmp/types-aiobotocore-qldb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qldb-2.9.0.tar", last modified: Wed Dec 13 20:00:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-qldb-2.9.1.tar", last modified: Thu Jan 18 01:21:33 2024, max compression
```

## Comparing `types-aiobotocore-qldb-2.9.0.tar` & `types-aiobotocore-qldb-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.125289 types-aiobotocore-qldb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2023-12-13 20:00:13.125289 types-aiobotocore-qldb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10573 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:13.125289 types-aiobotocore-qldb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.125289 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      909 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16649 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16646 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9106 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14035 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14034 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:52:08.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:13.125289 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 20:00:13.000000 types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.117104 types-aiobotocore-qldb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-01-18 01:21:33.117104 types-aiobotocore-qldb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:33.117104 types-aiobotocore-qldb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.113104 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16654 2024-01-18 01:13:44.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-01-18 01:13:44.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9104 2024-01-18 01:13:44.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-01-18 01:13:44.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14034 2024-01-18 01:13:44.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:43.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:33.113104 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12144 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:21:33.000000 types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qldb-2.9.0/LICENSE` & `types-aiobotocore-qldb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-qldb-2.9.0/PKG-INFO` & `types-aiobotocore-qldb-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QLDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QLDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
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
 
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QLDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[aiobotocore.QLDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qldb-2.9.0/README.md` & `types-aiobotocore-qldb-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QLDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[aiobotocore.QLDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qldb-2.9.0/setup.py` & `types-aiobotocore-qldb-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qldb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_qldb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.QLDB 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.QLDB 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore qldb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_qldb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/__main__.py` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QLDB 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.QLDB 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB\nOther"
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

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/client.py` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,33 +44,30 @@
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourcePreconditionNotMetException: Type[BotocoreClientError]
 
-
 class QLDBClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/)
     """
 
     meta: ClientMeta
@@ -113,15 +110,15 @@
     async def create_ledger(
         self,
         *,
         Name: str,
         PermissionsMode: PermissionsModeType,
         Tags: Mapping[str, str] = ...,
         DeletionProtection: bool = ...,
-        KmsKey: str = ...
+        KmsKey: str = ...,
     ) -> CreateLedgerResponseTypeDef:
         """
         Creates a new ledger in your Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.create_ledger)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#create_ledger)
         """
@@ -171,15 +168,15 @@
         self,
         *,
         Name: str,
         InclusiveStartTime: TimestampTypeDef,
         ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
-        OutputFormat: OutputFormatType = ...
+        OutputFormat: OutputFormatType = ...,
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.export_journal_to_s3)
@@ -201,15 +198,15 @@
         """
 
     async def get_block(
         self,
         *,
         Name: str,
         BlockAddress: ValueHolderTypeDef,
-        DigestTipAddress: ValueHolderTypeDef = ...
+        DigestTipAddress: ValueHolderTypeDef = ...,
     ) -> GetBlockResponseTypeDef:
         """
         Returns a block object at a specified address in a journal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#get_block)
         """
@@ -224,15 +221,15 @@
 
     async def get_revision(
         self,
         *,
         Name: str,
         BlockAddress: ValueHolderTypeDef,
         DocumentId: str,
-        DigestTipAddress: ValueHolderTypeDef = ...
+        DigestTipAddress: ValueHolderTypeDef = ...,
     ) -> GetRevisionResponseTypeDef:
         """
         Returns a revision data object for a specified document ID and block address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#get_revision)
         """
@@ -296,15 +293,15 @@
         *,
         LedgerName: str,
         RoleArn: str,
         InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: TimestampTypeDef = ...
+        ExclusiveEndTime: TimestampTypeDef = ...,
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/client.pyi` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,30 +44,33 @@
     UpdateLedgerPermissionsModeResponseTypeDef,
     UpdateLedgerResponseTypeDef,
     ValueHolderTypeDef,
 )
 
 __all__ = ("QLDBClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     InvalidParameterException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceAlreadyExistsException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourcePreconditionNotMetException: Type[BotocoreClientError]
 
+
 class QLDBClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/)
     """
 
     meta: ClientMeta
@@ -110,15 +113,15 @@
     async def create_ledger(
         self,
         *,
         Name: str,
         PermissionsMode: PermissionsModeType,
         Tags: Mapping[str, str] = ...,
         DeletionProtection: bool = ...,
-        KmsKey: str = ...
+        KmsKey: str = ...,
     ) -> CreateLedgerResponseTypeDef:
         """
         Creates a new ledger in your Amazon Web Services account in the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.create_ledger)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#create_ledger)
         """
@@ -168,15 +171,15 @@
         self,
         *,
         Name: str,
         InclusiveStartTime: TimestampTypeDef,
         ExclusiveEndTime: TimestampTypeDef,
         S3ExportConfiguration: S3ExportConfigurationTypeDef,
         RoleArn: str,
-        OutputFormat: OutputFormatType = ...
+        OutputFormat: OutputFormatType = ...,
     ) -> ExportJournalToS3ResponseTypeDef:
         """
         Exports journal contents within a date and time range from a ledger into a
         specified Amazon Simple Storage Service (Amazon S3)
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.export_journal_to_s3)
@@ -198,15 +201,15 @@
         """
 
     async def get_block(
         self,
         *,
         Name: str,
         BlockAddress: ValueHolderTypeDef,
-        DigestTipAddress: ValueHolderTypeDef = ...
+        DigestTipAddress: ValueHolderTypeDef = ...,
     ) -> GetBlockResponseTypeDef:
         """
         Returns a block object at a specified address in a journal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_block)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#get_block)
         """
@@ -221,15 +224,15 @@
 
     async def get_revision(
         self,
         *,
         Name: str,
         BlockAddress: ValueHolderTypeDef,
         DocumentId: str,
-        DigestTipAddress: ValueHolderTypeDef = ...
+        DigestTipAddress: ValueHolderTypeDef = ...,
     ) -> GetRevisionResponseTypeDef:
         """
         Returns a revision data object for a specified document ID and block address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.get_revision)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#get_revision)
         """
@@ -293,15 +296,15 @@
         *,
         LedgerName: str,
         RoleArn: str,
         InclusiveStartTime: TimestampTypeDef,
         KinesisConfiguration: KinesisConfigurationTypeDef,
         StreamName: str,
         Tags: Mapping[str, str] = ...,
-        ExclusiveEndTime: TimestampTypeDef = ...
+        ExclusiveEndTime: TimestampTypeDef = ...,
     ) -> StreamJournalToKinesisResponseTypeDef:
         """
         Creates a journal stream for a given Amazon QLDB ledger.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB.Client.stream_journal_to_kinesis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/client/#stream_journal_to_kinesis)
         """
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/literals.py` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/literals.py`

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
     "EncryptionStatusType",
     "ErrorCauseType",
     "ExportStatusType",
     "LedgerStateType",
     "OutputFormatType",
     "PermissionsModeType",
@@ -31,15 +30,14 @@
     "StreamStatusType",
     "QLDBServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 EncryptionStatusType = Literal["ENABLED", "KMS_KEY_INACCESSIBLE", "UPDATING"]
 ErrorCauseType = Literal["IAM_PERMISSION_REVOKED", "KINESIS_STREAM_NOT_FOUND"]
 ExportStatusType = Literal["CANCELLED", "COMPLETED", "IN_PROGRESS"]
 LedgerStateType = Literal["ACTIVE", "CREATING", "DELETED", "DELETING"]
 OutputFormatType = Literal["ION_BINARY", "ION_TEXT", "JSON"]
 PermissionsModeType = Literal["ALLOW_ALL", "STANDARD"]
 S3ObjectEncryptionTypeType = Literal["NO_ENCRYPTION", "SSE_KMS", "SSE_S3"]
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/literals.pyi` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/type_defs.py` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelJournalKinesisStreamRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateLedgerRequestRequestTypeDef",
     "DeleteLedgerRequestRequestTypeDef",
     "DescribeJournalKinesisStreamRequestRequestTypeDef",
     "DescribeJournalS3ExportRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb/type_defs.pyi` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/PKG-INFO` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.QLDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.QLDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/
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
 
 <a id="types-aiobotocore-qldb"></a>
 
 # types-aiobotocore-qldb
 
 [![PyPI - types-aiobotocore-qldb](https://img.shields.io/pypi/v/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-qldb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-qldb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-qldb)](https://pepy.tech/project/types-aiobotocore-qldb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.QLDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
+[aiobotocore.QLDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#QLDB)
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
 [types-aiobotocore-qldb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-qldb-2.9.0/types_aiobotocore_qldb.egg-info/SOURCES.txt` & `types-aiobotocore-qldb-2.9.1/types_aiobotocore_qldb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

