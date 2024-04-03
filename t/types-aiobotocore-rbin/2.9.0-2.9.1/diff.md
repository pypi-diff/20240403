# Comparing `tmp/types-aiobotocore-rbin-2.9.0.tar.gz` & `tmp/types-aiobotocore-rbin-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rbin-2.9.0.tar", last modified: Wed Dec 13 20:00:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-rbin-2.9.1.tar", last modified: Thu Jan 18 01:21:34 2024, max compression
```

## Comparing `types-aiobotocore-rbin-2.9.0.tar` & `types-aiobotocore-rbin-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.693275 types-aiobotocore-rbin-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2023-12-13 20:00:14.693275 types-aiobotocore-rbin-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11252 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:14.693275 types-aiobotocore-rbin-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.693275 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      921 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10321 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9176 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8521 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8520 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:03.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.693275 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 20:00:14.000000 types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.541098 types-aiobotocore-rbin-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-01-18 01:21:34.541098 types-aiobotocore-rbin-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11252 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:34.541098 types-aiobotocore-rbin-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.537098 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10320 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9176 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-01-18 01:15:39.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-01-18 01:15:39.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:38.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.537098 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 01:21:34.000000 types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rbin-2.9.0/LICENSE` & `types-aiobotocore-rbin-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rbin-2.9.0/PKG-INFO` & `types-aiobotocore-rbin-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rbin
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RecycleBin 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RecycleBin 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
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
 
 <a id="types-aiobotocore-rbin"></a>
 
 # types-aiobotocore-rbin
 
 [![PyPI - types-aiobotocore-rbin](https://img.shields.io/pypi/v/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [types-aiobotocore-rbin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rbin-2.9.0/README.md` & `types-aiobotocore-rbin-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [types-aiobotocore-rbin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rbin-2.9.0/setup.py` & `types-aiobotocore-rbin-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rbin",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rbin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RecycleBin 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.RecycleBin 2.9.1 service generated with"
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
     keywords="aiobotocore rbin type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rbin": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__init__.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import RecycleBinClient
 from .paginator import ListRulesPaginator
 
 Client = RecycleBinClient
 
-
 __all__ = ("Client", "ListRulesPaginator", "RecycleBinClient")
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__init__.pyi` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/__main__.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RecycleBin 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RecycleBin 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin\nOther"
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

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/client.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -38,35 +38,31 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RecycleBinClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class RecycleBinClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/)
     """
 
     meta: ClientMeta
@@ -100,15 +96,15 @@
         self,
         *,
         RetentionPeriod: RetentionPeriodTypeDef,
         ResourceType: ResourceTypeType,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
-        LockConfiguration: LockConfigurationTypeDef = ...
+        LockConfiguration: LockConfigurationTypeDef = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a Recycle Bin retention rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#create_rule)
         """
@@ -146,15 +142,15 @@
     async def list_rules(
         self,
         *,
         ResourceType: ResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
-        LockState: LockStateType = ...
+        LockState: LockStateType = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the Recycle Bin retention rules in the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#list_rules)
         """
@@ -206,15 +202,15 @@
     async def update_rule(
         self,
         *,
         Identifier: str,
         RetentionPeriod: RetentionPeriodTypeDef = ...,
         Description: str = ...,
         ResourceType: ResourceTypeType = ...,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates an existing Recycle Bin retention rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#update_rule)
         """
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/client.pyi` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,32 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("RecycleBinClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class RecycleBinClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/)
     """
 
     meta: ClientMeta
@@ -96,15 +99,15 @@
         self,
         *,
         RetentionPeriod: RetentionPeriodTypeDef,
         ResourceType: ResourceTypeType,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
-        LockConfiguration: LockConfigurationTypeDef = ...
+        LockConfiguration: LockConfigurationTypeDef = ...,
     ) -> CreateRuleResponseTypeDef:
         """
         Creates a Recycle Bin retention rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.create_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#create_rule)
         """
@@ -142,15 +145,15 @@
     async def list_rules(
         self,
         *,
         ResourceType: ResourceTypeType,
         MaxResults: int = ...,
         NextToken: str = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
-        LockState: LockStateType = ...
+        LockState: LockStateType = ...,
     ) -> ListRulesResponseTypeDef:
         """
         Lists the Recycle Bin retention rules in the Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.list_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#list_rules)
         """
@@ -202,15 +205,15 @@
     async def update_rule(
         self,
         *,
         Identifier: str,
         RetentionPeriod: RetentionPeriodTypeDef = ...,
         Description: str = ...,
         ResourceType: ResourceTypeType = ...,
-        ResourceTags: Sequence[ResourceTagTypeDef] = ...
+        ResourceTags: Sequence[ResourceTagTypeDef] = ...,
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates an existing Recycle Bin retention rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/client/#update_rule)
         """
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/literals.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,30 +15,28 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListRulesPaginatorName",
     "LockStateType",
     "ResourceTypeType",
     "RetentionPeriodUnitType",
     "RuleStatusType",
     "UnlockDelayUnitType",
     "RecycleBinServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListRulesPaginatorName = Literal["list_rules"]
 LockStateType = Literal["locked", "pending_unlock", "unlocked"]
 ResourceTypeType = Literal["EBS_SNAPSHOT", "EC2_IMAGE"]
 RetentionPeriodUnitType = Literal["DAYS"]
 RuleStatusType = Literal["available", "pending"]
 UnlockDelayUnitType = Literal["DAYS"]
 RecycleBinServiceName = Literal["rbin"]
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/literals.pyi` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/paginator.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import LockStateType, ResourceTypeType
 from .type_defs import ListRulesResponseTypeDef, PaginatorConfigTypeDef, ResourceTagTypeDef
 
 __all__ = ("ListRulesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -50,13 +49,13 @@
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/paginator.pyi` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
     def paginate(
         self,
         *,
         ResourceType: ResourceTypeType,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...,
         LockState: LockStateType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/paginators/#listrulespaginator)
         """
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/type_defs.py` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ResourceTagTypeDef",
     "RetentionPeriodTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "GetRuleRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin/type_defs.pyi` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/PKG-INFO` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rbin
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RecycleBin 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RecycleBin 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/
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
 
 <a id="types-aiobotocore-rbin"></a>
 
 # types-aiobotocore-rbin
 
 [![PyPI - types-aiobotocore-rbin](https://img.shields.io/pypi/v/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rbin.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rbin)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rbin)](https://pepy.tech/project/types-aiobotocore-rbin)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RecycleBin 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
+[aiobotocore.RecycleBin 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#RecycleBin)
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
 [types-aiobotocore-rbin docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rbin/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rbin-2.9.0/types_aiobotocore_rbin.egg-info/SOURCES.txt` & `types-aiobotocore-rbin-2.9.1/types_aiobotocore_rbin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

