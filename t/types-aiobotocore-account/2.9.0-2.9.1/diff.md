# Comparing `tmp/types-aiobotocore-account-2.9.0.tar.gz` & `tmp/types-aiobotocore-account-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-account-2.9.0.tar", last modified: Wed Dec 13 19:58:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-account-2.9.1.tar", last modified: Thu Jan 18 01:19:57 2024, max compression
```

## Comparing `types-aiobotocore-account-2.9.0.tar` & `types-aiobotocore-account-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.018142 types-aiobotocore-account-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2023-12-13 19:58:29.018142 types-aiobotocore-account-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:29.018142 types-aiobotocore-account-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.018142 types-aiobotocore-account-2.9.0/types_aiobotocore_account/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10275 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2023-12-13 19:40:35.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8473 2023-12-13 19:40:35.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2023-12-13 19:40:35.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2023-12-13 19:40:35.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:34.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:29.018142 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:28.000000 types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.605540 types-aiobotocore-account-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-01-18 01:19:57.605540 types-aiobotocore-account-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:57.605540 types-aiobotocore-account-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.605540 types-aiobotocore-account-2.9.1/types_aiobotocore_account/
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8473 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:34.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:57.605540 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:19:57.000000 types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-account-2.9.0/LICENSE` & `types-aiobotocore-account-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-account-2.9.0/PKG-INFO` & `types-aiobotocore-account-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Account 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Account 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
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
 
 <a id="types-aiobotocore-account"></a>
 
 # types-aiobotocore-account
 
 [![PyPI - types-aiobotocore-account](https://img.shields.io/pypi/v/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Account 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[aiobotocore.Account 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-account-2.9.0/README.md` & `types-aiobotocore-account-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Account 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[aiobotocore.Account 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-account-2.9.0/setup.py` & `types-aiobotocore-account-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-account",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Account 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Account 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore account type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_account": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/__init__.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import AccountClient
 from .paginator import ListRegionsPaginator
 
 Client = AccountClient
 
-
 __all__ = ("AccountClient", "Client", "ListRegionsPaginator")
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/__init__.pyi` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/__main__.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Account 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Account 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
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

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/client.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AccountClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -169,15 +168,15 @@
 
     async def list_regions(
         self,
         *,
         AccountId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        RegionOptStatusContains: Sequence[RegionOptStatusType] = ...
+        RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,
     ) -> ListRegionsResponseTypeDef:
         """
         Lists all the Regions for a given account and their respective opt-in statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.list_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/client/#list_regions)
         """
@@ -186,15 +185,15 @@
         self,
         *,
         AlternateContactType: AlternateContactTypeType,
         EmailAddress: str,
         Name: str,
         PhoneNumber: str,
         Title: str,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies the specified alternate contact attached to an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.put_alternate_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/client/#put_alternate_contact)
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/client.pyi` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 
     async def list_regions(
         self,
         *,
         AccountId: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        RegionOptStatusContains: Sequence[RegionOptStatusType] = ...
+        RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,
     ) -> ListRegionsResponseTypeDef:
         """
         Lists all the Regions for a given account and their respective opt-in statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.list_regions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/client/#list_regions)
         """
@@ -182,15 +182,15 @@
         self,
         *,
         AlternateContactType: AlternateContactTypeType,
         EmailAddress: str,
         Name: str,
         PhoneNumber: str,
         Title: str,
-        AccountId: str = ...
+        AccountId: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Modifies the specified alternate contact attached to an Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Client.put_alternate_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/client/#put_alternate_contact)
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/literals.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlternateContactTypeType",
     "ListRegionsPaginatorName",
     "RegionOptStatusType",
     "AccountServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 AlternateContactTypeType = Literal["BILLING", "OPERATIONS", "SECURITY"]
 ListRegionsPaginatorName = Literal["list_regions"]
 RegionOptStatusType = Literal["DISABLED", "DISABLING", "ENABLED", "ENABLED_BY_DEFAULT", "ENABLING"]
 AccountServiceName = Literal["account"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/literals.pyi` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/paginator.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import RegionOptStatusType
 from .type_defs import ListRegionsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListRegionsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -49,13 +48,13 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str = ...,
         RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Paginator.ListRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/paginators/#listregionspaginator)
         """
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/paginator.pyi` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,13 +46,13 @@
     """
 
     def paginate(
         self,
         *,
         AccountId: str = ...,
         RegionOptStatusContains: Sequence[RegionOptStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account.Paginator.ListRegions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/paginators/#listregionspaginator)
         """
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/type_defs.py` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/type_defs.py`

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
     "AlternateContactTypeDef",
     "ContactInformationTypeDef",
     "DeleteAlternateContactRequestRequestTypeDef",
     "DisableRegionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EnableRegionRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account/type_defs.pyi` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/PKG-INFO` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Account 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Account 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
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
 
 <a id="types-aiobotocore-account"></a>
 
 # types-aiobotocore-account
 
 [![PyPI - types-aiobotocore-account](https://img.shields.io/pypi/v/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Account 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
+[aiobotocore.Account 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-account-2.9.0/types_aiobotocore_account.egg-info/SOURCES.txt` & `types-aiobotocore-account-2.9.1/types_aiobotocore_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*

