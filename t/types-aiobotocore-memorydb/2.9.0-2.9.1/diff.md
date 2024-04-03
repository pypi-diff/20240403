# Comparing `tmp/types-aiobotocore-memorydb-2.9.0.tar.gz` & `tmp/types-aiobotocore-memorydb-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-memorydb-2.9.0.tar", last modified: Wed Dec 13 19:59:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-memorydb-2.9.1.tar", last modified: Thu Jan 18 01:21:17 2024, max compression
```

## Comparing `types-aiobotocore-memorydb-2.9.0.tar` & `types-aiobotocore-memorydb-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.093436 types-aiobotocore-memorydb-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14770 2023-12-13 19:59:56.093436 types-aiobotocore-memorydb-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:56.093436 types-aiobotocore-memorydb-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.093436 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38450 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    38446 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10788 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10786 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15802 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    15788 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    38953 2023-12-13 19:50:26.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    38952 2023-12-13 19:50:25.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:23.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:56.093436 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14770 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:56.000000 types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.765174 types-aiobotocore-memorydb-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-01-18 01:21:17.765174 types-aiobotocore-memorydb-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:17.765174 types-aiobotocore-memorydb-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.761174 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38468 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38465 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10786 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    38952 2024-01-18 01:12:08.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38952 2024-01-18 01:12:07.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:06.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:17.765174 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14790 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:17.000000 types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-memorydb-2.9.0/LICENSE` & `types-aiobotocore-memorydb-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-memorydb-2.9.0/PKG-INFO` & `types-aiobotocore-memorydb-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-memorydb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MemoryDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MemoryDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/
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
 
 <a id="types-aiobotocore-memorydb"></a>
 
 # types-aiobotocore-memorydb
 
 [![PyPI - types-aiobotocore-memorydb](https://img.shields.io/pypi/v/types-aiobotocore-memorydb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-memorydb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-memorydb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-memorydb)](https://pepy.tech/project/types-aiobotocore-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MemoryDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[aiobotocore.MemoryDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [types-aiobotocore-memorydb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-memorydb-2.9.0/README.md` & `types-aiobotocore-memorydb-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-memorydb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-memorydb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-memorydb)](https://pepy.tech/project/types-aiobotocore-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MemoryDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[aiobotocore.MemoryDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [types-aiobotocore-memorydb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-memorydb-2.9.0/setup.py` & `types-aiobotocore-memorydb-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-memorydb",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_memorydb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MemoryDB 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.MemoryDB 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore memorydb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_memorydb": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__init__.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     DescribeSnapshotsPaginator,
     DescribeSubnetGroupsPaginator,
     DescribeUsersPaginator,
 )
 
 Client = MemoryDBClient
 
-
 __all__ = (
     "Client",
     "DescribeACLsPaginator",
     "DescribeClustersPaginator",
     "DescribeEngineVersionsPaginator",
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__init__.pyi` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/__main__.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MemoryDB 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MemoryDB 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB\nOther"
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

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/client.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MemoryDBClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -205,15 +204,15 @@
     async def copy_snapshot(
         self,
         *,
         SourceSnapshotName: str,
         TargetSnapshotName: str,
         TargetBucket: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopySnapshotResponseTypeDef:
         """
         Makes a copy of an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#copy_snapshot)
         """
@@ -248,75 +247,75 @@
         SnapshotArns: Sequence[str] = ...,
         SnapshotName: str = ...,
         SnapshotRetentionLimit: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SnapshotWindow: str = ...,
         EngineVersion: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
-        DataTiering: bool = ...
+        DataTiering: bool = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_cluster)
         """
 
     async def create_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         Family: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateParameterGroupResponseTypeDef:
         """
         Creates a new MemoryDB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_parameter_group)
         """
 
     async def create_snapshot(
         self,
         *,
         ClusterName: str,
         SnapshotName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a copy of an entire cluster at a specific moment in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_snapshot)
         """
 
     async def create_subnet_group(
         self,
         *,
         SubnetGroupName: str,
         SubnetIds: Sequence[str],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSubnetGroupResponseTypeDef:
         """
         Creates a subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_subnet_group)
         """
 
     async def create_user(
         self,
         *,
         UserName: str,
         AuthenticationMode: AuthenticationModeTypeDef,
         AccessString: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a MemoryDB user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_user)
         """
@@ -388,15 +387,15 @@
 
     async def describe_clusters(
         self,
         *,
         ClusterName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ShowShardDetails: bool = ...
+        ShowShardDetails: bool = ...,
     ) -> DescribeClustersResponseTypeDef:
         """
         Returns information about all provisioned clusters if no cluster identifier is
         specified, or about a specific cluster if a cluster name is
         supplied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_clusters)
@@ -406,15 +405,15 @@
     async def describe_engine_versions(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        DefaultOnly: bool = ...
+        DefaultOnly: bool = ...,
     ) -> DescribeEngineVersionsResponseTypeDef:
         """
         Returns a list of the available Redis engine versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_engine_versions)
         """
@@ -424,15 +423,15 @@
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to clusters, security groups, and parameter groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_events)
         """
@@ -462,15 +461,15 @@
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedNodesResponseTypeDef:
         """
         Returns information about reserved nodes for this account, or about a specified
         reserved
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes)
@@ -481,15 +480,15 @@
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedNodesOfferingsResponseTypeDef:
         """
         Lists available reserved node offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_reserved_nodes_offerings)
         """
@@ -497,15 +496,15 @@
     async def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeServiceUpdatesResponseTypeDef:
         """
         Returns details of the service updates See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/memorydb-2021-01-01/DescribeServiceUpdates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_service_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_service_updates)
@@ -515,15 +514,15 @@
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ShowDetail: bool = ...
+        ShowDetail: bool = ...,
     ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns information about cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_snapshots)
         """
@@ -540,15 +539,15 @@
 
     async def describe_users(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUsersResponseTypeDef:
         """
         Returns a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_users)
         """
@@ -599,29 +598,29 @@
 
     async def purchase_reserved_nodes_offering(
         self,
         *,
         ReservedNodesOfferingId: str,
         ReservationId: str = ...,
         NodeCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedNodesOfferingResponseTypeDef:
         """
         Allows you to purchase a reserved node offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.purchase_reserved_nodes_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#purchase_reserved_nodes_offering)
         """
 
     async def reset_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         AllParameters: bool = ...,
-        ParameterNames: Sequence[str] = ...
+        ParameterNames: Sequence[str] = ...,
     ) -> ResetParameterGroupResponseTypeDef:
         """
         Modifies the parameters of a parameter group to the engine or system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.reset_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#reset_parameter_group)
@@ -649,15 +648,15 @@
         """
 
     async def update_acl(
         self,
         *,
         ACLName: str,
         UserNamesToAdd: Sequence[str] = ...,
-        UserNamesToRemove: Sequence[str] = ...
+        UserNamesToRemove: Sequence[str] = ...,
     ) -> UpdateACLResponseTypeDef:
         """
         Changes the list of users that belong to the Access Control List.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_acl)
         """
@@ -674,15 +673,15 @@
         ParameterGroupName: str = ...,
         SnapshotWindow: str = ...,
         SnapshotRetentionLimit: int = ...,
         NodeType: str = ...,
         EngineVersion: str = ...,
         ReplicaConfiguration: ReplicaConfigurationRequestTypeDef = ...,
         ShardConfiguration: ShardConfigurationRequestTypeDef = ...,
-        ACLName: str = ...
+        ACLName: str = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_cluster)
         """
@@ -708,15 +707,15 @@
         """
 
     async def update_user(
         self,
         *,
         UserName: str,
         AuthenticationMode: AuthenticationModeTypeDef = ...,
-        AccessString: str = ...
+        AccessString: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_user)
         """
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/client.pyi` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -201,15 +201,15 @@
     async def copy_snapshot(
         self,
         *,
         SourceSnapshotName: str,
         TargetSnapshotName: str,
         TargetBucket: str = ...,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CopySnapshotResponseTypeDef:
         """
         Makes a copy of an existing snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#copy_snapshot)
         """
@@ -244,75 +244,75 @@
         SnapshotArns: Sequence[str] = ...,
         SnapshotName: str = ...,
         SnapshotRetentionLimit: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SnapshotWindow: str = ...,
         EngineVersion: str = ...,
         AutoMinorVersionUpgrade: bool = ...,
-        DataTiering: bool = ...
+        DataTiering: bool = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_cluster)
         """
 
     async def create_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         Family: str,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateParameterGroupResponseTypeDef:
         """
         Creates a new MemoryDB parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_parameter_group)
         """
 
     async def create_snapshot(
         self,
         *,
         ClusterName: str,
         SnapshotName: str,
         KmsKeyId: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSnapshotResponseTypeDef:
         """
         Creates a copy of an entire cluster at a specific moment in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_snapshot)
         """
 
     async def create_subnet_group(
         self,
         *,
         SubnetGroupName: str,
         SubnetIds: Sequence[str],
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSubnetGroupResponseTypeDef:
         """
         Creates a subnet group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_subnet_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_subnet_group)
         """
 
     async def create_user(
         self,
         *,
         UserName: str,
         AuthenticationMode: AuthenticationModeTypeDef,
         AccessString: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateUserResponseTypeDef:
         """
         Creates a MemoryDB user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#create_user)
         """
@@ -384,15 +384,15 @@
 
     async def describe_clusters(
         self,
         *,
         ClusterName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ShowShardDetails: bool = ...
+        ShowShardDetails: bool = ...,
     ) -> DescribeClustersResponseTypeDef:
         """
         Returns information about all provisioned clusters if no cluster identifier is
         specified, or about a specific cluster if a cluster name is
         supplied.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_clusters)
