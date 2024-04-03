# Comparing `tmp/types-aiobotocore-dynamodbstreams-2.9.0.tar.gz` & `tmp/types-aiobotocore-dynamodbstreams-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.9.0.tar", last modified: Wed Dec 13 19:59:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.9.1.tar", last modified: Thu Jan 18 01:20:35 2024, max compression
```

## Comparing `types-aiobotocore-dynamodbstreams-2.9.0.tar` & `types-aiobotocore-dynamodbstreams-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.845807 types-aiobotocore-dynamodbstreams-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-12-13 19:59:09.845807 types-aiobotocore-dynamodbstreams-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11044 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:09.845807 types-aiobotocore-dynamodbstreams-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.845807 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9190 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9188 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2023-12-13 19:44:36.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2023-12-13 19:44:36.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:35.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:09.845807 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12639 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:09.000000 types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.009369 types-aiobotocore-dynamodbstreams-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-01-18 01:20:35.009369 types-aiobotocore-dynamodbstreams-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11044 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:35.009369 types-aiobotocore-dynamodbstreams-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.009369 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6926 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9188 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-01-18 01:06:31.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-01-18 01:06:30.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:29.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:35.009369 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:20:34.000000 types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/LICENSE` & `types-aiobotocore-dynamodbstreams-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
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
 
 <a id="types-aiobotocore-dynamodbstreams"></a>
 
 # types-aiobotocore-dynamodbstreams
 
 [![PyPI - types-aiobotocore-dynamodbstreams](https://img.shields.io/pypi/v/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/README.md` & `types-aiobotocore-dynamodbstreams-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/setup.py` & `types-aiobotocore-dynamodbstreams-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodbstreams",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DynamoDBStreams 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DynamoDBStreams 2.9.1 service generated with"
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
     keywords="aiobotocore dynamodbstreams type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dynamodbstreams": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/__main__.py` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDBStreams 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDBStreams 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/client.py` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,32 +26,29 @@
     GetRecordsOutputTypeDef,
     GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
 )
 
 __all__ = ("DynamoDBStreamsClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ExpiredIteratorException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TrimmedDataAccessException: Type[BotocoreClientError]
 
-
 class DynamoDBStreamsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/client/)
     """
 
     meta: ClientMeta
@@ -118,15 +115,15 @@
 
     async def get_shard_iterator(
         self,
         *,
         StreamArn: str,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
-        SequenceNumber: str = ...
+        SequenceNumber: str = ...,
     ) -> GetShardIteratorOutputTypeDef:
         """
         Returns a shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.get_shard_iterator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/client/#get_shard_iterator)
         """
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/client.pyi` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,29 +26,32 @@
     GetRecordsOutputTypeDef,
     GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
 )
 
 __all__ = ("DynamoDBStreamsClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ExpiredIteratorException: Type[BotocoreClientError]
     InternalServerError: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     TrimmedDataAccessException: Type[BotocoreClientError]
 
+
 class DynamoDBStreamsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/client/)
     """
 
     meta: ClientMeta
@@ -115,15 +118,15 @@
 
     async def get_shard_iterator(
         self,
         *,
         StreamArn: str,
         ShardId: str,
         ShardIteratorType: ShardIteratorTypeType,
-        SequenceNumber: str = ...
+        SequenceNumber: str = ...,
     ) -> GetShardIteratorOutputTypeDef:
         """
         Returns a shard iterator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams.Client.get_shard_iterator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/client/#get_shard_iterator)
         """
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/literals.py` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,28 +15,26 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "KeyTypeType",
     "OperationTypeType",
     "ShardIteratorTypeType",
     "StreamStatusType",
     "StreamViewTypeType",
     "DynamoDBStreamsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 KeyTypeType = Literal["HASH", "RANGE"]
 OperationTypeType = Literal["INSERT", "MODIFY", "REMOVE"]
 ShardIteratorTypeType = Literal[
     "AFTER_SEQUENCE_NUMBER", "AT_SEQUENCE_NUMBER", "LATEST", "TRIM_HORIZON"
 ]
 StreamStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLING"]
 StreamViewTypeType = Literal["KEYS_ONLY", "NEW_AND_OLD_IMAGES", "NEW_IMAGE", "OLD_IMAGE"]
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/literals.pyi` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/type_defs.py` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
     "IdentityTypeDef",
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams/type_defs.pyi` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
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
 
 <a id="types-aiobotocore-dynamodbstreams"></a>
 
 # types-aiobotocore-dynamodbstreams
 
 [![PyPI - types-aiobotocore-dynamodbstreams](https://img.shields.io/pypi/v/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DynamoDBStreams 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[aiobotocore.DynamoDBStreams 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-dynamodbstreams-2.9.0/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodbstreams-2.9.1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

