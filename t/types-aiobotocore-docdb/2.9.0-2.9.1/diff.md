# Comparing `tmp/types-aiobotocore-docdb-2.9.0.tar.gz` & `tmp/types-aiobotocore-docdb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-2.9.0.tar", last modified: Wed Dec 13 19:59:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-2.9.1.tar", last modified: Thu Jan 18 01:20:33 2024, max compression
```

## Comparing `types-aiobotocore-docdb-2.9.0.tar` & `types-aiobotocore-docdb-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.317819 types-aiobotocore-docdb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2023-12-13 19:59:08.317819 types-aiobotocore-docdb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14439 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:08.317819 types-aiobotocore-docdb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.317819 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54033 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54029 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2023-12-13 19:44:21.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11317 2023-12-13 19:44:20.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18072 2023-12-13 19:44:20.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    18057 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56474 2023-12-13 19:44:22.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56473 2023-12-13 19:44:21.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:19.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-12-13 19:44:20.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-12-13 19:44:20.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:08.317819 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15994 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 19:59:08.000000 types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.593377 types-aiobotocore-docdb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-01-18 01:20:33.593377 types-aiobotocore-docdb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14439 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:33.593377 types-aiobotocore-docdb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.593377 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54065 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54062 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11317 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18084 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18070 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56473 2024-01-18 01:06:17.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:14.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-01-18 01:06:15.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:33.593377 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:20:33.000000 types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-2.9.0/LICENSE` & `types-aiobotocore-docdb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-docdb-2.9.0/PKG-INFO` & `types-aiobotocore-docdb-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DocDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DocDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
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
 
 <a id="types-aiobotocore-docdb"></a>
 
 # types-aiobotocore-docdb
 
 [![PyPI - types-aiobotocore-docdb](https://img.shields.io/pypi/v/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-2.9.0/README.md` & `types-aiobotocore-docdb-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-2.9.0/setup.py` & `types-aiobotocore-docdb-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_docdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DocDB 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DocDB 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore docdb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_docdb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/__init__.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     DescribeOrderableDBInstanceOptionsPaginator,
     DescribePendingMaintenanceActionsPaginator,
 )
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 Client = DocDBClient
 
-
 __all__ = (
     "Client",
     "DBInstanceAvailableWaiter",
     "DBInstanceDeletedWaiter",
     "DescribeCertificatesPaginator",
     "DescribeDBClusterParameterGroupsPaginator",
     "DescribeDBClusterParametersPaginator",
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/__init__.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/client.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,14 @@
 from .waiter import DBInstanceAvailableWaiter, DBInstanceDeletedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DocDBClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -240,15 +239,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#copy_db_cluster_parameter_group)
         """
@@ -258,15 +257,15 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#copy_db_cluster_snapshot)
         """
@@ -291,44 +290,44 @@
         StorageEncrypted: bool = ...,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         GlobalClusterIdentifier: str = ...,
         StorageType: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster)
         """
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster_snapshot)
         """
@@ -344,30 +343,30 @@
         PreferredMaintenanceWindow: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToSnapshot: bool = ...,
         PromotionTier: int = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
-        CACertificateIdentifier: str = ...
+        CACertificateIdentifier: str = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_instance)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_subnet_group)
         """
@@ -377,15 +376,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon DocumentDB event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_event_subscription)
         """
@@ -395,15 +394,15 @@
         *,
         GlobalClusterIdentifier: str,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
         DatabaseName: str = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates an Amazon DocumentDB global cluster that can span multiple multiple
         Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_global_cluster)
@@ -411,15 +410,15 @@
         """
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         Deletes a previously provisioned cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#delete_db_cluster)
         """
