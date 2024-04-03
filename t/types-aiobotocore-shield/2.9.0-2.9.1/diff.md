# Comparing `tmp/types-aiobotocore-shield-2.9.0.tar.gz` & `tmp/types-aiobotocore-shield-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-shield-2.9.0.tar", last modified: Wed Dec 13 20:00:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-shield-2.9.1.tar", last modified: Thu Jan 18 01:21:50 2024, max compression
```

## Comparing `types-aiobotocore-shield-2.9.0.tar` & `types-aiobotocore-shield-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.753127 types-aiobotocore-shield-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2023-12-13 20:00:31.753127 types-aiobotocore-shield-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11486 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:31.753127 types-aiobotocore-shield-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.753127 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27583 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    27579 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20713 2023-12-13 19:56:33.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20712 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:56:32.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:31.753127 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13045 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 20:00:31.000000 types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.053029 types-aiobotocore-shield-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-01-18 01:21:50.053029 types-aiobotocore-shield-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11486 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:50.053029 types-aiobotocore-shield-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.049029 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27587 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27584 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9736 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20712 2024-01-18 01:18:01.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20712 2024-01-18 01:18:01.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:00.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:50.049029 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13065 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:50.000000 types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-shield-2.9.0/LICENSE` & `types-aiobotocore-shield-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-shield-2.9.0/PKG-INFO` & `types-aiobotocore-shield-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Shield 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Shield 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
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
 
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-shield-2.9.0/README.md` & `types-aiobotocore-shield-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-shield-2.9.0/setup.py` & `types-aiobotocore-shield-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-shield",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_shield"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Shield 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Shield 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore shield type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_shield": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__init__.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import ShieldClient
 from .paginator import ListAttacksPaginator, ListProtectionsPaginator
 
 Client = ShieldClient
 
-
 __all__ = ("Client", "ListAttacksPaginator", "ListProtectionsPaginator", "ShieldClient")
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__init__.pyi` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/__main__.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Shield 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Shield 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield\nOther"
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

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/client.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ShieldClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -176,15 +175,15 @@
         self,
         *,
         ProtectionGroupId: str,
         Aggregation: ProtectionGroupAggregationType,
         Pattern: ProtectionGroupPatternType,
         ResourceType: ProtectedResourceTypeType = ...,
         Members: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a grouping of protected resources so they can be handled as a
         collective.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.create_protection_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#create_protection_group)
@@ -392,44 +391,44 @@
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_attacks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_attacks)
         """
 
     async def list_protection_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        InclusionFilters: InclusionProtectionGroupFiltersTypeDef = ...
+        InclusionFilters: InclusionProtectionGroupFiltersTypeDef = ...,
     ) -> ListProtectionGroupsResponseTypeDef:
         """
         Retrieves  ProtectionGroup objects for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_protection_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_protection_groups)
         """
 
     async def list_protections(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        InclusionFilters: InclusionProtectionFiltersTypeDef = ...
+        InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
     ) -> ListProtectionsResponseTypeDef:
         """
         Retrieves  Protection objects for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_protections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_protections)
         """
@@ -501,15 +500,15 @@
     async def update_protection_group(
         self,
         *,
         ProtectionGroupId: str,
         Aggregation: ProtectionGroupAggregationType,
         Pattern: ProtectionGroupPatternType,
         ResourceType: ProtectedResourceTypeType = ...,
-        Members: Sequence[str] = ...
+        Members: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing protection group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_protection_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_protection_group)
         """
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/client.pyi` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         self,
         *,
         ProtectionGroupId: str,
         Aggregation: ProtectionGroupAggregationType,
         Pattern: ProtectionGroupPatternType,
         ResourceType: ProtectedResourceTypeType = ...,
         Members: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a grouping of protected resources so they can be handled as a
         collective.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.create_protection_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#create_protection_group)
