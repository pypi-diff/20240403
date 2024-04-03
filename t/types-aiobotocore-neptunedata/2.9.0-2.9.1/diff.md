# Comparing `tmp/types-aiobotocore-neptunedata-2.9.0.tar.gz` & `tmp/types-aiobotocore-neptunedata-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-neptunedata-2.9.0.tar", last modified: Wed Dec 13 20:00:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-neptunedata-2.9.1.tar", last modified: Thu Jan 18 01:21:22 2024, max compression
```

## Comparing `types-aiobotocore-neptunedata-2.9.0.tar` & `types-aiobotocore-neptunedata-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.965393 types-aiobotocore-neptunedata-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2023-12-13 20:00:00.965393 types-aiobotocore-neptunedata-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:00.965393 types-aiobotocore-neptunedata-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.965393 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35228 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35224 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    32867 2023-12-13 19:50:51.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32866 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:50.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:00.965393 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12457 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:00.000000 types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.173154 types-aiobotocore-neptunedata-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-01-18 01:21:22.173154 types-aiobotocore-neptunedata-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:22.173154 types-aiobotocore-neptunedata-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.169154 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35236 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    32866 2024-01-18 01:12:31.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32866 2024-01-18 01:12:31.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:30.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:22.173154 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12477 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:22.000000 types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/LICENSE` & `types-aiobotocore-neptunedata-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-neptunedata-2.9.0/PKG-INFO` & `types-aiobotocore-neptunedata-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptunedata
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NeptuneData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NeptuneData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/
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
 
 <a id="types-aiobotocore-neptunedata"></a>
 
 # types-aiobotocore-neptunedata
 
 [![PyPI - types-aiobotocore-neptunedata](https://img.shields.io/pypi/v/types-aiobotocore-neptunedata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptunedata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptunedata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptunedata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptunedata)](https://pepy.tech/project/types-aiobotocore-neptunedata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NeptuneData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
+[aiobotocore.NeptuneData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
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
 [types-aiobotocore-neptunedata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/README.md` & `types-aiobotocore-neptunedata-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptunedata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptunedata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptunedata)](https://pepy.tech/project/types-aiobotocore-neptunedata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NeptuneData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
+[aiobotocore.NeptuneData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
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
 [types-aiobotocore-neptunedata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/setup.py` & `types-aiobotocore-neptunedata-2.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-neptunedata",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_neptunedata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.NeptuneData 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.NeptuneData 2.9.1 service generated with"
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
     keywords="aiobotocore neptunedata type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_neptunedata": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/__main__.py` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NeptuneData 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.NeptuneData 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData\nOther"
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

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/client.py` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -81,26 +81,23 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("NeptuneDataClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     BulkLoadIdNotFoundException: Type[BotocoreClientError]
     CancelledByUserException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientTimeoutException: Type[BotocoreClientError]
@@ -130,15 +127,14 @@
     StatisticsNotAvailableException: Type[BotocoreClientError]
     StreamRecordsNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TimeLimitExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class NeptuneDataClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/)
     """
 
     meta: ClientMeta
@@ -231,15 +227,15 @@
         mlModelTrainingJobId: str = ...,
         mlModelTransformJobId: str = ...,
         update: bool = ...,
         neptuneIamRoleArn: str = ...,
         modelName: str = ...,
         instanceType: str = ...,
         instanceCount: int = ...,
-        volumeEncryptionKMSKey: str = ...
+        volumeEncryptionKMSKey: str = ...,
     ) -> CreateMLEndpointOutputTypeDef:
         """
         Creates a new Neptune ML inference endpoint that lets you query one specific
         model that the model-training process
         constructed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.create_ml_endpoint)
@@ -300,15 +296,15 @@
     async def execute_gremlin_profile_query(
         self,
         *,
         gremlinQuery: str,
         results: bool = ...,
         chop: int = ...,
         serializer: str = ...,
-        indexOps: bool = ...
+        indexOps: bool = ...,
     ) -> ExecuteGremlinProfileQueryOutputTypeDef:
         """
         Executes a Gremlin Profile query, which runs a specified traversal, collects
         various metrics about the run, and produces a profile report as
         output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.execute_gremlin_profile_query)
@@ -378,15 +374,15 @@
     async def get_loader_job_status(
         self,
         *,
         loadId: str,
         details: bool = ...,
         errors: bool = ...,
         page: int = ...,
-        errorsPerPage: int = ...
+        errorsPerPage: int = ...,
     ) -> GetLoaderJobStatusOutputTypeDef:
         """
         Gets status information about a specified load job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_loader_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_loader_job_status)
         """
@@ -452,15 +448,15 @@
     async def get_propertygraph_stream(
         self,
         *,
         limit: int = ...,
         iteratorType: IteratorTypeType = ...,
         commitNum: int = ...,
         opNum: int = ...,
-        encoding: Literal["gzip"] = ...
+        encoding: Literal["gzip"] = ...,
     ) -> GetPropertygraphStreamOutputTypeDef:
         """
         Gets a stream for a property graph.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_propertygraph_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_propertygraph_stream)
         """
@@ -496,15 +492,15 @@
     async def get_sparql_stream(
         self,
         *,
         limit: int = ...,
         iteratorType: IteratorTypeType = ...,
         commitNum: int = ...,
         opNum: int = ...,
-        encoding: Literal["gzip"] = ...
+        encoding: Literal["gzip"] = ...,
     ) -> GetSparqlStreamOutputTypeDef:
         """
         Gets a stream for an RDF graph.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_sparql_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_sparql_stream)
         """
@@ -609,15 +605,15 @@
         mode: ModeType = ...,
         failOnError: bool = ...,
         parallelism: ParallelismType = ...,
         parserConfiguration: Mapping[str, str] = ...,
         updateSingleCardinalityProperties: bool = ...,
         queueRequest: bool = ...,
         dependencies: Sequence[str] = ...,
-        userProvidedEdgeIds: bool = ...
+        userProvidedEdgeIds: bool = ...,
     ) -> StartLoaderJobOutputTypeDef:
         """
         Starts a Neptune bulk loader job to load data from an Amazon S3 bucket into a
         Neptune DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_loader_job)
