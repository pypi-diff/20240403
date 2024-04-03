# Comparing `tmp/types-aiobotocore-lambda-2.9.0.tar.gz` & `tmp/types-aiobotocore-lambda-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lambda-2.9.0.tar", last modified: Wed Dec 13 19:59:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-lambda-2.9.1.tar", last modified: Thu Jan 18 01:21:05 2024, max compression
```

## Comparing `types-aiobotocore-lambda-2.9.0.tar` & `types-aiobotocore-lambda-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.953548 types-aiobotocore-lambda-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15968 2023-12-13 19:59:42.953548 types-aiobotocore-lambda-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:42.953548 types-aiobotocore-lambda-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.953548 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62690 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    62686 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15231 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14420 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14406 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    72465 2023-12-13 19:48:49.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    72464 2023-12-13 19:48:49.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:47.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6548 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2023-12-13 19:48:48.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:42.953548 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15968 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:42.000000 types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.625229 types-aiobotocore-lambda-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-01-18 01:21:05.625229 types-aiobotocore-lambda-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:05.625229 types-aiobotocore-lambda-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.625229 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62714 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62711 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14411 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    72464 2024-01-18 01:10:37.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72464 2024-01-18 01:10:36.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:34.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6548 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-01-18 01:10:35.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:05.625229 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15988 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:05.000000 types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lambda-2.9.0/LICENSE` & `types-aiobotocore-lambda-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lambda-2.9.0/PKG-INFO` & `types-aiobotocore-lambda-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lambda
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Lambda 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Lambda 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/
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
 
 <a id="types-aiobotocore-lambda"></a>
 
 # types-aiobotocore-lambda
 
 [![PyPI - types-aiobotocore-lambda](https://img.shields.io/pypi/v/types-aiobotocore-lambda.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lambda.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lambda)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lambda)](https://pepy.tech/project/types-aiobotocore-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lambda 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[aiobotocore.Lambda 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [types-aiobotocore-lambda docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lambda-2.9.0/README.md` & `types-aiobotocore-lambda-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lambda.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lambda)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lambda)](https://pepy.tech/project/types-aiobotocore-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lambda 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[aiobotocore.Lambda 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [types-aiobotocore-lambda docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lambda-2.9.0/setup.py` & `types-aiobotocore-lambda-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lambda",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Lambda 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Lambda 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore lambda type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lambda": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__init__.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     FunctionUpdatedV2Waiter,
     FunctionUpdatedWaiter,
     PublishedVersionActiveWaiter,
 )
 
 Client = LambdaClient
 
-
 __all__ = (
     "Client",
     "FunctionActiveV2Waiter",
     "FunctionActiveWaiter",
     "FunctionExistsWaiter",
     "FunctionUpdatedV2Waiter",
     "FunctionUpdatedWaiter",
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__init__.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/__main__.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Lambda 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Lambda 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/client.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LambdaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -205,15 +204,15 @@
         *,
         LayerName: str,
         VersionNumber: int,
         StatementId: str,
         Action: str,
         Principal: str,
         OrganizationId: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> AddLayerVersionPermissionResponseTypeDef:
         """
         Adds permissions to the resource-based policy of a version of an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.add_layer_version_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#add_layer_version_permission)
@@ -228,15 +227,15 @@
         Principal: str,
         SourceArn: str = ...,
         SourceAccount: str = ...,
         EventSourceToken: str = ...,
         Qualifier: str = ...,
         RevisionId: str = ...,
         PrincipalOrgID: str = ...,
-        FunctionUrlAuthType: FunctionUrlAuthTypeType = ...
+        FunctionUrlAuthType: FunctionUrlAuthTypeType = ...,
     ) -> AddPermissionResponseTypeDef:
         """
         Grants an Amazon Web Service, Amazon Web Services account, or Amazon Web
         Services organization permission to use a
         function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.add_permission)
@@ -262,15 +261,15 @@
     async def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html)
         for a Lambda function
         version.
 
@@ -279,15 +278,15 @@
         """
 
     async def create_code_signing_config(
         self,
         *,
         AllowedPublishers: AllowedPublishersTypeDef,
         Description: str = ...,
-        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
+        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_code_signing_config)
         """
@@ -313,15 +312,15 @@
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
-        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_event_source_mapping)
         """
@@ -348,15 +347,15 @@
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...,
-        LoggingConfig: LoggingConfigTypeDef = ...
+        LoggingConfig: LoggingConfigTypeDef = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function)
         """
