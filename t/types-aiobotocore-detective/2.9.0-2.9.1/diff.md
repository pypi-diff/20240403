# Comparing `tmp/types-aiobotocore-detective-2.9.0.tar.gz` & `tmp/types-aiobotocore-detective-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-detective-2.9.0.tar", last modified: Wed Dec 13 19:59:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-detective-2.9.1.tar", last modified: Thu Jan 18 01:20:30 2024, max compression
```

## Comparing `types-aiobotocore-detective-2.9.0.tar` & `types-aiobotocore-detective-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.325844 types-aiobotocore-detective-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2023-12-13 19:59:05.325844 types-aiobotocore-detective-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10824 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:05.325844 types-aiobotocore-detective-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.325844 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21807 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    21804 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2023-12-13 19:43:59.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20844 2023-12-13 19:43:59.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20843 2023-12-13 19:43:59.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:58.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:05.325844 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:05.000000 types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.817392 types-aiobotocore-detective-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-01-18 01:20:30.817392 types-aiobotocore-detective-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10824 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:30.817392 types-aiobotocore-detective-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.817392 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20843 2024-01-18 01:05:54.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20843 2024-01-18 01:05:54.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:53.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:30.817392 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:30.000000 types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-detective-2.9.0/LICENSE` & `types-aiobotocore-detective-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-detective-2.9.0/PKG-INFO` & `types-aiobotocore-detective-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-detective
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Detective 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Detective 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/
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
 
 <a id="types-aiobotocore-detective"></a>
 
 # types-aiobotocore-detective
 
 [![PyPI - types-aiobotocore-detective](https://img.shields.io/pypi/v/types-aiobotocore-detective.svg?color=blue)](https://pypi.org/project/types-aiobotocore-detective)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-detective.svg?color=blue)](https://pypi.org/project/types-aiobotocore-detective)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-detective)](https://pepy.tech/project/types-aiobotocore-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Detective 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[aiobotocore.Detective 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [types-aiobotocore-detective docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-detective-2.9.0/README.md` & `types-aiobotocore-detective-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-detective.svg?color=blue)](https://pypi.org/project/types-aiobotocore-detective)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-detective)](https://pepy.tech/project/types-aiobotocore-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Detective 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[aiobotocore.Detective 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [types-aiobotocore-detective docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-detective-2.9.0/setup.py` & `types-aiobotocore-detective-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-detective",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_detective"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Detective 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Detective 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore detective type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_detective": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/__main__.py` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Detective 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Detective 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective\nOther"
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

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/client.py` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -44,34 +44,31 @@
     SortCriteriaTypeDef,
     StartInvestigationResponseTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("DetectiveClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class DetectiveClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/)
     """
 
     meta: ClientMeta
@@ -142,15 +139,15 @@
 
     async def create_members(
         self,
         *,
         GraphArn: str,
         Accounts: Sequence[AccountTypeDef],
         Message: str = ...,
-        DisableEmailNotification: bool = ...
+        DisableEmailNotification: bool = ...,
     ) -> CreateMembersResponseTypeDef:
         """
         `CreateMembers` is used to send invitations to accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#create_members)
         """
@@ -271,15 +268,15 @@
     async def list_indicators(
         self,
         *,
         GraphArn: str,
         InvestigationId: str,
         IndicatorType: IndicatorTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIndicatorsResponseTypeDef:
         """
         Get the indicators from an investigation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/detective-2018-10-26/ListIndicators).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_indicators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#list_indicators)
@@ -288,15 +285,15 @@
     async def list_investigations(
         self,
         *,
         GraphArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: FilterCriteriaTypeDef = ...,
-        SortCriteria: SortCriteriaTypeDef = ...
+        SortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListInvestigationsResponseTypeDef:
         """
         List all Investigations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_investigations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#list_investigations)
         """
@@ -354,15 +351,15 @@
 
     async def start_investigation(
         self,
         *,
         GraphArn: str,
         EntityArn: str,
         ScopeStartTime: TimestampTypeDef,
-        ScopeEndTime: TimestampTypeDef
+        ScopeEndTime: TimestampTypeDef,
     ) -> StartInvestigationResponseTypeDef:
         """
         initiate an investigation on an entity in a graph See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/detective-2018-10-26/StartInvestigation).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_investigation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#start_investigation)
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/client.pyi` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,31 +44,34 @@
     SortCriteriaTypeDef,
     StartInvestigationResponseTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("DetectiveClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class DetectiveClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/)
     """
 
     meta: ClientMeta
@@ -139,15 +142,15 @@
 
     async def create_members(
         self,
         *,
         GraphArn: str,
         Accounts: Sequence[AccountTypeDef],
         Message: str = ...,
-        DisableEmailNotification: bool = ...
+        DisableEmailNotification: bool = ...,
     ) -> CreateMembersResponseTypeDef:
         """
         `CreateMembers` is used to send invitations to accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.create_members)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#create_members)
         """
@@ -268,15 +271,15 @@
     async def list_indicators(
         self,
         *,
         GraphArn: str,
         InvestigationId: str,
         IndicatorType: IndicatorTypeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListIndicatorsResponseTypeDef:
         """
         Get the indicators from an investigation See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/detective-2018-10-26/ListIndicators).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_indicators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#list_indicators)
@@ -285,15 +288,15 @@
     async def list_investigations(
         self,
         *,
         GraphArn: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         FilterCriteria: FilterCriteriaTypeDef = ...,
-        SortCriteria: SortCriteriaTypeDef = ...
+        SortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListInvestigationsResponseTypeDef:
         """
         List all Investigations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.list_investigations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#list_investigations)
         """
@@ -351,15 +354,15 @@
 
     async def start_investigation(
         self,
         *,
         GraphArn: str,
         EntityArn: str,
         ScopeStartTime: TimestampTypeDef,
-        ScopeEndTime: TimestampTypeDef
+        ScopeEndTime: TimestampTypeDef,
     ) -> StartInvestigationResponseTypeDef:
         """
         initiate an investigation on an entity in a graph See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/detective-2018-10-26/StartInvestigation).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective.Client.start_investigation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/client/#start_investigation)
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/literals.py` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DatasourcePackageIngestStateType",
     "DatasourcePackageType",
     "EntityTypeType",
     "FieldType",
     "IndicatorTypeType",
     "InvitationTypeType",
@@ -36,15 +35,14 @@
     "StatusType",
     "DetectiveServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 DatasourcePackageIngestStateType = Literal["DISABLED", "STARTED", "STOPPED"]
 DatasourcePackageType = Literal["ASFF_SECURITYHUB_FINDING", "DETECTIVE_CORE", "EKS_AUDIT"]
 EntityTypeType = Literal["IAM_ROLE", "IAM_USER"]
 FieldType = Literal["CREATED_TIME", "SEVERITY", "STATUS"]
 IndicatorTypeType = Literal[
     "FLAGGED_IP_ADDRESS",
     "IMPOSSIBLE_TRAVEL",
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/literals.pyi` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/type_defs.py` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccountTypeDef",
     "AdministratorTypeDef",
     "BatchGetGraphMemberDatasourcesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedAccountTypeDef",
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective/type_defs.pyi` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/PKG-INFO` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-detective
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Detective 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Detective 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/
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
 
 <a id="types-aiobotocore-detective"></a>
 
 # types-aiobotocore-detective
 
 [![PyPI - types-aiobotocore-detective](https://img.shields.io/pypi/v/types-aiobotocore-detective.svg?color=blue)](https://pypi.org/project/types-aiobotocore-detective)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-detective.svg?color=blue)](https://pypi.org/project/types-aiobotocore-detective)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-detective)](https://pepy.tech/project/types-aiobotocore-detective)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Detective 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
+[aiobotocore.Detective 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#Detective)
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
 [types-aiobotocore-detective docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_detective/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-detective-2.9.0/types_aiobotocore_detective.egg-info/SOURCES.txt` & `types-aiobotocore-detective-2.9.1/types_aiobotocore_detective.egg-info/SOURCES.txt`

 * *Files identical despite different names*