@@ -637,15 +633,15 @@
         processingInstanceVolumeSizeInGB: int = ...,
         processingTimeOutInSeconds: int = ...,
         modelType: str = ...,
         configFileName: str = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
-        s3OutputEncryptionKMSKey: str = ...
+        s3OutputEncryptionKMSKey: str = ...,
     ) -> StartMLDataProcessingJobOutputTypeDef:
         """
         Creates a new Neptune ML data processing job for processing the graph data
         exported from Neptune for
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_data_processing_job)
@@ -668,15 +664,15 @@
         maxHPONumberOfTrainingJobs: int = ...,
         maxHPOParallelTrainingJobs: int = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
         s3OutputEncryptionKMSKey: str = ...,
         enableManagedSpotTraining: bool = ...,
-        customModelTrainingParameters: CustomModelTrainingParametersTypeDef = ...
+        customModelTrainingParameters: CustomModelTrainingParametersTypeDef = ...,
     ) -> StartMLModelTrainingJobOutputTypeDef:
         """
         Creates a new Neptune ML model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_model_training_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#start_ml_model_training_job)
         """
@@ -693,15 +689,15 @@
         neptuneIamRoleArn: str = ...,
         customModelTransformParameters: CustomModelTransformParametersTypeDef = ...,
         baseProcessingInstanceType: str = ...,
         baseProcessingInstanceVolumeSizeInGB: int = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
-        s3OutputEncryptionKMSKey: str = ...
+        s3OutputEncryptionKMSKey: str = ...,
     ) -> StartMLModelTransformJobOutputTypeDef:
         """
         Creates a new model transform job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_model_transform_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#start_ml_model_transform_job)
         """
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/client.pyi` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,21 +83,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("NeptuneDataClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     BulkLoadIdNotFoundException: Type[BotocoreClientError]
     CancelledByUserException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ClientTimeoutException: Type[BotocoreClientError]
@@ -127,14 +129,15 @@
     StatisticsNotAvailableException: Type[BotocoreClientError]
     StreamRecordsNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     TimeLimitExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class NeptuneDataClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/)
     """
 
     meta: ClientMeta