@@ -364,15 +363,15 @@
     async def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
         Cors: CorsTypeDef = ...,
-        InvokeMode: InvokeModeType = ...
+        InvokeMode: InvokeModeType = ...,
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function_url_config)
         """
@@ -669,15 +668,15 @@
         self,
         *,
         FunctionName: str,
         InvocationType: InvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Payload: BlobTypeDef = ...,
-        Qualifier: str = ...
+        Qualifier: str = ...,
     ) -> InvocationResponseTypeDef:
         """
         Invokes a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#invoke)
         """
@@ -696,30 +695,30 @@
         self,
         *,
         FunctionName: str,
         InvocationType: ResponseStreamingInvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Qualifier: str = ...,
-        Payload: BlobTypeDef = ...
+        Payload: BlobTypeDef = ...,
     ) -> InvokeWithResponseStreamResponseTypeDef:
         """
         Configure your Lambda functions to stream response payloads back to clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_with_response_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#invoke_with_response_stream)
         """
 
     async def list_aliases(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListAliasesResponseTypeDef:
         """
         Returns a list of
         [aliases](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html)
         for a Lambda
         function.
 
@@ -740,15 +739,15 @@
 
     async def list_event_source_mappings(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListEventSourceMappingsResponseTypeDef:
         """
         Lists event source mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_event_source_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_event_source_mappings)
         """
@@ -775,15 +774,15 @@
 
     async def list_functions(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListFunctionsResponseTypeDef:
         """
         Returns a list of Lambda functions, with the version-specific configuration of
         each.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_functions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_functions)
@@ -802,15 +801,15 @@
     async def list_layer_versions(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         Marker: str = ...,
         MaxItems: int = ...,
-        CompatibleArchitecture: ArchitectureType = ...
+        CompatibleArchitecture: ArchitectureType = ...,
     ) -> ListLayerVersionsResponseTypeDef:
         """
         Lists the versions of an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_layer_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_layer_versions)
@@ -818,15 +817,15 @@
 
     async def list_layers(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         Marker: str = ...,
         MaxItems: int = ...,
-        CompatibleArchitecture: ArchitectureType = ...
+        CompatibleArchitecture: ArchitectureType = ...,
     ) -> ListLayersResponseTypeDef:
         """
         Lists [Lambda
         layers](https://docs.aws.amazon.com/lambda/latest/dg/invocation-layers.html)
         and shows information about the latest version of
         each.
 
@@ -870,15 +869,15 @@
         self,
         *,
         LayerName: str,
         Content: LayerVersionContentInputTypeDef,
         Description: str = ...,
         CompatibleRuntimes: Sequence[RuntimeType] = ...,
         LicenseInfo: str = ...,
-        CompatibleArchitectures: Sequence[ArchitectureType] = ...
+        CompatibleArchitectures: Sequence[ArchitectureType] = ...,
     ) -> PublishLayerVersionResponseTypeDef:
         """
         Creates an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)
         from a ZIP
         archive.
 
@@ -888,15 +887,15 @@
 
     async def publish_version(
         self,
         *,
         FunctionName: str,
         CodeSha256: str = ...,
         Description: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a
         [version](https://docs.aws.amazon.com/lambda/latest/dg/versioning-aliases.html)
         from the current code and configuration of a
         function.
 
@@ -929,15 +928,15 @@
     async def put_function_event_invoke_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
-        DestinationConfig: DestinationConfigTypeDef = ...
+        DestinationConfig: DestinationConfigTypeDef = ...,
     ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Configures options for [asynchronous
         invocation](https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html)
         on a function, version, or
         alias.
 
@@ -957,15 +956,15 @@
 
     async def put_runtime_management_config(
         self,
         *,
         FunctionName: str,
         UpdateRuntimeOn: UpdateRuntimeOnType,
         Qualifier: str = ...,
-        RuntimeVersionArn: str = ...
+        RuntimeVersionArn: str = ...,
     ) -> PutRuntimeManagementConfigResponseTypeDef:
         """
         Sets the runtime management configuration for a function's version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_runtime_management_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#put_runtime_management_config)
         """
@@ -1020,15 +1019,15 @@
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_alias)
@@ -1036,15 +1035,15 @@
 
     async def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
         AllowedPublishers: AllowedPublishersTypeDef = ...,
-        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
+        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_code_signing_config)
         """
@@ -1063,15 +1062,15 @@
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
-        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_event_source_mapping)
         """