@@ -402,15 +402,15 @@
     async def describe_engine_versions(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        DefaultOnly: bool = ...
+        DefaultOnly: bool = ...,
     ) -> DescribeEngineVersionsResponseTypeDef:
         """
         Returns a list of the available Redis engine versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_engine_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_engine_versions)
         """
@@ -420,15 +420,15 @@
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeEventsResponseTypeDef:
         """
         Returns events related to clusters, security groups, and parameter groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_events)
         """
@@ -458,15 +458,15 @@
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedNodesResponseTypeDef:
         """
         Returns information about reserved nodes for this account, or about a specified
         reserved
         node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes)
@@ -477,15 +477,15 @@
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeReservedNodesOfferingsResponseTypeDef:
         """
         Lists available reserved node offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_reserved_nodes_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_reserved_nodes_offerings)
         """
@@ -493,15 +493,15 @@
     async def describe_service_updates(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeServiceUpdatesResponseTypeDef:
         """
         Returns details of the service updates See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/memorydb-2021-01-01/DescribeServiceUpdates).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_service_updates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_service_updates)
@@ -511,15 +511,15 @@
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ShowDetail: bool = ...
+        ShowDetail: bool = ...,
     ) -> DescribeSnapshotsResponseTypeDef:
         """
         Returns information about cluster snapshots.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_snapshots)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_snapshots)
         """