@@ -486,15 +485,15 @@
 
     async def describe_certificates(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CertificateMessageTypeDef:
         """
         Returns a list of certificate authority (CA) certificates provided by Amazon
         DocumentDB for this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_certificates)
@@ -503,15 +502,15 @@
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_parameter_groups)
         """
@@ -519,15 +518,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_parameters)
         """
@@ -550,30 +549,30 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_snapshots)
         """
 
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Returns information about provisioned Amazon DocumentDB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_clusters)
         """
@@ -585,60 +584,60 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
-        ListSupportedTimezones: bool = ...
+        ListSupportedTimezones: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Returns a list of the available engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_engine_versions)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Returns information about provisioned Amazon DocumentDB instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_instances)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of `DBSubnetGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_engine_default_cluster_parameters)
@@ -659,15 +658,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_event_subscriptions)
         """
@@ -679,15 +678,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to instances, security groups, snapshots, and DB
         parameter groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_events)
@@ -696,15 +695,15 @@
 
     async def describe_global_clusters(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GlobalClustersMessageTypeDef:
         """
         Returns information about Amazon DocumentDB global clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_global_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_global_clusters)
         """
@@ -715,30 +714,30 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Returns a list of orderable instance options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_pending_maintenance_actions)
@@ -792,15 +791,15 @@
         MasterUserPassword: str = ...,
         PreferredBackupWindow: str = ...,
         PreferredMaintenanceWindow: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         DeletionProtection: bool = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies a setting for an Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_cluster)
         """
@@ -817,15 +816,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster_snapshot_attribute)
@@ -842,29 +841,29 @@
         AutoMinorVersionUpgrade: bool = ...,
         NewDBInstanceIdentifier: str = ...,
         CACertificateIdentifier: str = ...,
         CopyTagsToSnapshot: bool = ...,
         PromotionTier: int = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
-        CertificateRotationRestart: bool = ...
+        CertificateRotationRestart: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_instance)
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_subnet_group)
         """
@@ -872,29 +871,29 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon DocumentDB event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_event_subscription)
         """
 
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         NewGlobalClusterIdentifier: str = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modify a setting for an Amazon DocumentDB global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_global_cluster)
         """
@@ -942,15 +941,15 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#reset_db_cluster_parameter_group)
         """
@@ -967,15 +966,15 @@
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         DBClusterParameterGroupName: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot or cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#restore_db_cluster_from_snapshot)
         """
@@ -991,15 +990,15 @@
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#restore_db_cluster_to_point_in_time)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/client.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
     async def copy_db_cluster_parameter_group(
         self,
         *,
         SourceDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupIdentifier: str,
         TargetDBClusterParameterGroupDescription: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopyDBClusterParameterGroupResultTypeDef:
         """
         Copies the specified cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#copy_db_cluster_parameter_group)
         """
@@ -254,15 +254,15 @@
         *,
         SourceDBClusterSnapshotIdentifier: str,
         TargetDBClusterSnapshotIdentifier: str,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         CopyTags: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CopyDBClusterSnapshotResultTypeDef:
         """
         Copies a snapshot of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.copy_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#copy_db_cluster_snapshot)
         """
@@ -287,44 +287,44 @@
         StorageEncrypted: bool = ...,
         KmsKeyId: str = ...,
         PreSignedUrl: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         GlobalClusterIdentifier: str = ...,
         StorageType: str = ...,
-        SourceRegion: str = ...
+        SourceRegion: str = ...,
     ) -> CreateDBClusterResultTypeDef:
         """
         Creates a new Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster)
         """
 
     async def create_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         DBParameterGroupFamily: str,
         Description: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterParameterGroupResultTypeDef:
         """
         Creates a new cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster_parameter_group)
         """
 
     async def create_db_cluster_snapshot(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         DBClusterIdentifier: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBClusterSnapshotResultTypeDef:
         """
         Creates a snapshot of a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_cluster_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_cluster_snapshot)
         """
@@ -340,30 +340,30 @@
         PreferredMaintenanceWindow: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         CopyTagsToSnapshot: bool = ...,
         PromotionTier: int = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
-        CACertificateIdentifier: str = ...
+        CACertificateIdentifier: str = ...,
     ) -> CreateDBInstanceResultTypeDef:
         """
         Creates a new instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_instance)
         """
 
     async def create_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         DBSubnetGroupDescription: str,
         SubnetIds: Sequence[str],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDBSubnetGroupResultTypeDef:
         """
         Creates a new subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_db_subnet_group)
         """