@@ -1084,15 +1083,15 @@
         S3Bucket: str = ...,
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
-        Architectures: Sequence[ArchitectureType] = ...
+        Architectures: Sequence[ArchitectureType] = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Updates a Lambda function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_code)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_code)
         """
@@ -1114,15 +1113,15 @@
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...,
-        LoggingConfig: LoggingConfigTypeDef = ...
+        LoggingConfig: LoggingConfigTypeDef = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_configuration)
         """
@@ -1130,15 +1129,15 @@
     async def update_function_event_invoke_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
-        DestinationConfig: DestinationConfigTypeDef = ...
+        DestinationConfig: DestinationConfigTypeDef = ...,
     ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Updates the configuration for asynchronous invocation for a function, version,
         or
         alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_event_invoke_config)
@@ -1148,15 +1147,15 @@
     async def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
         Cors: CorsTypeDef = ...,
-        InvokeMode: InvokeModeType = ...
+        InvokeMode: InvokeModeType = ...,
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_url_config)
         """
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/client.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         *,
         LayerName: str,
         VersionNumber: int,
         StatementId: str,
         Action: str,
         Principal: str,
         OrganizationId: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> AddLayerVersionPermissionResponseTypeDef:
         """
         Adds permissions to the resource-based policy of a version of an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.add_layer_version_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#add_layer_version_permission)
@@ -224,15 +224,15 @@
         Principal: str,
         SourceArn: str = ...,
         SourceAccount: str = ...,
         EventSourceToken: str = ...,
         Qualifier: str = ...,
         RevisionId: str = ...,
         PrincipalOrgID: str = ...,
-        FunctionUrlAuthType: FunctionUrlAuthTypeType = ...
+        FunctionUrlAuthType: FunctionUrlAuthTypeType = ...,
     ) -> AddPermissionResponseTypeDef:
         """
         Grants an Amazon Web Service, Amazon Web Services account, or Amazon Web
         Services organization permission to use a
         function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.add_permission)
@@ -258,15 +258,15 @@
     async def create_alias(
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
-        RoutingConfig: AliasRoutingConfigurationTypeDef = ...
+        RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
     ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html)
         for a Lambda function
         version.
 
@@ -275,15 +275,15 @@
         """
 
     async def create_code_signing_config(
         self,
         *,
         AllowedPublishers: AllowedPublishersTypeDef,
         Description: str = ...,
-        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
+        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,
     ) -> CreateCodeSigningConfigResponseTypeDef:
         """
         Creates a code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_code_signing_config)
         """
@@ -309,15 +309,15 @@
         Queues: Sequence[str] = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
-        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_event_source_mapping)
         """
@@ -344,15 +344,15 @@
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...,
-        LoggingConfig: LoggingConfigTypeDef = ...
+        LoggingConfig: LoggingConfigTypeDef = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function)
         """
@@ -360,15 +360,15 @@
     async def create_function_url_config(
         self,
         *,
         FunctionName: str,
         AuthType: FunctionUrlAuthTypeType,
         Qualifier: str = ...,
         Cors: CorsTypeDef = ...,
-        InvokeMode: InvokeModeType = ...
+        InvokeMode: InvokeModeType = ...,
     ) -> CreateFunctionUrlConfigResponseTypeDef:
         """
         Creates a Lambda function URL with the specified configuration parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#create_function_url_config)
         """
@@ -665,15 +665,15 @@
         self,
         *,
         FunctionName: str,
         InvocationType: InvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Payload: BlobTypeDef = ...,
-        Qualifier: str = ...
+        Qualifier: str = ...,
     ) -> InvocationResponseTypeDef:
         """
         Invokes a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#invoke)
         """
@@ -692,30 +692,30 @@
         self,
         *,
         FunctionName: str,
         InvocationType: ResponseStreamingInvocationTypeType = ...,
         LogType: LogTypeType = ...,
         ClientContext: str = ...,
         Qualifier: str = ...,