@@ -536,15 +536,15 @@
 
     async def describe_users(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeUsersResponseTypeDef:
         """
         Returns a list of users.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.describe_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#describe_users)
         """
@@ -595,29 +595,29 @@
 
     async def purchase_reserved_nodes_offering(
         self,
         *,
         ReservedNodesOfferingId: str,
         ReservationId: str = ...,
         NodeCount: int = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> PurchaseReservedNodesOfferingResponseTypeDef:
         """
         Allows you to purchase a reserved node offering.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.purchase_reserved_nodes_offering)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#purchase_reserved_nodes_offering)
         """
 
     async def reset_parameter_group(
         self,
         *,
         ParameterGroupName: str,
         AllParameters: bool = ...,
-        ParameterNames: Sequence[str] = ...
+        ParameterNames: Sequence[str] = ...,
     ) -> ResetParameterGroupResponseTypeDef:
         """
         Modifies the parameters of a parameter group to the engine or system default
         value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.reset_parameter_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#reset_parameter_group)
@@ -645,15 +645,15 @@
         """
 
     async def update_acl(
         self,
         *,
         ACLName: str,
         UserNamesToAdd: Sequence[str] = ...,
-        UserNamesToRemove: Sequence[str] = ...
+        UserNamesToRemove: Sequence[str] = ...,
     ) -> UpdateACLResponseTypeDef:
         """
         Changes the list of users that belong to the Access Control List.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_acl)
         """
@@ -670,15 +670,15 @@
         ParameterGroupName: str = ...,
         SnapshotWindow: str = ...,
         SnapshotRetentionLimit: int = ...,
         NodeType: str = ...,
         EngineVersion: str = ...,
         ReplicaConfiguration: ReplicaConfigurationRequestTypeDef = ...,
         ShardConfiguration: ShardConfigurationRequestTypeDef = ...,
-        ACLName: str = ...
+        ACLName: str = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Modifies the settings for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_cluster)
         """
@@ -704,15 +704,15 @@
         """
 
     async def update_user(
         self,
         *,
         UserName: str,
         AuthenticationMode: AuthenticationModeTypeDef = ...,
-        AccessString: str = ...
+        AccessString: str = ...,
     ) -> UpdateUserResponseTypeDef:
         """
         Changes user password(s) and/or access string.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/client/#update_user)
         """
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/literals.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/literals.py`

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
     "AZStatusType",
     "AuthenticationTypeType",
     "DataTieringStatusType",
     "DescribeACLsPaginatorName",
     "DescribeClustersPaginatorName",
     "DescribeEngineVersionsPaginatorName",
@@ -43,15 +42,14 @@
     "MemoryDBServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AZStatusType = Literal["multiaz", "singleaz"]
 AuthenticationTypeType = Literal["iam", "no-password", "password"]
 DataTieringStatusType = Literal["false", "true"]
 DescribeACLsPaginatorName = Literal["describe_acls"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
 DescribeEngineVersionsPaginatorName = Literal["describe_engine_versions"]
 DescribeEventsPaginatorName = Literal["describe_events"]
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/literals.pyi` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/paginator.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
     "DescribeReservedNodesOfferingsPaginator",
     "DescribeServiceUpdatesPaginator",
     "DescribeSnapshotsPaginator",
     "DescribeSubnetGroupsPaginator",
     "DescribeUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -115,15 +114,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         ShowShardDetails: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeclusterspaginator)
         """
 
 
@@ -135,15 +134,15 @@
 
     def paginate(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeengineversionspaginator)
         """
 
 
@@ -157,15 +156,15 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeeventspaginator)
         """
 
 
@@ -209,15 +208,15 @@
         self,
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describereservednodespaginator)
         """
 
 
