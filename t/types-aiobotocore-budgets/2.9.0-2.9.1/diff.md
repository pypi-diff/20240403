# Comparing `tmp/types-aiobotocore-budgets-2.9.0.tar.gz` & `tmp/types-aiobotocore-budgets-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-budgets-2.9.0.tar", last modified: Wed Dec 13 19:58:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-budgets-2.9.1.tar", last modified: Thu Jan 18 01:20:11 2024, max compression
```

## Comparing `types-aiobotocore-budgets-2.9.0.tar` & `types-aiobotocore-budgets-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.950017 types-aiobotocore-budgets-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14479 2023-12-13 19:58:43.950017 types-aiobotocore-budgets-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12916 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:43.950017 types-aiobotocore-budgets-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.946017 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23637 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23633 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11223 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11526 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    27131 2023-12-13 19:41:50.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27130 2023-12-13 19:41:50.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:49.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.950017 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14479 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:43.000000 types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.197485 types-aiobotocore-budgets-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-01-18 01:20:11.197485 types-aiobotocore-budgets-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12916 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:11.197485 types-aiobotocore-budgets-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.197485 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23647 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23644 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11223 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    27130 2024-01-18 01:03:48.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27130 2024-01-18 01:03:48.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:47.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:11.197485 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14499 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:11.000000 types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-budgets-2.9.0/LICENSE` & `types-aiobotocore-budgets-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-budgets-2.9.0/PKG-INFO` & `types-aiobotocore-budgets-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Budgets 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Budgets 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
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
 
 <a id="types-aiobotocore-budgets"></a>
 
 # types-aiobotocore-budgets
 
 [![PyPI - types-aiobotocore-budgets](https://img.shields.io/pypi/v/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-budgets-2.9.0/README.md` & `types-aiobotocore-budgets-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-budgets-2.9.0/setup.py` & `types-aiobotocore-budgets-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-budgets",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_budgets"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Budgets 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Budgets 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore budgets type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_budgets": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__init__.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     DescribeBudgetsPaginator,
     DescribeNotificationsForBudgetPaginator,
     DescribeSubscribersForNotificationPaginator,
 )
 
 Client = BudgetsClient
 
-
 __all__ = (
     "BudgetsClient",
     "Client",
     "DescribeBudgetActionHistoriesPaginator",
     "DescribeBudgetActionsForAccountPaginator",
     "DescribeBudgetActionsForBudgetPaginator",
     "DescribeBudgetNotificationsForAccountPaginator",
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__init__.pyi` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/__main__.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Budgets 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Budgets 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets\nOther"
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

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/client.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BudgetsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -121,15 +120,15 @@
         """
 
     async def create_budget(
         self,
         *,
         AccountId: str,
         Budget: BudgetTypeDef,
-        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
+        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
         """
@@ -141,45 +140,45 @@
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
         Definition: DefinitionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget_action)
         """
 
     async def create_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> Dict[str, Any]:
         """
         Creates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_notification)
         """
 
     async def create_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_subscriber)
         """
@@ -214,15 +213,15 @@
 
     async def delete_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#delete_subscriber)
         """
@@ -251,15 +250,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_action_histories)
         """
@@ -297,15 +296,15 @@
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_performance_history)
         """
@@ -333,15 +332,15 @@
     async def describe_subscribers_for_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSubscribersForNotificationResponseTypeDef:
         """
         Lists the subscribers that are associated with a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_subscribers_for_notification)
         """
@@ -385,30 +384,30 @@
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
         Definition: DefinitionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
-        Subscribers: Sequence[SubscriberTypeDef] = ...
+        Subscribers: Sequence[SubscriberTypeDef] = ...,
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget_action)
         """
 
     async def update_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         OldNotification: NotificationTypeDef,
-        NewNotification: NotificationTypeDef
+        NewNotification: NotificationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_notification)
         """
@@ -416,15 +415,15 @@
     async def update_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         OldSubscriber: SubscriberTypeDef,
-        NewSubscriber: SubscriberTypeDef
+        NewSubscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_subscriber)
         """
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/client.pyi` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
         """
 
     async def create_budget(
         self,
         *,
         AccountId: str,
         Budget: BudgetTypeDef,
-        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...
+        NotificationsWithSubscribers: Sequence[NotificationWithSubscribersTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a budget and, if included, notifications and subscribers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget)
         """
@@ -137,45 +137,45 @@
         BudgetName: str,
         NotificationType: NotificationTypeType,
         ActionType: ActionTypeType,
         ActionThreshold: ActionThresholdTypeDef,
         Definition: DefinitionTypeDef,
         ExecutionRoleArn: str,
         ApprovalModel: ApprovalModelType,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> CreateBudgetActionResponseTypeDef:
         """
         Creates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_budget_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_budget_action)
         """
 
     async def create_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscribers: Sequence[SubscriberTypeDef]
+        Subscribers: Sequence[SubscriberTypeDef],
     ) -> Dict[str, Any]:
         """
         Creates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_notification)
         """
 
     async def create_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Creates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.create_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#create_subscriber)
         """
@@ -210,15 +210,15 @@
 
     async def delete_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        Subscriber: SubscriberTypeDef
+        Subscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.delete_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#delete_subscriber)
         """
@@ -247,15 +247,15 @@
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetActionHistoriesResponseTypeDef:
         """
         Describes a budget action history detail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_action_histories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_action_histories)
         """
@@ -293,15 +293,15 @@
     async def describe_budget_performance_history(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeBudgetPerformanceHistoryResponseTypeDef:
         """
         Describes the history for `DAILY`, `MONTHLY`, and `QUARTERLY` budgets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_budget_performance_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_budget_performance_history)
         """
@@ -329,15 +329,15 @@
     async def describe_subscribers_for_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeSubscribersForNotificationResponseTypeDef:
         """
         Lists the subscribers that are associated with a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.describe_subscribers_for_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#describe_subscribers_for_notification)
         """
@@ -381,30 +381,30 @@
         BudgetName: str,
         ActionId: str,
         NotificationType: NotificationTypeType = ...,
         ActionThreshold: ActionThresholdTypeDef = ...,
         Definition: DefinitionTypeDef = ...,
         ExecutionRoleArn: str = ...,
         ApprovalModel: ApprovalModelType = ...,
-        Subscribers: Sequence[SubscriberTypeDef] = ...
+        Subscribers: Sequence[SubscriberTypeDef] = ...,
     ) -> UpdateBudgetActionResponseTypeDef:
         """
         Updates a budget action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_budget_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_budget_action)
         """
 
     async def update_notification(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         OldNotification: NotificationTypeDef,
-        NewNotification: NotificationTypeDef
+        NewNotification: NotificationTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a notification.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_notification)
         """
@@ -412,15 +412,15 @@
     async def update_subscriber(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
         OldSubscriber: SubscriberTypeDef,
-        NewSubscriber: SubscriberTypeDef
+        NewSubscriber: SubscriberTypeDef,
     ) -> Dict[str, Any]:
         """
         Updates a subscriber.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Client.update_subscriber)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/client/#update_subscriber)
         """
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/literals.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/literals.py`

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
     "ActionStatusType",
     "ActionSubTypeType",
     "ActionTypeType",
     "ApprovalModelType",
     "AutoAdjustTypeType",
     "BudgetTypeType",
@@ -45,15 +44,14 @@
     "TimeUnitType",
     "BudgetsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ActionStatusType = Literal[
     "EXECUTION_FAILURE",
     "EXECUTION_IN_PROGRESS",
     "EXECUTION_SUCCESS",
     "PENDING",
     "RESET_FAILURE",
     "RESET_IN_PROGRESS",
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/literals.pyi` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/paginator.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     "DescribeBudgetNotificationsForAccountPaginator",
     "DescribeBudgetPerformanceHistoryPaginator",
     "DescribeBudgetsPaginator",
     "DescribeNotificationsForBudgetPaginator",
     "DescribeSubscribersForNotificationPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -85,15 +84,15 @@
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 
@@ -150,15 +149,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 
@@ -200,13 +199,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/paginator.pyi` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         ActionId: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBudgetActionHistoriesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetActionHistories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetactionhistoriespaginator)
         """
 
 class DescribeBudgetActionsForAccountPaginator(AioPaginator):