-        Payload: BlobTypeDef = ...
+        Payload: BlobTypeDef = ...,
     ) -> InvokeWithResponseStreamResponseTypeDef:
         """
         Configure your Lambda functions to stream response payloads back to clients.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.invoke_with_response_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#invoke_with_response_stream)
         """
 
     async def list_aliases(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListAliasesResponseTypeDef:
         """
         Returns a list of
         [aliases](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html)
         for a Lambda
         function.
 
@@ -736,15 +736,15 @@
 
     async def list_event_source_mappings(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListEventSourceMappingsResponseTypeDef:
         """
         Lists event source mappings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_event_source_mappings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_event_source_mappings)
         """
@@ -771,15 +771,15 @@
 
     async def list_functions(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListFunctionsResponseTypeDef:
         """
         Returns a list of Lambda functions, with the version-specific configuration of
         each.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_functions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_functions)
@@ -798,15 +798,15 @@
     async def list_layer_versions(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         Marker: str = ...,
         MaxItems: int = ...,
-        CompatibleArchitecture: ArchitectureType = ...
+        CompatibleArchitecture: ArchitectureType = ...,
     ) -> ListLayerVersionsResponseTypeDef:
         """
         Lists the versions of an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.list_layer_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#list_layer_versions)
@@ -814,15 +814,15 @@
 
     async def list_layers(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         Marker: str = ...,
         MaxItems: int = ...,
-        CompatibleArchitecture: ArchitectureType = ...
+        CompatibleArchitecture: ArchitectureType = ...,
     ) -> ListLayersResponseTypeDef:
         """
         Lists [Lambda
         layers](https://docs.aws.amazon.com/lambda/latest/dg/invocation-layers.html)
         and shows information about the latest version of
         each.
 
@@ -866,15 +866,15 @@
         self,
         *,
         LayerName: str,
         Content: LayerVersionContentInputTypeDef,
         Description: str = ...,
         CompatibleRuntimes: Sequence[RuntimeType] = ...,
         LicenseInfo: str = ...,
-        CompatibleArchitectures: Sequence[ArchitectureType] = ...
+        CompatibleArchitectures: Sequence[ArchitectureType] = ...,
     ) -> PublishLayerVersionResponseTypeDef:
         """
         Creates an [Lambda
         layer](https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html)
         from a ZIP
         archive.
 
@@ -884,15 +884,15 @@
 
     async def publish_version(
         self,
         *,
         FunctionName: str,
         CodeSha256: str = ...,
         Description: str = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a
         [version](https://docs.aws.amazon.com/lambda/latest/dg/versioning-aliases.html)
         from the current code and configuration of a
         function.
 
@@ -925,15 +925,15 @@
     async def put_function_event_invoke_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
-        DestinationConfig: DestinationConfigTypeDef = ...
+        DestinationConfig: DestinationConfigTypeDef = ...,
     ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Configures options for [asynchronous
         invocation](https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html)
         on a function, version, or
         alias.
 
@@ -953,15 +953,15 @@
 
     async def put_runtime_management_config(
         self,
         *,
         FunctionName: str,
         UpdateRuntimeOn: UpdateRuntimeOnType,
         Qualifier: str = ...,
-        RuntimeVersionArn: str = ...
+        RuntimeVersionArn: str = ...,
     ) -> PutRuntimeManagementConfigResponseTypeDef:
         """
         Sets the runtime management configuration for a function's version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_runtime_management_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#put_runtime_management_config)
         """
@@ -1016,15 +1016,15 @@
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
-        RevisionId: str = ...
+        RevisionId: str = ...,
     ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-aliases.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_alias)
@@ -1032,15 +1032,15 @@
 
     async def update_code_signing_config(
         self,
         *,
         CodeSigningConfigArn: str,
         Description: str = ...,
         AllowedPublishers: AllowedPublishersTypeDef = ...,
-        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...
+        CodeSigningPolicies: CodeSigningPoliciesTypeDef = ...,
     ) -> UpdateCodeSigningConfigResponseTypeDef:
         """
         Update the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_code_signing_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_code_signing_config)
         """
@@ -1059,15 +1059,15 @@
         BisectBatchOnFunctionError: bool = ...,
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
-        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
+        DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...,
     ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_event_source_mapping)
         """
@@ -1080,15 +1080,15 @@
         S3Bucket: str = ...,
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
-        Architectures: Sequence[ArchitectureType] = ...
+        Architectures: Sequence[ArchitectureType] = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Updates a Lambda function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_code)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_code)
         """
@@ -1110,15 +1110,15 @@
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...,
-        LoggingConfig: LoggingConfigTypeDef = ...
+        LoggingConfig: LoggingConfigTypeDef = ...,
     ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_configuration)
         """
