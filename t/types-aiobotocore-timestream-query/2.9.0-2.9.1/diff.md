# Comparing `tmp/types-aiobotocore-timestream-query-2.9.0.tar.gz` & `tmp/types-aiobotocore-timestream-query-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-query-2.9.0.tar", last modified: Wed Dec 13 20:00:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-query-2.9.1.tar", last modified: Thu Jan 18 01:21:58 2024, max compression
```

## Comparing `types-aiobotocore-timestream-query-2.9.0.tar` & `types-aiobotocore-timestream-query-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.745050 types-aiobotocore-timestream-query-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-12-13 20:00:40.745050 types-aiobotocore-timestream-query-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12193 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:40.745050 types-aiobotocore-timestream-query-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.745050 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14526 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9451 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9449 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15916 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15915 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:20.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.745050 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-12-13 20:00:40.000000 types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.180992 types-aiobotocore-timestream-query-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-01-18 01:21:58.180992 types-aiobotocore-timestream-query-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12193 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:58.180992 types-aiobotocore-timestream-query-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.180992 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14526 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14523 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9449 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-01-18 01:18:49.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:48.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:58.180992 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-18 01:21:58.000000 types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/LICENSE` & `types-aiobotocore-timestream-query-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-timestream-query-2.9.0/PKG-INFO` & `types-aiobotocore-timestream-query-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
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
 
 <a id="types-aiobotocore-timestream-query"></a>
 
 # types-aiobotocore-timestream-query
 
 [![PyPI - types-aiobotocore-timestream-query](https://img.shields.io/pypi/v/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/README.md` & `types-aiobotocore-timestream-query-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/setup.py` & `types-aiobotocore-timestream-query-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-query",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TimestreamQuery 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.TimestreamQuery 2.9.1 service generated with"
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
     keywords="aiobotocore timestream-query type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_timestream_query": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__init__.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import TimestreamQueryClient
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 
 Client = TimestreamQueryClient
 
-
 __all__ = (
     "Client",
     "ListScheduledQueriesPaginator",
     "ListTagsForResourcePaginator",
     "QueryPaginator",
     "TimestreamQueryClient",
 )
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__init__.pyi` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/__main__.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TimestreamQuery 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.TimestreamQuery 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/client.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TimestreamQueryClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -120,15 +119,15 @@
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
         TargetConfiguration: TargetConfigurationTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.create_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#create_scheduled_query)
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/client.pyi` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
         TargetConfiguration: TargetConfigurationTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.create_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#create_scheduled_query)
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/literals.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/literals.py`

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
     "DimensionValueTypeType",
     "ListScheduledQueriesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "MeasureValueTypeType",
     "QueryPaginatorName",
     "S3EncryptionOptionType",
@@ -33,15 +32,14 @@
     "ScheduledQueryStateType",
     "TimestreamQueryServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DimensionValueTypeType = Literal["VARCHAR"]
 ListScheduledQueriesPaginatorName = Literal["list_scheduled_queries"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "VARCHAR"]
 QueryPaginatorName = Literal["query"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/literals.pyi` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/paginator.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QueryResponseTypeDef,
 )
 
 __all__ = ("ListScheduledQueriesPaginator", "ListTagsForResourcePaginator", "QueryPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -87,13 +86,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/paginator.pyi` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,13 +82,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/type_defs.py` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/type_defs.py`

 * *Files 0% similar despite different names*

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
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
     "RowTypeDef",
@@ -434,15 +433,15 @@
 )
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
-        "ColumnInfo": List[ColumnInfoTypeDef],
+        "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query/type_defs.pyi` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
 )
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
-        "ColumnInfo": List[ColumnInfoTypeDef],
+        "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/PKG-INFO` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
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
 
 <a id="types-aiobotocore-timestream-query"></a>
 
 # types-aiobotocore-timestream-query
 
 [![PyPI - types-aiobotocore-timestream-query](https://img.shields.io/pypi/v/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TimestreamQuery 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[aiobotocore.TimestreamQuery 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-timestream-query-2.9.0/types_aiobotocore_timestream_query.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-query-2.9.1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