@@ -388,44 +388,44 @@
     async def list_attacks(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangeTypeDef = ...,
         EndTime: TimeRangeTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAttacksResponseTypeDef:
         """
         Returns all ongoing DDoS attacks or all DDoS attacks during a specified time
         period.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_attacks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_attacks)
         """
 
     async def list_protection_groups(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        InclusionFilters: InclusionProtectionGroupFiltersTypeDef = ...
+        InclusionFilters: InclusionProtectionGroupFiltersTypeDef = ...,
     ) -> ListProtectionGroupsResponseTypeDef:
         """
         Retrieves  ProtectionGroup objects for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_protection_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_protection_groups)
         """
 
     async def list_protections(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
-        InclusionFilters: InclusionProtectionFiltersTypeDef = ...
+        InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
     ) -> ListProtectionsResponseTypeDef:
         """
         Retrieves  Protection objects for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.list_protections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#list_protections)
         """
@@ -497,15 +497,15 @@
     async def update_protection_group(
         self,
         *,
         ProtectionGroupId: str,
         Aggregation: ProtectionGroupAggregationType,
         Pattern: ProtectionGroupPatternType,
         ResourceType: ProtectedResourceTypeType = ...,
-        Members: Sequence[str] = ...
+        Members: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates an existing protection group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Client.update_protection_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/client/#update_protection_group)
         """
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/literals.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/literals.py`

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
     "ApplicationLayerAutomaticResponseStatusType",
     "AttackLayerType",
     "AttackPropertyIdentifierType",
     "AutoRenewType",
     "ListAttacksPaginatorName",
     "ListProtectionsPaginatorName",
@@ -36,15 +35,14 @@
     "UnitType",
     "ShieldServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ApplicationLayerAutomaticResponseStatusType = Literal["DISABLED", "ENABLED"]
 AttackLayerType = Literal["APPLICATION", "NETWORK"]
 AttackPropertyIdentifierType = Literal[
     "DESTINATION_URL",
     "REFERRER",
     "SOURCE_ASN",
     "SOURCE_COUNTRY",
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/literals.pyi` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/paginator.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,54 +34,50 @@
     ListProtectionsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimeRangePaginatorTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAttacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangePaginatorTypeDef = ...,
         EndTime: TimeRangePaginatorTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
 
-
 class ListProtectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/paginator.pyi` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,48 +36,51 @@
     TimeRangePaginatorTypeDef,
 )
 
 __all__ = ("ListAttacksPaginator", "ListProtectionsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAttacksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceArns: Sequence[str] = ...,
         StartTime: TimeRangePaginatorTypeDef = ...,
         EndTime: TimeRangePaginatorTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAttacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListAttacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listattackspaginator)
         """
 
+
 class ListProtectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
     """
 
     def paginate(
         self,
         *,
         InclusionFilters: InclusionProtectionFiltersTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield.Paginator.ListProtections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/paginators/#listprotectionspaginator)
         """
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/type_defs.py` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResponseActionTypeDef",
     "AssociateDRTLogBucketRequestRequestTypeDef",
     "AssociateDRTRoleRequestRequestTypeDef",
     "AssociateHealthCheckRequestRequestTypeDef",
     "EmergencyContactTypeDef",
     "MitigationTypeDef",
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield/type_defs.pyi` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/PKG-INFO` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-shield
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Shield 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Shield 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/
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
 
 <a id="types-aiobotocore-shield"></a>
 
 # types-aiobotocore-shield
 
 [![PyPI - types-aiobotocore-shield](https://img.shields.io/pypi/v/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-shield.svg?color=blue)](https://pypi.org/project/types-aiobotocore-shield)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-shield)](https://pepy.tech/project/types-aiobotocore-shield)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Shield 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
+[aiobotocore.Shield 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#Shield)
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
 [types-aiobotocore-shield docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_shield/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-shield-2.9.0/types_aiobotocore_shield.egg-info/SOURCES.txt` & `types-aiobotocore-shield-2.9.1/types_aiobotocore_shield.egg-info/SOURCES.txt`

 * *Files identical despite different names*