@@ -1126,15 +1126,15 @@
     async def update_function_event_invoke_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
-        DestinationConfig: DestinationConfigTypeDef = ...
+        DestinationConfig: DestinationConfigTypeDef = ...,
     ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Updates the configuration for asynchronous invocation for a function, version,
         or
         alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_event_invoke_config)
@@ -1144,15 +1144,15 @@
     async def update_function_url_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         AuthType: FunctionUrlAuthTypeType = ...,
         Cors: CorsTypeDef = ...,
-        InvokeMode: InvokeModeType = ...
+        InvokeMode: InvokeModeType = ...,
     ) -> UpdateFunctionUrlConfigResponseTypeDef:
         """
         Updates the configuration for a Lambda function URL.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_url_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/client/#update_function_url_config)
         """
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/literals.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/literals.py`

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
     "ApplicationLogLevelType",
     "ArchitectureType",
     "CodeSigningPolicyType",
     "EndPointTypeType",
     "EventSourcePositionType",
     "FullDocumentType",
@@ -69,15 +68,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ApplicationLogLevelType = Literal["DEBUG", "ERROR", "FATAL", "INFO", "TRACE", "WARN"]
 ArchitectureType = Literal["arm64", "x86_64"]
 CodeSigningPolicyType = Literal["Enforce", "Warn"]
 EndPointTypeType = Literal["KAFKA_BOOTSTRAP_SERVERS"]
 EventSourcePositionType = Literal["AT_TIMESTAMP", "LATEST", "TRIM_HORIZON"]
 FullDocumentType = Literal["Default", "UpdateLookup"]
 FunctionActiveV2WaiterName = Literal["function_active_v2"]
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/literals.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/paginator.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,30 +64,28 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAliasesPaginator",
     "ListCodeSigningConfigsPaginator",
     "ListEventSourceMappingsPaginator",
     "ListFunctionEventInvokeConfigsPaginator",
     "ListFunctionUrlConfigsPaginator",
     "ListFunctionsPaginator",
     "ListFunctionsByCodeSigningConfigPaginator",
     "ListLayerVersionsPaginator",
     "ListLayersPaginator",
     "ListProvisionedConcurrencyConfigsPaginator",
     "ListVersionsByFunctionPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -101,15 +99,15 @@
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listaliasespaginator)
         """
 
 
@@ -135,15 +133,15 @@
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventSourceMappingsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
 
@@ -184,15 +182,15 @@
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFunctionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listfunctionspaginator)
         """
 
 
@@ -219,15 +217,15 @@
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listlayerversionspaginator)
         """
 
 
@@ -238,15 +236,15 @@
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listlayerspaginator)
         """
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/paginator.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listaliasespaginator)
         """
 
 class ListCodeSigningConfigsPaginator(AioPaginator):
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEventSourceMappingsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
 class ListFunctionEventInvokeConfigsPaginator(AioPaginator):
@@ -175,15 +175,15 @@
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFunctionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listfunctionspaginator)
         """
 
 class ListFunctionsByCodeSigningConfigPaginator(AioPaginator):
@@ -208,15 +208,15 @@
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listlayerversionspaginator)
         """
 
 class ListLayersPaginator(AioPaginator):
@@ -226,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/paginators/#listlayerspaginator)
         """
 
 class ListProvisionedConcurrencyConfigsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/type_defs.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "AliasRoutingConfigurationPaginatorTypeDef",
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/type_defs.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/waiter.py` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda/waiter.pyi` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/PKG-INFO` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lambda
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Lambda 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Lambda 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/
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
 
 <a id="types-aiobotocore-lambda"></a>
 
 # types-aiobotocore-lambda
 
 [![PyPI - types-aiobotocore-lambda](https://img.shields.io/pypi/v/types-aiobotocore-lambda.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lambda.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lambda)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lambda)](https://pepy.tech/project/types-aiobotocore-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Lambda 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[aiobotocore.Lambda 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [types-aiobotocore-lambda docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lambda/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lambda-2.9.0/types_aiobotocore_lambda.egg-info/SOURCES.txt` & `types-aiobotocore-lambda-2.9.1/types_aiobotocore_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

