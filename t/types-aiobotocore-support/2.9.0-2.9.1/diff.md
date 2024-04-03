# Comparing `tmp/types-aiobotocore-support-2.9.0.tar.gz` & `tmp/types-aiobotocore-support-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-2.9.0.tar", last modified: Wed Dec 13 20:00:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-2.9.1.tar", last modified: Thu Jan 18 01:21:56 2024, max compression
```

## Comparing `types-aiobotocore-support-2.9.0.tar` & `types-aiobotocore-support-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.273063 types-aiobotocore-support-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13137 2023-12-13 20:00:39.273063 types-aiobotocore-support-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:39.273063 types-aiobotocore-support-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.273063 types-aiobotocore-support-2.9.0/types_aiobotocore_support/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16292 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16288 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8406 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16673 2023-12-13 19:57:12.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16672 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:11.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:39.273063 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13137 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:39.000000 types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.828998 types-aiobotocore-support-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-01-18 01:21:56.824998 types-aiobotocore-support-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:56.828998 types-aiobotocore-support-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.824998 types-aiobotocore-support-2.9.1/types_aiobotocore_support/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16295 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16672 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16672 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:39.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:56.824998 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:56.000000 types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-2.9.0/LICENSE` & `types-aiobotocore-support-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-support-2.9.0/PKG-INFO` & `types-aiobotocore-support-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Support 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Support 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
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
 
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-2.9.0/README.md` & `types-aiobotocore-support-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-2.9.0/setup.py` & `types-aiobotocore-support-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_support"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Support 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Support 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore support type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_support": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/__init__.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import SupportClient
 from .paginator import DescribeCasesPaginator, DescribeCommunicationsPaginator
 
 Client = SupportClient
 
-
 __all__ = ("Client", "DescribeCasesPaginator", "DescribeCommunicationsPaginator", "SupportClient")
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/__init__.pyi` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/__main__.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Support 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Support 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support\nOther"
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

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/client.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SupportClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -102,15 +101,15 @@
 
     async def add_communication_to_case(
         self,
         *,
         communicationBody: str,
         caseId: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> AddCommunicationToCaseResponseTypeDef:
         """
         Adds additional customer communication to an Amazon Web Services Support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_communication_to_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_communication_to_case)
         """
@@ -138,15 +137,15 @@
         communicationBody: str,
         serviceCode: str = ...,
         severityCode: str = ...,
         categoryCode: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
         language: str = ...,
         issueType: str = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the Amazon Web Services Support Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.create_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#create_case)
         """
@@ -166,15 +165,15 @@
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         language: str = ...,
-        includeCommunications: bool = ...
+        includeCommunications: bool = ...,
     ) -> DescribeCasesResponseTypeDef:
         """
         Returns a list of cases that you specify by passing one or more case IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#describe_cases)
         """
@@ -182,15 +181,15 @@
     async def describe_communications(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeCommunicationsResponseTypeDef:
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#describe_communications)
         """
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/client.pyi` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     async def add_communication_to_case(
         self,
         *,
         communicationBody: str,
         caseId: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> AddCommunicationToCaseResponseTypeDef:
         """
         Adds additional customer communication to an Amazon Web Services Support case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_communication_to_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#add_communication_to_case)
         """
@@ -134,15 +134,15 @@
         communicationBody: str,
         serviceCode: str = ...,
         severityCode: str = ...,
         categoryCode: str = ...,
         ccEmailAddresses: Sequence[str] = ...,
         language: str = ...,
         issueType: str = ...,
-        attachmentSetId: str = ...
+        attachmentSetId: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the Amazon Web Services Support Center.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.create_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#create_case)
         """
@@ -162,15 +162,15 @@
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         language: str = ...,
-        includeCommunications: bool = ...
+        includeCommunications: bool = ...,
     ) -> DescribeCasesResponseTypeDef:
         """
         Returns a list of cases that you specify by passing one or more case IDs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#describe_cases)
         """
@@ -178,15 +178,15 @@
     async def describe_communications(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeCommunicationsResponseTypeDef:
         """
         Returns communications and attachments for one or more support cases.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/client/#describe_communications)
         """
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/literals.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeCasesPaginatorName",
     "DescribeCommunicationsPaginatorName",
     "SupportServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 DescribeCasesPaginatorName = Literal["describe_cases"]
 DescribeCommunicationsPaginatorName = Literal["describe_communications"]
 SupportServiceName = Literal["support"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/literals.pyi` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/paginator.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     DescribeCasesResponseTypeDef,
     DescribeCommunicationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeCasesPaginator", "DescribeCommunicationsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecasespaginator)
         """
 
 
@@ -79,13 +78,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/paginator.pyi` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         caseIdList: Sequence[str] = ...,
         displayId: str = ...,
         afterTime: str = ...,
         beforeTime: str = ...,
         includeResolvedCases: bool = ...,
         language: str = ...,
         includeCommunications: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecasespaginator)
         """
 
 class DescribeCommunicationsPaginator(AioPaginator):
@@ -75,13 +75,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         beforeTime: str = ...,
         afterTime: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeCommunicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Paginator.DescribeCommunications.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/paginators/#describecommunicationspaginator)
         """
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/type_defs.py` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseMetadataTypeDef",
     "AddCommunicationToCaseRequestRequestTypeDef",
     "AttachmentDetailsTypeDef",
     "BlobTypeDef",
     "CategoryTypeDef",
     "DateIntervalTypeDef",
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support/type_defs.pyi` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/PKG-INFO` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Support 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Support 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/
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
 
 <a id="types-aiobotocore-support"></a>
 
 # types-aiobotocore-support
 
 [![PyPI - types-aiobotocore-support](https://img.shields.io/pypi/v/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-support)](https://pepy.tech/project/types-aiobotocore-support)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Support 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
+[aiobotocore.Support 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
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
 [types-aiobotocore-support docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-support-2.9.0/types_aiobotocore_support.egg-info/SOURCES.txt` & `types-aiobotocore-support-2.9.1/types_aiobotocore_support.egg-info/SOURCES.txt`

 * *Files identical despite different names*