@@ -373,15 +373,15 @@
         *,
         SubscriptionName: str,
         SnsTopicArn: str,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
         SourceIds: Sequence[str] = ...,
         Enabled: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEventSubscriptionResultTypeDef:
         """
         Creates an Amazon DocumentDB event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#create_event_subscription)
         """
@@ -391,15 +391,15 @@
         *,
         GlobalClusterIdentifier: str,
         SourceDBClusterIdentifier: str = ...,
         Engine: str = ...,
         EngineVersion: str = ...,
         DeletionProtection: bool = ...,
         DatabaseName: str = ...,
-        StorageEncrypted: bool = ...
+        StorageEncrypted: bool = ...,
     ) -> CreateGlobalClusterResultTypeDef:
         """
         Creates an Amazon DocumentDB global cluster that can span multiple multiple
         Amazon Web Services
         Regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.create_global_cluster)
@@ -407,15 +407,15 @@
         """
 
     async def delete_db_cluster(
         self,
         *,
         DBClusterIdentifier: str,
         SkipFinalSnapshot: bool = ...,
-        FinalDBSnapshotIdentifier: str = ...
+        FinalDBSnapshotIdentifier: str = ...,
     ) -> DeleteDBClusterResultTypeDef:
         """
         Deletes a previously provisioned cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.delete_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#delete_db_cluster)
         """