@@ -230,15 +229,15 @@
     def paginate(
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodesOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describereservednodesofferingspaginator)
         """
 
 
@@ -250,15 +249,15 @@
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServiceUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeserviceupdatespaginator)
         """
 
 
@@ -271,15 +270,15 @@
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         ShowDetail: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describesnapshotspaginator)
         """
 
 
@@ -305,13 +304,13 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/paginator.pyi` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         ShowShardDetails: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeclusterspaginator)
         """
 
 class DescribeEngineVersionsPaginator(AioPaginator):
@@ -130,15 +130,15 @@
 
     def paginate(
         self,
         *,
         EngineVersion: str = ...,
         ParameterGroupFamily: str = ...,
         DefaultOnly: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEngineVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEngineVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeengineversionspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
@@ -151,15 +151,15 @@
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Duration: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeeventspaginator)
         """
 
 class DescribeParameterGroupsPaginator(AioPaginator):
@@ -200,15 +200,15 @@
         self,
         *,
         ReservationId: str = ...,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describereservednodespaginator)
         """
 
 class DescribeReservedNodesOfferingsPaginator(AioPaginator):
@@ -220,15 +220,15 @@
     def paginate(
         self,
         *,
         ReservedNodesOfferingId: str = ...,
         NodeType: str = ...,
         Duration: str = ...,
         OfferingType: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeReservedNodesOfferingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeReservedNodesOfferings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describereservednodesofferingspaginator)
         """
 
 class DescribeServiceUpdatesPaginator(AioPaginator):
@@ -239,15 +239,15 @@
 
     def paginate(
         self,
         *,
         ServiceUpdateName: str = ...,
         ClusterNames: Sequence[str] = ...,
         Status: Sequence[ServiceUpdateStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServiceUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeServiceUpdates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeserviceupdatespaginator)
         """
 
 class DescribeSnapshotsPaginator(AioPaginator):
@@ -259,15 +259,15 @@
     def paginate(
         self,
         *,
         ClusterName: str = ...,
         SnapshotName: str = ...,
         Source: str = ...,
         ShowDetail: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSnapshotsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeSnapshots.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describesnapshotspaginator)
         """
 
 class DescribeSubnetGroupsPaginator(AioPaginator):
@@ -291,13 +291,13 @@
     """
 
     def paginate(
         self,
         *,
         UserName: str = ...,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB.Paginator.DescribeUsers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/paginators/#describeuserspaginator)
         """
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/type_defs.py` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ACLPendingChangesTypeDef",
     "ACLsUpdateStatusTypeDef",
     "AuthenticationModeTypeDef",
     "AuthenticationTypeDef",
     "AvailabilityZoneTypeDef",
     "ServiceUpdateRequestTypeDef",
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb/type_defs.pyi` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/PKG-INFO` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-memorydb
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MemoryDB 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MemoryDB 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/
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
 
 <a id="types-aiobotocore-memorydb"></a>
 
 # types-aiobotocore-memorydb
 
 [![PyPI - types-aiobotocore-memorydb](https://img.shields.io/pypi/v/types-aiobotocore-memorydb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-memorydb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-memorydb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-memorydb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-memorydb)](https://pepy.tech/project/types-aiobotocore-memorydb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MemoryDB 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
+[aiobotocore.MemoryDB 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#MemoryDB)
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
 [types-aiobotocore-memorydb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_memorydb/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-memorydb-2.9.0/types_aiobotocore_memorydb.egg-info/SOURCES.txt` & `types-aiobotocore-memorydb-2.9.1/types_aiobotocore_memorydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