@@ -227,15 +230,15 @@
         mlModelTrainingJobId: str = ...,
         mlModelTransformJobId: str = ...,
         update: bool = ...,
         neptuneIamRoleArn: str = ...,
         modelName: str = ...,
         instanceType: str = ...,
         instanceCount: int = ...,
-        volumeEncryptionKMSKey: str = ...
+        volumeEncryptionKMSKey: str = ...,
     ) -> CreateMLEndpointOutputTypeDef:
         """
         Creates a new Neptune ML inference endpoint that lets you query one specific
         model that the model-training process
         constructed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.create_ml_endpoint)
@@ -296,15 +299,15 @@
     async def execute_gremlin_profile_query(
         self,
         *,
         gremlinQuery: str,
         results: bool = ...,
         chop: int = ...,
         serializer: str = ...,
-        indexOps: bool = ...
+        indexOps: bool = ...,
     ) -> ExecuteGremlinProfileQueryOutputTypeDef:
         """
         Executes a Gremlin Profile query, which runs a specified traversal, collects
         various metrics about the run, and produces a profile report as
         output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.execute_gremlin_profile_query)
@@ -374,15 +377,15 @@
     async def get_loader_job_status(
         self,
         *,
         loadId: str,
         details: bool = ...,
         errors: bool = ...,
         page: int = ...,
-        errorsPerPage: int = ...
+        errorsPerPage: int = ...,
     ) -> GetLoaderJobStatusOutputTypeDef:
         """
         Gets status information about a specified load job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_loader_job_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_loader_job_status)
         """
@@ -448,15 +451,15 @@
     async def get_propertygraph_stream(
         self,
         *,
         limit: int = ...,
         iteratorType: IteratorTypeType = ...,
         commitNum: int = ...,
         opNum: int = ...,
-        encoding: Literal["gzip"] = ...
+        encoding: Literal["gzip"] = ...,
     ) -> GetPropertygraphStreamOutputTypeDef:
         """
         Gets a stream for a property graph.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_propertygraph_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_propertygraph_stream)
         """
@@ -492,15 +495,15 @@
     async def get_sparql_stream(
         self,
         *,
         limit: int = ...,
         iteratorType: IteratorTypeType = ...,
         commitNum: int = ...,
         opNum: int = ...,
-        encoding: Literal["gzip"] = ...
+        encoding: Literal["gzip"] = ...,
     ) -> GetSparqlStreamOutputTypeDef:
         """
         Gets a stream for an RDF graph.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.get_sparql_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#get_sparql_stream)
         """
@@ -605,15 +608,15 @@
         mode: ModeType = ...,
         failOnError: bool = ...,
         parallelism: ParallelismType = ...,
         parserConfiguration: Mapping[str, str] = ...,
         updateSingleCardinalityProperties: bool = ...,
         queueRequest: bool = ...,
         dependencies: Sequence[str] = ...,