@@ -482,15 +482,15 @@
 
     async def describe_certificates(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> CertificateMessageTypeDef:
         """
         Returns a list of certificate authority (CA) certificates provided by Amazon
         DocumentDB for this Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_certificates)
@@ -499,15 +499,15 @@
 
     async def describe_db_cluster_parameter_groups(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupsMessageTypeDef:
         """
         Returns a list of `DBClusterParameterGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_parameter_groups)
         """
@@ -515,15 +515,15 @@
     async def describe_db_cluster_parameters(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterParameterGroupDetailsTypeDef:
         """
         Returns the detailed parameter list for a particular cluster parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_parameters)
         """
@@ -546,30 +546,30 @@
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         IncludeShared: bool = ...,
-        IncludePublic: bool = ...
+        IncludePublic: bool = ...,
     ) -> DBClusterSnapshotMessageTypeDef:
         """
         Returns information about cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_cluster_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_cluster_snapshots)
         """
 
     async def describe_db_clusters(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBClusterMessageTypeDef:
         """
         Returns information about provisioned Amazon DocumentDB clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_clusters)
         """
@@ -581,60 +581,60 @@
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
-        ListSupportedTimezones: bool = ...
+        ListSupportedTimezones: bool = ...,
     ) -> DBEngineVersionMessageTypeDef:
         """
         Returns a list of the available engines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_engine_versions)
         """
 
     async def describe_db_instances(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBInstanceMessageTypeDef:
         """
         Returns information about provisioned Amazon DocumentDB instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_instances)
         """
 
     async def describe_db_subnet_groups(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DBSubnetGroupMessageTypeDef:
         """
         Returns a list of `DBSubnetGroup` descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_db_subnet_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_db_subnet_groups)
         """
 
     async def describe_engine_default_cluster_parameters(
         self,
         *,
         DBParameterGroupFamily: str,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> DescribeEngineDefaultClusterParametersResultTypeDef:
         """
         Returns the default engine and system parameter information for the cluster
         database
         engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_engine_default_cluster_parameters)
@@ -655,15 +655,15 @@
 
     async def describe_event_subscriptions(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventSubscriptionsMessageTypeDef:
         """
         Lists all the subscription descriptions for a customer account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_event_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_event_subscriptions)
         """
@@ -675,15 +675,15 @@
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> EventsMessageTypeDef:
         """
         Returns events related to instances, security groups, snapshots, and DB
         parameter groups for the past 14
         days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_events)
@@ -692,15 +692,15 @@
 
     async def describe_global_clusters(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> GlobalClustersMessageTypeDef:
         """
         Returns information about Amazon DocumentDB global clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_global_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_global_clusters)
         """
@@ -711,30 +711,30 @@
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
-        Marker: str = ...
+        Marker: str = ...,
     ) -> OrderableDBInstanceOptionsMessageTypeDef:
         """
         Returns a list of orderable instance options for the specified engine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_orderable_db_instance_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#describe_orderable_db_instance_options)
         """
 
     async def describe_pending_maintenance_actions(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         Marker: str = ...,
-        MaxRecords: int = ...
+        MaxRecords: int = ...,
     ) -> PendingMaintenanceActionsMessageTypeDef:
         """
         Returns a list of resources (for example, instances) that have at least one
         pending maintenance
         action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.describe_pending_maintenance_actions)
@@ -788,15 +788,15 @@
         MasterUserPassword: str = ...,
         PreferredBackupWindow: str = ...,
         PreferredMaintenanceWindow: str = ...,
         CloudwatchLogsExportConfiguration: CloudwatchLogsExportConfigurationTypeDef = ...,
         EngineVersion: str = ...,
         AllowMajorVersionUpgrade: bool = ...,
         DeletionProtection: bool = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> ModifyDBClusterResultTypeDef:
         """
         Modifies a setting for an Amazon DocumentDB cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_cluster)
         """
@@ -813,15 +813,15 @@
 
     async def modify_db_cluster_snapshot_attribute(
         self,
         *,
         DBClusterSnapshotIdentifier: str,
         AttributeName: str,
         ValuesToAdd: Sequence[str] = ...,
-        ValuesToRemove: Sequence[str] = ...
+        ValuesToRemove: Sequence[str] = ...,
     ) -> ModifyDBClusterSnapshotAttributeResultTypeDef:
         """
         Adds an attribute and values to, or removes an attribute and values from, a
         manual cluster
         snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_cluster_snapshot_attribute)
@@ -838,29 +838,29 @@
         AutoMinorVersionUpgrade: bool = ...,
         NewDBInstanceIdentifier: str = ...,
         CACertificateIdentifier: str = ...,
         CopyTagsToSnapshot: bool = ...,
         PromotionTier: int = ...,
         EnablePerformanceInsights: bool = ...,
         PerformanceInsightsKMSKeyId: str = ...,
-        CertificateRotationRestart: bool = ...
+        CertificateRotationRestart: bool = ...,
     ) -> ModifyDBInstanceResultTypeDef:
         """
         Modifies settings for an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_instance)
         """
 
     async def modify_db_subnet_group(
         self,
         *,
         DBSubnetGroupName: str,
         SubnetIds: Sequence[str],
-        DBSubnetGroupDescription: str = ...
+        DBSubnetGroupDescription: str = ...,
     ) -> ModifyDBSubnetGroupResultTypeDef:
         """
         Modifies an existing subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_db_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_db_subnet_group)
         """
@@ -868,29 +868,29 @@
     async def modify_event_subscription(
         self,
         *,
         SubscriptionName: str,
         SnsTopicArn: str = ...,
         SourceType: str = ...,
         EventCategories: Sequence[str] = ...,
-        Enabled: bool = ...
+        Enabled: bool = ...,
     ) -> ModifyEventSubscriptionResultTypeDef:
         """
         Modifies an existing Amazon DocumentDB event notification subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_event_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_event_subscription)
         """
 
     async def modify_global_cluster(
         self,
         *,
         GlobalClusterIdentifier: str,
         NewGlobalClusterIdentifier: str = ...,
-        DeletionProtection: bool = ...
+        DeletionProtection: bool = ...,
     ) -> ModifyGlobalClusterResultTypeDef:
         """
         Modify a setting for an Amazon DocumentDB global cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.modify_global_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#modify_global_cluster)
         """
@@ -938,15 +938,15 @@
         """
 
     async def reset_db_cluster_parameter_group(
         self,
         *,
         DBClusterParameterGroupName: str,
         ResetAllParameters: bool = ...,
-        Parameters: Sequence[ParameterTypeDef] = ...
+        Parameters: Sequence[ParameterTypeDef] = ...,
     ) -> DBClusterParameterGroupNameMessageTypeDef:
         """
         Modifies the parameters of a cluster parameter group to the default value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.reset_db_cluster_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#reset_db_cluster_parameter_group)
         """
@@ -963,15 +963,15 @@
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
         DBClusterParameterGroupName: str = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterFromSnapshotResultTypeDef:
         """
         Creates a new cluster from a snapshot or cluster snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_from_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#restore_db_cluster_from_snapshot)
         """
@@ -987,15 +987,15 @@
         Port: int = ...,
         DBSubnetGroupName: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         EnableCloudwatchLogsExports: Sequence[str] = ...,
         DeletionProtection: bool = ...,
-        StorageType: str = ...
+        StorageType: str = ...,
     ) -> RestoreDBClusterToPointInTimeResultTypeDef:
         """
         Restores a cluster to an arbitrary point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Client.restore_db_cluster_to_point_in_time)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/client/#restore_db_cluster_to_point_in_time)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/literals.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/literals.py`

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
     "ApplyMethodType",
     "DBInstanceAvailableWaiterName",
     "DBInstanceDeletedWaiterName",
     "DescribeCertificatesPaginatorName",
     "DescribeDBClusterParameterGroupsPaginatorName",
     "DescribeDBClusterParametersPaginatorName",
@@ -42,15 +41,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ApplyMethodType = Literal["immediate", "pending-reboot"]
 DBInstanceAvailableWaiterName = Literal["db_instance_available"]
 DBInstanceDeletedWaiterName = Literal["db_instance_deleted"]
 DescribeCertificatesPaginatorName = Literal["describe_certificates"]
 DescribeDBClusterParameterGroupsPaginatorName = Literal["describe_db_cluster_parameter_groups"]
 DescribeDBClusterParametersPaginatorName = Literal["describe_db_cluster_parameters"]
 DescribeDBClusterSnapshotsPaginatorName = Literal["describe_db_cluster_snapshots"]
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/literals.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/paginator.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
     "DescribeEventSubscriptionsPaginator",
     "DescribeEventsPaginator",
     "DescribeGlobalClustersPaginator",
     "DescribeOrderableDBInstanceOptionsPaginator",
     "DescribePendingMaintenanceActionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -104,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describecertificatespaginator)
         """
 
 
@@ -123,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 
@@ -143,15 +142,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 
@@ -166,15 +165,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 
@@ -185,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterspaginator)
         """
 
 
@@ -209,15 +208,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbengineversionspaginator)
         """
 
 
@@ -228,15 +227,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbinstancespaginator)
         """
 
 
