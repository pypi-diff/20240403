# Comparing `tmp/types-aiobotocore-savingsplans-2.9.0.tar.gz` & `tmp/types-aiobotocore-savingsplans-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-savingsplans-2.9.0.tar", last modified: Wed Dec 13 20:00:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-savingsplans-2.9.1.tar", last modified: Thu Jan 18 01:21:45 2024, max compression
```

## Comparing `types-aiobotocore-savingsplans-2.9.0.tar` & `types-aiobotocore-savingsplans-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.473172 types-aiobotocore-savingsplans-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2023-12-13 20:00:26.473172 types-aiobotocore-savingsplans-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:26.473172 types-aiobotocore-savingsplans-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.473172 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9957 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9955 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11962 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    11961 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:48.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:26.473172 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12480 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 20:00:26.000000 types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.249051 types-aiobotocore-savingsplans-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-01-18 01:21:45.249051 types-aiobotocore-savingsplans-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:45.249051 types-aiobotocore-savingsplans-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.245051 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11361 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11961 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:19.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.245051 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:45.000000 types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/LICENSE` & `types-aiobotocore-savingsplans-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-savingsplans-2.9.0/PKG-INFO` & `types-aiobotocore-savingsplans-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-savingsplans
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SavingsPlans 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SavingsPlans 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/
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
 
 <a id="types-aiobotocore-savingsplans"></a>
 
 # types-aiobotocore-savingsplans
 
 [![PyPI - types-aiobotocore-savingsplans](https://img.shields.io/pypi/v/types-aiobotocore-savingsplans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-savingsplans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-savingsplans)](https://pepy.tech/project/types-aiobotocore-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SavingsPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[aiobotocore.SavingsPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/README.md` & `types-aiobotocore-savingsplans-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-savingsplans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-savingsplans)](https://pepy.tech/project/types-aiobotocore-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SavingsPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[aiobotocore.SavingsPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/setup.py` & `types-aiobotocore-savingsplans-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-savingsplans",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_savingsplans"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SavingsPlans 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.SavingsPlans 2.9.1 service generated with"
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
     keywords="aiobotocore savingsplans type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_savingsplans": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/__main__.py` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SavingsPlans 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SavingsPlans 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans\nOther"
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

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/client.py` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self,
         *,
         savingsPlanOfferingId: str,
         commitment: str,
         upfrontPaymentAmount: str = ...,
         purchaseTime: TimestampTypeDef = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSavingsPlanResponseTypeDef:
         """
         Creates a Savings Plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.create_savings_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#create_savings_plan)
         """
@@ -121,15 +121,15 @@
 
     async def describe_savings_plan_rates(
         self,
         *,
         savingsPlanId: str,
         filters: Sequence[SavingsPlanRateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlanRatesResponseTypeDef:
         """
         Describes the specified Savings Plans rates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plan_rates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plan_rates)
         """
@@ -138,15 +138,15 @@
         self,
         *,
         savingsPlanArns: Sequence[str] = ...,
         savingsPlanIds: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         states: Sequence[SavingsPlanStateType] = ...,
-        filters: Sequence[SavingsPlanFilterTypeDef] = ...
+        filters: Sequence[SavingsPlanFilterTypeDef] = ...,
     ) -> DescribeSavingsPlansResponseTypeDef:
         """
         Describes the specified Savings Plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans)
         """
@@ -159,15 +159,15 @@
         savingsPlanTypes: Sequence[SavingsPlanTypeType] = ...,
         products: Sequence[SavingsPlanProductTypeType] = ...,
         serviceCodes: Sequence[SavingsPlanRateServiceCodeType] = ...,
         usageTypes: Sequence[str] = ...,
         operations: Sequence[str] = ...,
         filters: Sequence[SavingsPlanOfferingRateFilterElementTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlansOfferingRatesResponseTypeDef:
         """
         Describes the specified Savings Plans offering rates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offering_rates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans_offering_rates)
         """
@@ -183,15 +183,15 @@
         currencies: Sequence[CurrencyCodeType] = ...,
         descriptions: Sequence[str] = ...,
         serviceCodes: Sequence[str] = ...,
         usageTypes: Sequence[str] = ...,
         operations: Sequence[str] = ...,
         filters: Sequence[SavingsPlanOfferingFilterElementTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlansOfferingsResponseTypeDef:
         """
         Describes the specified Savings Plans offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans_offerings)
         """
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/client.pyi` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self,
         *,
         savingsPlanOfferingId: str,
         commitment: str,
         upfrontPaymentAmount: str = ...,
         purchaseTime: TimestampTypeDef = ...,
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSavingsPlanResponseTypeDef:
         """
         Creates a Savings Plan.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.create_savings_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#create_savings_plan)
         """
@@ -118,15 +118,15 @@
 
     async def describe_savings_plan_rates(
         self,
         *,
         savingsPlanId: str,
         filters: Sequence[SavingsPlanRateFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlanRatesResponseTypeDef:
         """
         Describes the specified Savings Plans rates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plan_rates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plan_rates)
         """
@@ -135,15 +135,15 @@
         self,
         *,
         savingsPlanArns: Sequence[str] = ...,
         savingsPlanIds: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         states: Sequence[SavingsPlanStateType] = ...,
-        filters: Sequence[SavingsPlanFilterTypeDef] = ...
+        filters: Sequence[SavingsPlanFilterTypeDef] = ...,
     ) -> DescribeSavingsPlansResponseTypeDef:
         """
         Describes the specified Savings Plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans)
         """
@@ -156,15 +156,15 @@
         savingsPlanTypes: Sequence[SavingsPlanTypeType] = ...,
         products: Sequence[SavingsPlanProductTypeType] = ...,
         serviceCodes: Sequence[SavingsPlanRateServiceCodeType] = ...,
         usageTypes: Sequence[str] = ...,
         operations: Sequence[str] = ...,
         filters: Sequence[SavingsPlanOfferingRateFilterElementTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlansOfferingRatesResponseTypeDef:
         """
         Describes the specified Savings Plans offering rates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offering_rates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans_offering_rates)
         """
@@ -180,15 +180,15 @@
         currencies: Sequence[CurrencyCodeType] = ...,
         descriptions: Sequence[str] = ...,
         serviceCodes: Sequence[str] = ...,
         usageTypes: Sequence[str] = ...,
         operations: Sequence[str] = ...,
         filters: Sequence[SavingsPlanOfferingFilterElementTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeSavingsPlansOfferingsResponseTypeDef:
         """
         Describes the specified Savings Plans offerings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans.Client.describe_savings_plans_offerings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/client/#describe_savings_plans_offerings)
         """
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/literals.py` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/literals.py`

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
     "CurrencyCodeType",
     "SavingsPlanOfferingFilterAttributeType",
     "SavingsPlanOfferingPropertyKeyType",
     "SavingsPlanPaymentOptionType",
     "SavingsPlanProductTypeType",
     "SavingsPlanRateFilterAttributeType",
@@ -35,15 +34,14 @@
     "SavingsPlanTypeType",
     "SavingsPlansFilterNameType",
     "SavingsPlansServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 CurrencyCodeType = Literal["CNY", "USD"]
 SavingsPlanOfferingFilterAttributeType = Literal["instanceFamily", "region"]
 SavingsPlanOfferingPropertyKeyType = Literal["instanceFamily", "region"]
 SavingsPlanPaymentOptionType = Literal["All Upfront", "No Upfront", "Partial Upfront"]
 SavingsPlanProductTypeType = Literal["EC2", "Fargate", "Lambda", "SageMaker"]
 SavingsPlanRateFilterAttributeType = Literal[
     "instanceFamily", "instanceType", "productDescription", "productId", "region", "tenancy"
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/literals.pyi` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/type_defs.py` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TimestampTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteQueuedSavingsPlanRequestRequestTypeDef",
     "SavingsPlanRateFilterTypeDef",
     "SavingsPlanOfferingRateFilterElementTypeDef",
     "SavingsPlanOfferingFilterElementTypeDef",
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans/type_defs.pyi` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/PKG-INFO` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-savingsplans
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SavingsPlans 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SavingsPlans 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/
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
 
 <a id="types-aiobotocore-savingsplans"></a>
 
 # types-aiobotocore-savingsplans
 
 [![PyPI - types-aiobotocore-savingsplans](https://img.shields.io/pypi/v/types-aiobotocore-savingsplans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-savingsplans)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-savingsplans.svg?color=blue)](https://pypi.org/project/types-aiobotocore-savingsplans)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-savingsplans)](https://pepy.tech/project/types-aiobotocore-savingsplans)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SavingsPlans 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
+[aiobotocore.SavingsPlans 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#SavingsPlans)
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
 [types-aiobotocore-savingsplans docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_savingsplans/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-savingsplans-2.9.0/types_aiobotocore_savingsplans.egg-info/SOURCES.txt` & `types-aiobotocore-savingsplans-2.9.1/types_aiobotocore_savingsplans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

