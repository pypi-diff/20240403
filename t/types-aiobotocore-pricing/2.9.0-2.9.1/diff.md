# Comparing `tmp/types-aiobotocore-pricing-2.9.0.tar.gz` & `tmp/types-aiobotocore-pricing-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pricing-2.9.0.tar", last modified: Wed Dec 13 20:00:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-pricing-2.9.1.tar", last modified: Thu Jan 18 01:21:31 2024, max compression
```

## Comparing `types-aiobotocore-pricing-2.9.0.tar` & `types-aiobotocore-pricing-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.245305 types-aiobotocore-pricing-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2023-12-13 20:00:11.245305 types-aiobotocore-pricing-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11830 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:11.245305 types-aiobotocore-pricing-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.245305 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9500 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8772 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6397 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:55.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:11.245305 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13393 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:11.000000 types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.405112 types-aiobotocore-pricing-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-01-18 01:21:31.405112 types-aiobotocore-pricing-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11830 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:31.405112 types-aiobotocore-pricing-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.401112 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8772 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5684 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6397 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:32.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.401112 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13413 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:31.000000 types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pricing-2.9.0/LICENSE` & `types-aiobotocore-pricing-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-pricing-2.9.0/PKG-INFO` & `types-aiobotocore-pricing-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pricing
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Pricing 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Pricing 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/
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
 
 <a id="types-aiobotocore-pricing"></a>
 
 # types-aiobotocore-pricing
 
 [![PyPI - types-aiobotocore-pricing](https://img.shields.io/pypi/v/types-aiobotocore-pricing.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pricing.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pricing)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pricing)](https://pepy.tech/project/types-aiobotocore-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pricing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[aiobotocore.Pricing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [types-aiobotocore-pricing docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pricing-2.9.0/README.md` & `types-aiobotocore-pricing-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pricing.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pricing)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pricing)](https://pepy.tech/project/types-aiobotocore-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pricing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[aiobotocore.Pricing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [types-aiobotocore-pricing docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pricing-2.9.0/setup.py` & `types-aiobotocore-pricing-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pricing",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_pricing"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Pricing 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Pricing 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore pricing type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_pricing": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__init__.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     GetAttributeValuesPaginator,
     GetProductsPaginator,
     ListPriceListsPaginator,
 )
 
 Client = PricingClient
 
-
 __all__ = (
     "Client",
     "DescribeServicesPaginator",
     "GetAttributeValuesPaginator",
     "GetProductsPaginator",
     "ListPriceListsPaginator",
     "PricingClient",
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__init__.pyi` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/__main__.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Pricing 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Pricing 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing\nOther"
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

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/client.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PricingClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -99,15 +98,15 @@
 
     async def describe_services(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeServicesResponseTypeDef:
         """
         Returns the metadata for one service or a list of the metadata for all services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.describe_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#describe_services)
         """
@@ -149,15 +148,15 @@
     async def get_products(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProductsResponseTypeDef:
         """
         Returns a list of all products that match the filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.get_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#get_products)
         """
@@ -166,15 +165,15 @@
         self,
         *,
         ServiceCode: str,
         EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPriceListsResponseTypeDef:
         """
         This feature is in preview release and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.list_price_lists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#list_price_lists)
         """
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/client.pyi` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     async def describe_services(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeServicesResponseTypeDef:
         """
         Returns the metadata for one service or a list of the metadata for all services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.describe_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#describe_services)
         """
@@ -145,15 +145,15 @@
     async def get_products(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetProductsResponseTypeDef:
         """
         Returns a list of all products that match the filter criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.get_products)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#get_products)
         """
@@ -162,15 +162,15 @@
         self,
         *,
         ServiceCode: str,
         EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPriceListsResponseTypeDef:
         """
         This feature is in preview release and is subject to change.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Client.list_price_lists)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/client/#list_price_lists)
         """
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/literals.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/literals.py`

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
     "DescribeServicesPaginatorName",
     "FilterTypeType",
     "GetAttributeValuesPaginatorName",
     "GetProductsPaginatorName",
     "ListPriceListsPaginatorName",
     "PricingServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeServicesPaginatorName = Literal["describe_services"]
 FilterTypeType = Literal["TERM_MATCH"]
 GetAttributeValuesPaginatorName = Literal["get_attribute_values"]
 GetProductsPaginatorName = Literal["get_products"]
 ListPriceListsPaginatorName = Literal["list_price_lists"]
 PricingServiceName = Literal["pricing"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/literals.pyi` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/paginator.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 __all__ = (
     "DescribeServicesPaginator",
     "GetAttributeValuesPaginator",
     "GetProductsPaginator",
     "ListPriceListsPaginator",
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
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#describeservicespaginator)
         """
 
 
@@ -86,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#getattributevaluespaginator)
         """
 
 
@@ -106,15 +105,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#getproductspaginator)
         """
 
 
@@ -127,13 +126,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/paginator.pyi` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.DescribeServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#describeservicespaginator)
         """
 
 class GetAttributeValuesPaginator(AioPaginator):
@@ -82,15 +82,15 @@
     """
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         AttributeName: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetAttributeValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetAttributeValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#getattributevaluespaginator)
         """
 
 class GetProductsPaginator(AioPaginator):
@@ -101,15 +101,15 @@
 
     def paginate(
         self,
         *,
         ServiceCode: str,
         Filters: Sequence[FilterTypeDef] = ...,
         FormatVersion: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetProductsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.GetProducts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#getproductspaginator)
         """
 
 class ListPriceListsPaginator(AioPaginator):
@@ -121,13 +121,13 @@
     def paginate(
         self,
         *,
         ServiceCode: str,
         EffectiveDate: TimestampTypeDef,
         CurrencyCode: str,
         RegionCode: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPriceListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing.Paginator.ListPriceLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/paginators/#listpricelistspaginator)
         """
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/type_defs.py` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeValueTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeServicesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ServiceTypeDef",
     "FilterTypeDef",
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing/type_defs.pyi` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/PKG-INFO` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pricing
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Pricing 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Pricing 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/
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
 
 <a id="types-aiobotocore-pricing"></a>
 
 # types-aiobotocore-pricing
 
 [![PyPI - types-aiobotocore-pricing](https://img.shields.io/pypi/v/types-aiobotocore-pricing.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pricing)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pricing.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pricing)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-pricing)](https://pepy.tech/project/types-aiobotocore-pricing)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Pricing 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
+[aiobotocore.Pricing 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#Pricing)
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
 [types-aiobotocore-pricing docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pricing/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-pricing-2.9.0/types_aiobotocore_pricing.egg-info/SOURCES.txt` & `types-aiobotocore-pricing-2.9.1/types_aiobotocore_pricing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