@@ -247,15 +246,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 
@@ -266,15 +265,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 
@@ -290,15 +289,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventspaginator)
         """
 
 
@@ -309,15 +308,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 
@@ -332,15 +331,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 
@@ -351,13 +350,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/paginator.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         CertificateIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[CertificateMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeCertificates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describecertificatespaginator)
         """
 
 class DescribeDBClusterParameterGroupsPaginator(AioPaginator):
@@ -119,15 +119,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparametergroupspaginator)
         """
 
 class DescribeDBClusterParametersPaginator(AioPaginator):
@@ -138,15 +138,15 @@
 
     def paginate(
         self,
         *,
         DBClusterParameterGroupName: str,
         Source: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterParameterGroupDetailsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterparameterspaginator)
         """
 
 class DescribeDBClusterSnapshotsPaginator(AioPaginator):
@@ -160,15 +160,15 @@
         *,
         DBClusterIdentifier: str = ...,
         DBClusterSnapshotIdentifier: str = ...,
         SnapshotType: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         IncludeShared: bool = ...,
         IncludePublic: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterSnapshotMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusterSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclustersnapshotspaginator)
         """
 
 class DescribeDBClustersPaginator(AioPaginator):
@@ -178,15 +178,15 @@
     """
 
     def paginate(
         self,
         *,
         DBClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBClusterMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbclusterspaginator)
         """
 
 class DescribeDBEngineVersionsPaginator(AioPaginator):
@@ -201,15 +201,15 @@
         Engine: str = ...,
         EngineVersion: str = ...,
         DBParameterGroupFamily: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         DefaultOnly: bool = ...,
         ListSupportedCharacterSets: bool = ...,
         ListSupportedTimezones: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBEngineVersionMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbengineversionspaginator)
         """
 
 class DescribeDBInstancesPaginator(AioPaginator):