-        userProvidedEdgeIds: bool = ...
+        userProvidedEdgeIds: bool = ...,
     ) -> StartLoaderJobOutputTypeDef:
         """
         Starts a Neptune bulk loader job to load data from an Amazon S3 bucket into a
         Neptune DB
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_loader_job)
@@ -633,15 +636,15 @@
         processingInstanceVolumeSizeInGB: int = ...,
         processingTimeOutInSeconds: int = ...,
         modelType: str = ...,
         configFileName: str = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
-        s3OutputEncryptionKMSKey: str = ...
+        s3OutputEncryptionKMSKey: str = ...,
     ) -> StartMLDataProcessingJobOutputTypeDef:
         """
         Creates a new Neptune ML data processing job for processing the graph data
         exported from Neptune for
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_data_processing_job)
@@ -664,15 +667,15 @@
         maxHPONumberOfTrainingJobs: int = ...,
         maxHPOParallelTrainingJobs: int = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
         s3OutputEncryptionKMSKey: str = ...,
         enableManagedSpotTraining: bool = ...,
-        customModelTrainingParameters: CustomModelTrainingParametersTypeDef = ...
+        customModelTrainingParameters: CustomModelTrainingParametersTypeDef = ...,
     ) -> StartMLModelTrainingJobOutputTypeDef:
         """
         Creates a new Neptune ML model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_model_training_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#start_ml_model_training_job)
         """
@@ -689,15 +692,15 @@
         neptuneIamRoleArn: str = ...,
         customModelTransformParameters: CustomModelTransformParametersTypeDef = ...,
         baseProcessingInstanceType: str = ...,
         baseProcessingInstanceVolumeSizeInGB: int = ...,
         subnets: Sequence[str] = ...,
         securityGroupIds: Sequence[str] = ...,
         volumeEncryptionKMSKey: str = ...,
-        s3OutputEncryptionKMSKey: str = ...
+        s3OutputEncryptionKMSKey: str = ...,
     ) -> StartMLModelTransformJobOutputTypeDef:
         """
         Creates a new model transform job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData.Client.start_ml_model_transform_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/client/#start_ml_model_transform_job)
         """
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/literals.py` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/literals.py`

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
     "ActionType",
     "EncodingType",
     "FormatType",
     "GraphSummaryTypeType",
     "IteratorTypeType",
     "ModeType",
@@ -32,15 +31,14 @@
     "S3BucketRegionType",
     "StatisticsAutoGenerationModeType",
     "NeptuneDataServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 ActionType = Literal["initiateDatabaseReset", "performDatabaseReset"]
 EncodingType = Literal["gzip"]
 FormatType = Literal["csv", "nquads", "ntriples", "opencypher", "rdfxml", "turtle"]
 GraphSummaryTypeType = Literal["basic", "detailed"]
 IteratorTypeType = Literal["AFTER_SEQUENCE_NUMBER", "AT_SEQUENCE_NUMBER", "LATEST", "TRIM_HORIZON"]
 ModeType = Literal["AUTO", "NEW", "RESUME"]
 OpenCypherExplainModeType = Literal["details", "dynamic", "static"]
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/literals.pyi` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/type_defs.py` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelGremlinQueryInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelLoaderJobInputRequestTypeDef",
     "CancelMLDataProcessingJobInputRequestTypeDef",
     "CancelMLModelTrainingJobInputRequestTypeDef",
     "CancelMLModelTransformJobInputRequestTypeDef",
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata/type_defs.pyi` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/PKG-INFO` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-neptunedata
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.NeptuneData 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.NeptuneData 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/
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
 
 <a id="types-aiobotocore-neptunedata"></a>
 
 # types-aiobotocore-neptunedata
 
 [![PyPI - types-aiobotocore-neptunedata](https://img.shields.io/pypi/v/types-aiobotocore-neptunedata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptunedata)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-neptunedata.svg?color=blue)](https://pypi.org/project/types-aiobotocore-neptunedata)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-neptunedata)](https://pepy.tech/project/types-aiobotocore-neptunedata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.NeptuneData 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
+[aiobotocore.NeptuneData 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#NeptuneData)
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
 [types-aiobotocore-neptunedata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_neptunedata/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-neptunedata-2.9.0/types_aiobotocore_neptunedata.egg-info/SOURCES.txt` & `types-aiobotocore-neptunedata-2.9.1/types_aiobotocore_neptunedata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

