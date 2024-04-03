# Comparing `tmp/types-aiobotocore-dax-2.9.0.tar.gz` & `tmp/types-aiobotocore-dax-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dax-2.9.0.tar", last modified: Wed Dec 13 19:59:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-dax-2.9.1.tar", last modified: Thu Jan 18 01:20:30 2024, max compression
```

## Comparing `types-aiobotocore-dax-2.9.0.tar` & `types-aiobotocore-dax-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.961847 types-aiobotocore-dax-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2023-12-13 19:59:04.961847 types-aiobotocore-dax-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12082 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:04.961847 types-aiobotocore-dax-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.961847 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21990 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21986 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9835 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8999 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8990 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19913 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19912 2023-12-13 19:43:58.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:57.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:04.961847 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:04.000000 types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.477394 types-aiobotocore-dax-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-01-18 01:20:30.477394 types-aiobotocore-dax-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12082 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:30.477394 types-aiobotocore-dax-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.477394 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21995 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21992 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9835 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19912 2024-01-18 01:05:53.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19912 2024-01-18 01:05:53.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:52.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.477394 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13649 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:30.000000 types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dax-2.9.0/LICENSE` & `types-aiobotocore-dax-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-dax-2.9.0/PKG-INFO` & `types-aiobotocore-dax-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dax
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DAX 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DAX 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
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
 
 <a id="types-aiobotocore-dax"></a>
 
 # types-aiobotocore-dax
 
 [![PyPI - types-aiobotocore-dax](https://img.shields.io/pypi/v/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dax)](https://pepy.tech/project/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dax-2.9.0/README.md` & `types-aiobotocore-dax-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dax)](https://pepy.tech/project/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dax-2.9.0/setup.py` & `types-aiobotocore-dax-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dax",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DAX 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.DAX 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore dax type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dax": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__init__.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     DescribeParametersPaginator,
     DescribeSubnetGroupsPaginator,
     ListTagsPaginator,
 )
 
 Client = DAXClient
 
-
 __all__ = (
     "Client",
     "DAXClient",
     "DescribeClustersPaginator",
     "DescribeDefaultParametersPaginator",
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__init__.pyi` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/__main__.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DAX 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DAX 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/client.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DAXClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -152,15 +151,15 @@
         SubnetGroupName: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreferredMaintenanceWindow: str = ...,
         NotificationTopicArn: str = ...,
         ParameterGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
-        ClusterEndpointEncryptionType: ClusterEndpointEncryptionTypeType = ...
+        ClusterEndpointEncryptionType: ClusterEndpointEncryptionTypeType = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#create_cluster)
         """
@@ -187,15 +186,15 @@
 
     async def decrease_replication_factor(
         self,
         *,
         ClusterName: str,
         NewReplicationFactor: int,
         AvailabilityZones: Sequence[str] = ...,
-        NodeIdsToRemove: Sequence[str] = ...
+        NodeIdsToRemove: Sequence[str] = ...,
     ) -> DecreaseReplicationFactorResponseTypeDef:
         """
         Removes one or more nodes from a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.decrease_replication_factor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#decrease_replication_factor)
         """
@@ -255,44 +254,44 @@
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
         Returns events related to DAX clusters and parameter groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_events)
         """
 
     async def describe_parameter_groups(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParameterGroupsResponseTypeDef:
         """
         Returns a list of parameter group descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_parameter_groups)
         """
 
     async def describe_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParametersResponseTypeDef:
         """
         Returns the detailed parameter list for a particular parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_parameters)
         """
@@ -374,15 +373,15 @@
         *,
         ClusterName: str,
         Description: str = ...,
         PreferredMaintenanceWindow: str = ...,
         NotificationTopicArn: str = ...,
         NotificationTopicStatus: str = ...,
         ParameterGroupName: str = ...,
-        SecurityGroupIds: Sequence[str] = ...
+        SecurityGroupIds: Sequence[str] = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Modifies the settings for a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#update_cluster)
         """
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/client.pyi` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         SubnetGroupName: str = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreferredMaintenanceWindow: str = ...,
         NotificationTopicArn: str = ...,
         ParameterGroupName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SSESpecification: SSESpecificationTypeDef = ...,
-        ClusterEndpointEncryptionType: ClusterEndpointEncryptionTypeType = ...
+        ClusterEndpointEncryptionType: ClusterEndpointEncryptionTypeType = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#create_cluster)
         """
@@ -183,15 +183,15 @@
 
     async def decrease_replication_factor(
         self,
         *,
         ClusterName: str,
         NewReplicationFactor: int,
         AvailabilityZones: Sequence[str] = ...,
-        NodeIdsToRemove: Sequence[str] = ...
+        NodeIdsToRemove: Sequence[str] = ...,
     ) -> DecreaseReplicationFactorResponseTypeDef:
         """
         Removes one or more nodes from a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.decrease_replication_factor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#decrease_replication_factor)
         """
@@ -251,44 +251,44 @@
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
         Returns events related to DAX clusters and parameter groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_events)
         """
 
     async def describe_parameter_groups(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParameterGroupsResponseTypeDef:
         """
         Returns a list of parameter group descriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_parameter_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_parameter_groups)
         """
 
     async def describe_parameters(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeParametersResponseTypeDef:
         """
         Returns the detailed parameter list for a particular parameter group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.describe_parameters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#describe_parameters)
         """
@@ -370,15 +370,15 @@
         *,
         ClusterName: str,
         Description: str = ...,
         PreferredMaintenanceWindow: str = ...,
         NotificationTopicArn: str = ...,
         NotificationTopicStatus: str = ...,
         ParameterGroupName: str = ...,
-        SecurityGroupIds: Sequence[str] = ...
+        SecurityGroupIds: Sequence[str] = ...,
     ) -> UpdateClusterResponseTypeDef:
         """
         Modifies the settings for a DAX cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/client/#update_cluster)
         """
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/literals.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/literals.py`

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
     "ChangeTypeType",
     "ClusterEndpointEncryptionTypeType",
     "DescribeClustersPaginatorName",
     "DescribeDefaultParametersPaginatorName",
     "DescribeEventsPaginatorName",
     "DescribeParameterGroupsPaginatorName",
@@ -37,15 +36,14 @@
     "DAXServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ChangeTypeType = Literal["IMMEDIATE", "REQUIRES_REBOOT"]
 ClusterEndpointEncryptionTypeType = Literal["NONE", "TLS"]
 DescribeClustersPaginatorName = Literal["describe_clusters"]
 DescribeDefaultParametersPaginatorName = Literal["describe_default_parameters"]
 DescribeEventsPaginatorName = Literal["describe_events"]
 DescribeParameterGroupsPaginatorName = Literal["describe_parameter_groups"]
 DescribeParametersPaginatorName = Literal["describe_parameters"]
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/literals.pyi` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/paginator.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
     "DescribeParametersPaginator",
     "DescribeSubnetGroupsPaginator",
     "ListTagsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -112,15 +111,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeeventspaginator)
         """
 
 
@@ -130,15 +129,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparametergroupspaginator)
         """
 
 
@@ -149,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparameterspaginator)
         """
 
 
@@ -167,15 +166,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describesubnetgroupspaginator)
         """
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/paginator.pyi` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
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
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeeventspaginator)
         """
 
 class DescribeParameterGroupsPaginator(AioPaginator):
@@ -124,15 +124,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparametergroupspaginator)
         """
 
 class DescribeParametersPaginator(AioPaginator):
@@ -142,15 +142,15 @@
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describeparameterspaginator)
         """
 
 class DescribeSubnetGroupsPaginator(AioPaginator):
@@ -159,15 +159,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/paginators/#describesubnetgroupspaginator)
         """
 
 class ListTagsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/type_defs.py` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax/type_defs.pyi` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/PKG-INFO` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dax
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DAX 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DAX 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/
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
 
 <a id="types-aiobotocore-dax"></a>
 
 # types-aiobotocore-dax
 
 [![PyPI - types-aiobotocore-dax](https://img.shields.io/pypi/v/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dax.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dax)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dax)](https://pepy.tech/project/types-aiobotocore-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DAX 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[aiobotocore.DAX 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [types-aiobotocore-dax docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dax/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dax-2.9.0/types_aiobotocore_dax.egg-info/SOURCES.txt` & `types-aiobotocore-dax-2.9.1/types_aiobotocore_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