@@ -219,15 +219,15 @@
     """
 
     def paginate(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBInstanceMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbinstancespaginator)
         """
 
 class DescribeDBSubnetGroupsPaginator(AioPaginator):
@@ -237,15 +237,15 @@
     """
 
     def paginate(
         self,
         *,
         DBSubnetGroupName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DBSubnetGroupMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeDBSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describedbsubnetgroupspaginator)
         """
 
 class DescribeEventSubscriptionsPaginator(AioPaginator):
@@ -255,15 +255,15 @@
     """
 
     def paginate(
         self,
         *,
         SubscriptionName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventSubscriptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEventSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventsubscriptionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -278,15 +278,15 @@
         SourceIdentifier: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         EventCategories: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[EventsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeeventspaginator)
         """
 
 class DescribeGlobalClustersPaginator(AioPaginator):
@@ -296,15 +296,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalClusterIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GlobalClustersMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeGlobalClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeglobalclusterspaginator)
         """
 
 class DescribeOrderableDBInstanceOptionsPaginator(AioPaginator):
@@ -318,15 +318,15 @@
         *,
         Engine: str,
         EngineVersion: str = ...,
         DBInstanceClass: str = ...,
         LicenseModel: str = ...,
         Vpc: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[OrderableDBInstanceOptionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribeOrderableDBInstanceOptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describeorderabledbinstanceoptionspaginator)
         """
 
 class DescribePendingMaintenanceActionsPaginator(AioPaginator):
@@ -336,13 +336,13 @@
     """
 
     def paginate(
         self,
         *,
         ResourceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[PendingMaintenanceActionsMessageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Paginator.DescribePendingMaintenanceActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/paginators/#describependingmaintenanceactionspaginator)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/type_defs.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddSourceIdentifierToSubscriptionMessageRequestTypeDef",
     "EventSubscriptionTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplyPendingMaintenanceActionMessageRequestTypeDef",
     "AvailabilityZoneTypeDef",
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/type_defs.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/waiter.py` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/waiters/#dbinstanceavailablewaiter)
         """
 
 
@@ -62,13 +62,13 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/waiters/#dbinstancedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb/waiter.pyi` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/waiters/#dbinstanceavailablewaiter)
         """
 
 class DBInstanceDeletedWaiter(AIOWaiter):
@@ -60,13 +60,13 @@
     async def wait(
         self,
         *,
         DBInstanceIdentifier: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxRecords: int = ...,
         Marker: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB.Waiter.DBInstanceDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/waiters/#dbinstancedeletedwaiter)
         """
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/PKG-INFO` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DocDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DocDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/
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
 
 <a id="types-aiobotocore-docdb"></a>
 
 # types-aiobotocore-docdb
 
 [![PyPI - types-aiobotocore-docdb](https://img.shields.io/pypi/v/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-docdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-docdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-docdb)](https://pepy.tech/project/types-aiobotocore-docdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DocDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
+[aiobotocore.DocDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#DocDB)
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
 [types-aiobotocore-docdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-docdb-2.9.0/types_aiobotocore_docdb.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-2.9.1/types_aiobotocore_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

