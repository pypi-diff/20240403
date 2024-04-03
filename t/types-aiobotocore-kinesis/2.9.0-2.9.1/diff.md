# Comparing `tmp/types-aiobotocore-kinesis-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesis-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-2.9.0.tar", last modified: Wed Dec 13 19:59:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-2.9.1.tar", last modified: Thu Jan 18 01:21:02 2024, max compression
```

## Comparing `types-aiobotocore-kinesis-2.9.0.tar` & `types-aiobotocore-kinesis-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.253578 types-aiobotocore-kinesis-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2023-12-13 19:59:39.253578 types-aiobotocore-kinesis-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12591 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:39.253578 types-aiobotocore-kinesis-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:48:31.000000 types-aiobotocore-kinesis-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.249578 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28191 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28187 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10399 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25303 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25302 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-12-13 19:48:32.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:39.253578 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14154 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:59:39.000000 types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.169244 types-aiobotocore-kinesis-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-01-18 01:21:02.169244 types-aiobotocore-kinesis-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:02.169244 types-aiobotocore-kinesis-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.165244 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28205 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28202 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10399 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25302 2024-01-18 01:10:21.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:18.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-01-18 01:10:19.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:02.169244 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:02.000000 types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-2.9.0/LICENSE` & `types-aiobotocore-kinesis-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesis-2.9.0/PKG-INFO` & `types-aiobotocore-kinesis-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Kinesis 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Kinesis 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/
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
 
 <a id="types-aiobotocore-kinesis"></a>
 
 # types-aiobotocore-kinesis
 
 [![PyPI - types-aiobotocore-kinesis](https://img.shields.io/pypi/v/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis)](https://pepy.tech/project/types-aiobotocore-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kinesis 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[aiobotocore.Kinesis 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [types-aiobotocore-kinesis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-2.9.0/README.md` & `types-aiobotocore-kinesis-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis)](https://pepy.tech/project/types-aiobotocore-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kinesis 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[aiobotocore.Kinesis 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [types-aiobotocore-kinesis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-2.9.0/setup.py` & `types-aiobotocore-kinesis-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Kinesis 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Kinesis 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore kinesis type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesis": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__init__.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     ListStreamConsumersPaginator,
     ListStreamsPaginator,
 )
 from .waiter import StreamExistsWaiter, StreamNotExistsWaiter
 
 Client = KinesisClient
 
-
 __all__ = (
     "Client",
     "DescribeStreamPaginator",
     "KinesisClient",
     "ListShardsPaginator",
     "ListStreamConsumersPaginator",
     "ListStreamsPaginator",
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__init__.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/__main__.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Kinesis 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Kinesis 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis\nOther"
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

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/client.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 from .waiter import StreamExistsWaiter, StreamNotExistsWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KinesisClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -137,15 +136,15 @@
         """
 
     async def create_stream(
         self,
         *,
         StreamName: str,
         ShardCount: int = ...,
-        StreamModeDetails: StreamModeDetailsTypeDef = ...
+        StreamModeDetails: StreamModeDetailsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#create_stream)
         """
@@ -200,15 +199,15 @@
 
     async def describe_stream(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> DescribeStreamOutputTypeDef:
         """
         Describes the specified Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.describe_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#describe_stream)
         """
@@ -237,29 +236,29 @@
         """
 
     async def disable_enhanced_monitoring(
         self,
         *,
         ShardLevelMetrics: Sequence[MetricsNameType],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EnhancedMonitoringOutputTypeDef:
         """
         Disables enhanced monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.disable_enhanced_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#disable_enhanced_monitoring)
         """
 
     async def enable_enhanced_monitoring(
         self,
         *,
         ShardLevelMetrics: Sequence[MetricsNameType],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EnhancedMonitoringOutputTypeDef:
         """
         Enables enhanced Kinesis data stream monitoring for shard-level metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.enable_enhanced_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#enable_enhanced_monitoring)
         """
@@ -300,15 +299,15 @@
         self,
         *,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
         StreamName: str = ...,
         StartingSequenceNumber: str = ...,
         Timestamp: TimestampTypeDef = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> GetShardIteratorOutputTypeDef:
         """
         Gets an Amazon Kinesis shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.get_shard_iterator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#get_shard_iterator)
         """
@@ -330,30 +329,30 @@
         *,
         StreamName: str = ...,
         NextToken: str = ...,
         ExclusiveStartShardId: str = ...,
         MaxResults: int = ...,
         StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> ListShardsOutputTypeDef:
         """
         Lists the shards in a stream and provides information about each shard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_shards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#list_shards)
         """
 
     async def list_stream_consumers(
         self,
         *,
         StreamARN: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: TimestampTypeDef = ...
+        StreamCreationTimestamp: TimestampTypeDef = ...,
     ) -> ListStreamConsumersOutputTypeDef:
         """
         Lists the consumers registered to receive data from a stream using enhanced
         fan-out, and provides information about each
         consumer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_stream_consumers)
@@ -372,30 +371,30 @@
 
     async def list_tags_for_stream(
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartTagKey: str = ...,
         Limit: int = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> ListTagsForStreamOutputTypeDef:
         """
         Lists the tags for the specified Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_tags_for_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#list_tags_for_stream)
         """
 
     async def merge_shards(
         self,
         *,
         ShardToMerge: str,
         AdjacentShardToMerge: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Merges two adjacent shards in a Kinesis data stream and combines them into a
         single shard to reduce the stream's capacity to ingest and transport
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.merge_shards)
@@ -406,29 +405,29 @@
         self,
         *,
         Data: BlobTypeDef,
         PartitionKey: str,
         StreamName: str = ...,
         ExplicitHashKey: str = ...,
         SequenceNumberForOrdering: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> PutRecordOutputTypeDef:
         """
         Writes a single data record into an Amazon Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.put_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#put_record)
         """
 
     async def put_records(
         self,
         *,
         Records: Sequence[PutRecordsRequestEntryTypeDef],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> PutRecordsOutputTypeDef:
         """
         Writes multiple data records into a Kinesis data stream in a single call (also
         referred to as a `PutRecords`
         request).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.put_records)
@@ -467,15 +466,15 @@
 
     async def split_shard(
         self,
         *,
         ShardToSplit: str,
         NewStartingHashKey: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Splits a shard into two new shards in the Kinesis data stream, to increase the
         stream's capacity to ingest and transport
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.split_shard)
@@ -484,15 +483,15 @@
 
     async def start_stream_encryption(
         self,
         *,
         EncryptionType: EncryptionTypeType,
         KeyId: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables or updates server-side encryption using an Amazon Web Services KMS key
         for a specified
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.start_stream_encryption)
@@ -501,15 +500,15 @@
 
     async def stop_stream_encryption(
         self,
         *,
         EncryptionType: EncryptionTypeType,
         KeyId: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables server-side encryption for a specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.stop_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#stop_stream_encryption)
         """
@@ -529,15 +528,15 @@
 
     async def update_shard_count(
         self,
         *,
         TargetShardCount: int,
         ScalingType: Literal["UNIFORM_SCALING"],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> UpdateShardCountOutputTypeDef:
         """
         Updates the shard count of the specified stream to the specified number of
         shards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.update_shard_count)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#update_shard_count)
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/client.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         """
 
     async def create_stream(
         self,
         *,
         StreamName: str,
         ShardCount: int = ...,
-        StreamModeDetails: StreamModeDetailsTypeDef = ...
+        StreamModeDetails: StreamModeDetailsTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.create_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#create_stream)
         """
@@ -196,15 +196,15 @@
 
     async def describe_stream(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> DescribeStreamOutputTypeDef:
         """
         Describes the specified Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.describe_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#describe_stream)
         """
@@ -233,29 +233,29 @@
         """
 
     async def disable_enhanced_monitoring(
         self,
         *,
         ShardLevelMetrics: Sequence[MetricsNameType],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EnhancedMonitoringOutputTypeDef:
         """
         Disables enhanced monitoring.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.disable_enhanced_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#disable_enhanced_monitoring)
         """
 
     async def enable_enhanced_monitoring(
         self,
         *,
         ShardLevelMetrics: Sequence[MetricsNameType],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EnhancedMonitoringOutputTypeDef:
         """
         Enables enhanced Kinesis data stream monitoring for shard-level metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.enable_enhanced_monitoring)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#enable_enhanced_monitoring)
         """
@@ -296,15 +296,15 @@
         self,
         *,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
         StreamName: str = ...,
         StartingSequenceNumber: str = ...,
         Timestamp: TimestampTypeDef = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> GetShardIteratorOutputTypeDef:
         """
         Gets an Amazon Kinesis shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.get_shard_iterator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#get_shard_iterator)
         """
@@ -326,30 +326,30 @@
         *,
         StreamName: str = ...,
         NextToken: str = ...,
         ExclusiveStartShardId: str = ...,
         MaxResults: int = ...,
         StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> ListShardsOutputTypeDef:
         """
         Lists the shards in a stream and provides information about each shard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_shards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#list_shards)
         """
 
     async def list_stream_consumers(
         self,
         *,
         StreamARN: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        StreamCreationTimestamp: TimestampTypeDef = ...
+        StreamCreationTimestamp: TimestampTypeDef = ...,
     ) -> ListStreamConsumersOutputTypeDef:
         """
         Lists the consumers registered to receive data from a stream using enhanced
         fan-out, and provides information about each
         consumer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_stream_consumers)
@@ -368,30 +368,30 @@
 
     async def list_tags_for_stream(
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartTagKey: str = ...,
         Limit: int = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> ListTagsForStreamOutputTypeDef:
         """
         Lists the tags for the specified Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.list_tags_for_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#list_tags_for_stream)
         """
 
     async def merge_shards(
         self,
         *,
         ShardToMerge: str,
         AdjacentShardToMerge: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Merges two adjacent shards in a Kinesis data stream and combines them into a
         single shard to reduce the stream's capacity to ingest and transport
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.merge_shards)
@@ -402,29 +402,29 @@
         self,
         *,
         Data: BlobTypeDef,
         PartitionKey: str,
         StreamName: str = ...,
         ExplicitHashKey: str = ...,
         SequenceNumberForOrdering: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> PutRecordOutputTypeDef:
         """
         Writes a single data record into an Amazon Kinesis data stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.put_record)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#put_record)
         """
 
     async def put_records(
         self,
         *,
         Records: Sequence[PutRecordsRequestEntryTypeDef],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> PutRecordsOutputTypeDef:
         """
         Writes multiple data records into a Kinesis data stream in a single call (also
         referred to as a `PutRecords`
         request).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.put_records)
@@ -463,15 +463,15 @@
 
     async def split_shard(
         self,
         *,
         ShardToSplit: str,
         NewStartingHashKey: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Splits a shard into two new shards in the Kinesis data stream, to increase the
         stream's capacity to ingest and transport
         data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.split_shard)
@@ -480,15 +480,15 @@
 
     async def start_stream_encryption(
         self,
         *,
         EncryptionType: EncryptionTypeType,
         KeyId: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Enables or updates server-side encryption using an Amazon Web Services KMS key
         for a specified
         stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.start_stream_encryption)
@@ -497,15 +497,15 @@
 
     async def stop_stream_encryption(
         self,
         *,
         EncryptionType: EncryptionTypeType,
         KeyId: str,
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Disables server-side encryption for a specified stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.stop_stream_encryption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#stop_stream_encryption)
         """
@@ -525,15 +525,15 @@
 
     async def update_shard_count(
         self,
         *,
         TargetShardCount: int,
         ScalingType: Literal["UNIFORM_SCALING"],
         StreamName: str = ...,
-        StreamARN: str = ...
+        StreamARN: str = ...,
     ) -> UpdateShardCountOutputTypeDef:
         """
         Updates the shard count of the specified stream to the specified number of
         shards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Client.update_shard_count)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/client/#update_shard_count)
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/literals.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/literals.py`

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
     "ConsumerStatusType",
     "DescribeStreamPaginatorName",
     "EncryptionTypeType",
     "ListShardsPaginatorName",
     "ListStreamConsumersPaginatorName",
     "ListStreamsPaginatorName",
@@ -39,15 +38,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ConsumerStatusType = Literal["ACTIVE", "CREATING", "DELETING"]
 DescribeStreamPaginatorName = Literal["describe_stream"]
 EncryptionTypeType = Literal["KMS", "NONE"]
 ListShardsPaginatorName = Literal["list_shards"]
 ListStreamConsumersPaginatorName = Literal["list_stream_consumers"]
 ListStreamsPaginatorName = Literal["list_streams"]
 MetricsNameType = Literal[
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/literals.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/paginator.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "DescribeStreamPaginator",
     "ListShardsPaginator",
     "ListStreamConsumersPaginator",
     "ListStreamsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -67,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#describestreampaginator)
         """
 
 
@@ -89,15 +88,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#listshardspaginator)
         """
 
 
@@ -108,15 +107,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#liststreamconsumerspaginator)
         """
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/paginator.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeStreamOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.DescribeStream.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#describestreampaginator)
         """
 
 class ListShardsPaginator(AioPaginator):
@@ -85,15 +85,15 @@
         self,
         *,
         StreamName: str = ...,
         ExclusiveStartShardId: str = ...,
         StreamCreationTimestamp: TimestampTypeDef = ...,
         ShardFilter: ShardFilterTypeDef = ...,
         StreamARN: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListShardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListShards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#listshardspaginator)
         """
 
 class ListStreamConsumersPaginator(AioPaginator):
@@ -103,15 +103,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamARN: str,
         StreamCreationTimestamp: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStreamConsumersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Paginator.ListStreamConsumers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/paginators/#liststreamconsumerspaginator)
         """
 
 class ListStreamsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/type_defs.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/type_defs.py`

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
     "AddTagsToStreamInputRequestTypeDef",
     "BlobTypeDef",
     "HashKeyRangeTypeDef",
     "ConsumerDescriptionTypeDef",
     "ConsumerTypeDef",
     "StreamModeDetailsTypeDef",
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/type_defs.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/waiter.py` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/waiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     async def wait(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
         StreamARN: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/waiters/#streamexistswaiter)
         """
 
 
@@ -60,13 +60,13 @@
     async def wait(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
         StreamARN: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/waiters/#streamnotexistswaiter)
         """
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis/waiter.pyi` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis/waiter.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     async def wait(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
         StreamARN: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/waiters/#streamexistswaiter)
         """
 
 class StreamNotExistsWaiter(AIOWaiter):
@@ -58,13 +58,13 @@
     async def wait(
         self,
         *,
         StreamName: str = ...,
         Limit: int = ...,
         ExclusiveStartShardId: str = ...,
         StreamARN: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis.Waiter.StreamNotExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/waiters/#streamnotexistswaiter)
         """
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Kinesis 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Kinesis 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/
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
 
 <a id="types-aiobotocore-kinesis"></a>
 
 # types-aiobotocore-kinesis
 
 [![PyPI - types-aiobotocore-kinesis](https://img.shields.io/pypi/v/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis)](https://pepy.tech/project/types-aiobotocore-kinesis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Kinesis 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
+[aiobotocore.Kinesis 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#Kinesis)
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
 [types-aiobotocore-kinesis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesis-2.9.0/types_aiobotocore_kinesis.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-2.9.1/types_aiobotocore_kinesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

