# Comparing `tmp/types-aiobotocore-lex-runtime-2.9.0.tar.gz` & `tmp/types-aiobotocore-lex-runtime-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-runtime-2.9.0.tar", last modified: Wed Dec 13 19:59:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-runtime-2.9.1.tar", last modified: Thu Jan 18 01:21:06 2024, max compression
```

## Comparing `types-aiobotocore-lex-runtime-2.9.0.tar` & `types-aiobotocore-lex-runtime-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.073539 types-aiobotocore-lex-runtime-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2023-12-13 19:59:44.073539 types-aiobotocore-lex-runtime-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:44.073539 types-aiobotocore-lex-runtime-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.073539 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (127)      505 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8262 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:54.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:44.073539 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 19:59:44.000000 types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.685225 types-aiobotocore-lex-runtime-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-01-18 01:21:06.685225 types-aiobotocore-lex-runtime-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:06.685225 types-aiobotocore-lex-runtime-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.685225 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8262 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:41.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:06.685225 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:06.000000 types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/LICENSE` & `types-aiobotocore-lex-runtime-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-lex-runtime-2.9.0/PKG-INFO` & `types-aiobotocore-lex-runtime-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
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
 
 <a id="types-aiobotocore-lex-runtime"></a>
 
 # types-aiobotocore-lex-runtime
 
 [![PyPI - types-aiobotocore-lex-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/README.md` & `types-aiobotocore-lex-runtime-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/setup.py` & `types-aiobotocore-lex-runtime-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-runtime",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.LexRuntimeService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.LexRuntimeService 2.9.1 service generated with"
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
     keywords="aiobotocore lex-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lex_runtime": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/__main__.py` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.LexRuntimeService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/client.py` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,38 +30,35 @@
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadGatewayException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailedException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     LoopDetectedException: Type[BotocoreClientError]
     NotAcceptableException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     RequestTimeoutException: Type[BotocoreClientError]
     UnsupportedMediaTypeException: Type[BotocoreClientError]
 
-
 class LexRuntimeServiceClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/)
     """
 
     meta: ClientMeta
@@ -132,15 +129,15 @@
         botAlias: str,
         userId: str,
         contentType: str,
         inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
-        activeContexts: str = ...
+        activeContexts: str = ...,
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_content)
         """
@@ -150,15 +147,15 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...,
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
@@ -169,15 +166,15 @@
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
         dialogAction: DialogActionTypeDef = ...,
         recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...,
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/client.pyi` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,35 +30,38 @@
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadGatewayException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     DependencyFailedException: Type[BotocoreClientError]
     InternalFailureException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     LoopDetectedException: Type[BotocoreClientError]
     NotAcceptableException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     RequestTimeoutException: Type[BotocoreClientError]
     UnsupportedMediaTypeException: Type[BotocoreClientError]
 
+
 class LexRuntimeServiceClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/)
     """
 
     meta: ClientMeta
@@ -129,15 +132,15 @@
         botAlias: str,
         userId: str,
         contentType: str,
         inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
-        activeContexts: str = ...
+        activeContexts: str = ...,
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_content)
         """
@@ -147,15 +150,15 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...,
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
@@ -166,15 +169,15 @@
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
         dialogAction: DialogActionTypeDef = ...,
         recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextTypeDef] = ...,
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/literals.py` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ConfirmationStatusType",
     "ContentTypeType",
     "DialogActionTypeType",
     "DialogStateType",
     "FulfillmentStateType",
     "MessageFormatTypeType",
     "LexRuntimeServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 ConfirmationStatusType = Literal["Confirmed", "Denied", "None"]
 ContentTypeType = Literal["application/vnd.amazonaws.card.generic"]
 DialogActionTypeType = Literal["Close", "ConfirmIntent", "Delegate", "ElicitIntent", "ElicitSlot"]
 DialogStateType = Literal[
     "ConfirmIntent", "ElicitIntent", "ElicitSlot", "Failed", "Fulfilled", "ReadyForFulfillment"
 ]
 FulfillmentStateType = Literal["Failed", "Fulfilled", "ReadyForFulfillment"]
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/literals.pyi` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/type_defs.py` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/type_defs.py`

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
     "ActiveContextTimeToLiveTypeDef",
     "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime/type_defs.pyi` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
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
 
 <a id="types-aiobotocore-lex-runtime"></a>
 
 # types-aiobotocore-lex-runtime
 
 [![PyPI - types-aiobotocore-lex-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.LexRuntimeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[aiobotocore.LexRuntimeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-lex-runtime-2.9.0/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lex-runtime-2.9.1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

