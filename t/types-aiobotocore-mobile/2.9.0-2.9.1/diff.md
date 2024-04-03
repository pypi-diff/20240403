# Comparing `tmp/types-aiobotocore-mobile-2.9.0.tar.gz` & `tmp/types-aiobotocore-mobile-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mobile-2.9.0.tar", last modified: Wed Dec 13 19:59:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-mobile-2.9.1.tar", last modified: Thu Jan 18 01:21:20 2024, max compression
```

## Comparing `types-aiobotocore-mobile-2.9.0.tar` & `types-aiobotocore-mobile-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.089410 types-aiobotocore-mobile-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12975 2023-12-13 19:59:59.089410 types-aiobotocore-mobile-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:59.089410 types-aiobotocore-mobile-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:50:38.000000 types-aiobotocore-mobile-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.089410 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10210 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:50:39.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:59.089410 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12975 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:59.000000 types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.473162 types-aiobotocore-mobile-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-01-18 01:21:20.473162 types-aiobotocore-mobile-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:20.473162 types-aiobotocore-mobile-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.473162 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-01-18 01:12:21.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-01-18 01:12:21.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-01-18 01:12:21.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:20.473162 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12995 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:20.000000 types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mobile-2.9.0/LICENSE` & `types-aiobotocore-mobile-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mobile-2.9.0/PKG-INFO` & `types-aiobotocore-mobile-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Mobile 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Mobile 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
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
 
 <a id="types-aiobotocore-mobile"></a>
 
 # types-aiobotocore-mobile
 
 [![PyPI - types-aiobotocore-mobile](https://img.shields.io/pypi/v/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mobile-2.9.0/README.md` & `types-aiobotocore-mobile-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mobile-2.9.0/setup.py` & `types-aiobotocore-mobile-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mobile",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mobile"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Mobile 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Mobile 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore mobile type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mobile": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__init__.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import MobileClient
 from .paginator import ListBundlesPaginator, ListProjectsPaginator
 
 Client = MobileClient
 
-
 __all__ = ("Client", "ListBundlesPaginator", "ListProjectsPaginator", "MobileClient")
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__init__.pyi` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/__main__.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Mobile 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Mobile 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile\nOther"
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

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/client.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MobileClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -100,15 +99,15 @@
 
     async def create_project(
         self,
         *,
         name: str = ...,
         region: str = ...,
         contents: BlobTypeDef = ...,
-        snapshotId: str = ...
+        snapshotId: str = ...,
     ) -> CreateProjectResultTypeDef:
         """
         Creates an AWS Mobile Hub project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/client/#create_project)
         """
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/client.pyi` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     async def create_project(
         self,
         *,
         name: str = ...,
         region: str = ...,
         contents: BlobTypeDef = ...,
-        snapshotId: str = ...
+        snapshotId: str = ...,
     ) -> CreateProjectResultTypeDef:
         """
         Creates an AWS Mobile Hub project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/client/#create_project)
         """
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/literals.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListBundlesPaginatorName",
     "ListProjectsPaginatorName",
     "PlatformType",
     "ProjectStateType",
     "MobileServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
 )
 
-
 ListBundlesPaginatorName = Literal["list_bundles"]
 ListProjectsPaginatorName = Literal["list_projects"]
 PlatformType = Literal["ANDROID", "JAVASCRIPT", "LINUX", "OBJC", "OSX", "SWIFT", "WINDOWS"]
 ProjectStateType = Literal["IMPORTING", "NORMAL", "SYNCING"]
 MobileServiceName = Literal["mobile"]
 ServiceName = Literal[
     "accessanalyzer",
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/literals.pyi` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/paginator.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListBundlesResultTypeDef, ListProjectsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListBundlesPaginator", "ListProjectsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/paginator.pyi` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/type_defs.py` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/type_defs.py`

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
     "BlobTypeDef",
     "BundleDetailsTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "ResourceTypeDef",
     "DescribeBundleRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile/type_defs.pyi` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/PKG-INFO` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mobile
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Mobile 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Mobile 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/
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
 
 <a id="types-aiobotocore-mobile"></a>
 
 # types-aiobotocore-mobile
 
 [![PyPI - types-aiobotocore-mobile](https://img.shields.io/pypi/v/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mobile.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mobile)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mobile)](https://pepy.tech/project/types-aiobotocore-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Mobile 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[aiobotocore.Mobile 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [types-aiobotocore-mobile docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mobile/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mobile-2.9.0/types_aiobotocore_mobile.egg-info/SOURCES.txt` & `types-aiobotocore-mobile-2.9.1/types_aiobotocore_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