@@ -143,15 +143,15 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         TimePeriod: TimePeriodTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBudgetPerformanceHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeBudgetPerformanceHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describebudgetperformancehistorypaginator)
         """
 
 class DescribeBudgetsPaginator(AioPaginator):
@@ -190,13 +190,13 @@
 
     def paginate(
         self,
         *,
         AccountId: str,
         BudgetName: str,
         Notification: NotificationTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeSubscribersForNotificationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets.Paginator.DescribeSubscribersForNotification.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/paginators/#describesubscribersfornotificationpaginator)
         """
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/type_defs.py` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionThresholdTypeDef",
     "SubscriberTypeDef",
     "HistoricalOptionsTypeDef",
     "TimestampTypeDef",
     "NotificationTypeDef",
     "CostTypesTypeDef",
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets/type_defs.pyi` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/PKG-INFO` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-budgets
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Budgets 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Budgets 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/
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
 
 <a id="types-aiobotocore-budgets"></a>
 
 # types-aiobotocore-budgets
 
 [![PyPI - types-aiobotocore-budgets](https://img.shields.io/pypi/v/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-budgets.svg?color=blue)](https://pypi.org/project/types-aiobotocore-budgets)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-budgets)](https://pepy.tech/project/types-aiobotocore-budgets)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Budgets 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
+[aiobotocore.Budgets 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#Budgets)
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
 [types-aiobotocore-budgets docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_budgets/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-budgets-2.9.0/types_aiobotocore_budgets.egg-info/SOURCES.txt` & `types-aiobotocore-budgets-2.9.1/types_aiobotocore_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

