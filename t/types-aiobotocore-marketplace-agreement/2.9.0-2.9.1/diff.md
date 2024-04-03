# Comparing `tmp/types-aiobotocore-marketplace-agreement-2.9.0.tar.gz` & `tmp/types-aiobotocore-marketplace-agreement-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-agreement-2.9.0.tar", last modified: Wed Dec 13 19:59:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-agreement-2.9.1.tar", last modified: Thu Jan 18 01:21:12 2024, max compression
```

## Comparing `types-aiobotocore-marketplace-agreement-2.9.0.tar` & `types-aiobotocore-marketplace-agreement-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.477487 types-aiobotocore-marketplace-agreement-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12930 2023-12-13 19:59:50.477487 types-aiobotocore-marketplace-agreement-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:50.477487 types-aiobotocore-marketplace-agreement-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.477487 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6549 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8495 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10527 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10526 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.477487 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12930 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.593198 types-aiobotocore-marketplace-agreement-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-01-18 01:21:12.593198 types-aiobotocore-marketplace-agreement-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:12.593198 types-aiobotocore-marketplace-agreement-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.589198 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6550 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10526 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:29.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.589198 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/LICENSE` & `types-aiobotocore-marketplace-agreement-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/PKG-INFO` & `types-aiobotocore-marketplace-agreement-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-agreement
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AgreementService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AgreementService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/
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
 
 <a id="types-aiobotocore-marketplace-agreement"></a>
 
 # types-aiobotocore-marketplace-agreement
 
 [![PyPI - types-aiobotocore-marketplace-agreement](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-agreement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-agreement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-agreement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-agreement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-agreement)](https://pepy.tech/project/types-aiobotocore-marketplace-agreement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgreementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
+[aiobotocore.AgreementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
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
 [types-aiobotocore-marketplace-agreement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/README.md` & `types-aiobotocore-marketplace-agreement-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-agreement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-agreement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-agreement)](https://pepy.tech/project/types-aiobotocore-marketplace-agreement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgreementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
+[aiobotocore.AgreementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
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
 [types-aiobotocore-marketplace-agreement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/setup.py` & `types-aiobotocore-marketplace-agreement-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-agreement",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_marketplace_agreement"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AgreementService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.AgreementService 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore marketplace-agreement type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_marketplace_agreement": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__init__.py` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import AgreementServiceClient
 
 Client = AgreementServiceClient
 
-
 __all__ = ("AgreementServiceClient", "Client")
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__init__.pyi` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/__main__.py` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AgreementService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AgreementService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService\nOther"
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

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/client.py` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     async def search_agreements(
         self,
         *,
         catalog: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sort: SortTypeDef = ...
+        sort: SortTypeDef = ...,
     ) -> SearchAgreementsOutputTypeDef:
         """
         Searches across all agreements that a proposer or an acceptor has in AWS
         Marketplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.search_agreements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/client/#search_agreements)
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/client.pyi` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     async def search_agreements(
         self,
         *,
         catalog: str = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sort: SortTypeDef = ...
+        sort: SortTypeDef = ...,
     ) -> SearchAgreementsOutputTypeDef:
         """
         Searches across all agreements that a proposer or an acceptor has in AWS
         Marketplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService.Client.search_agreements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/client/#search_agreements)
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/literals.py` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/literals.py`

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
     "AgreementStatusType",
     "SortOrderType",
     "AgreementServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AgreementStatusType = Literal[
     "ACTIVE",
     "ARCHIVED",
     "CANCELLED",
     "EXPIRED",
     "RENEWED",
     "REPLACED",
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/literals.pyi` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/type_defs.py` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ByolPricingTermTypeDef",
     "RecurringPaymentTermTypeDef",
     "SupportTermTypeDef",
     "ValidityTermTypeDef",
     "AcceptorTypeDef",
     "ProposerTypeDef",
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement/type_defs.pyi` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-agreement
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AgreementService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AgreementService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/
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
 
 <a id="types-aiobotocore-marketplace-agreement"></a>
 
 # types-aiobotocore-marketplace-agreement
 
 [![PyPI - types-aiobotocore-marketplace-agreement](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-agreement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-agreement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-agreement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-agreement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-agreement)](https://pepy.tech/project/types-aiobotocore-marketplace-agreement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AgreementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
+[aiobotocore.AgreementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#AgreementService)
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
 [types-aiobotocore-marketplace-agreement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_agreement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-agreement-2.9.0/types_aiobotocore_marketplace_agreement.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-agreement-2.9.1/types_aiobotocore_marketplace_agreement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

