# Comparing `tmp/types-aiobotocore-ram-2.9.0.tar.gz` & `tmp/types-aiobotocore-ram-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ram-2.9.0.tar", last modified: Wed Dec 13 20:00:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ram-2.9.1.tar", last modified: Thu Jan 18 01:21:34 2024, max compression
```

## Comparing `types-aiobotocore-ram-2.9.0.tar` & `types-aiobotocore-ram-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.313278 types-aiobotocore-ram-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2023-12-13 20:00:14.313278 types-aiobotocore-ram-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12088 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:14.313278 types-aiobotocore-ram-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.313278 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33855 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    33851 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11225 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9026 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9018 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31846 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31845 2023-12-13 19:54:02.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:01.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:14.313278 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13635 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 20:00:14.000000 types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.197099 types-aiobotocore-ram-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-01-18 01:21:34.197099 types-aiobotocore-ram-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12088 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:34.197099 types-aiobotocore-ram-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.193099 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33872 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33869 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-01-18 01:15:38.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31845 2024-01-18 01:15:38.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:15:37.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:34.197099 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13655 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:21:34.000000 types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ram-2.9.0/LICENSE` & `types-aiobotocore-ram-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ram-2.9.0/PKG-INFO` & `types-aiobotocore-ram-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ram
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RAM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RAM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/
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
 
 <a id="types-aiobotocore-ram"></a>
 
 # types-aiobotocore-ram
 
 [![PyPI - types-aiobotocore-ram](https://img.shields.io/pypi/v/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [types-aiobotocore-ram docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ram-2.9.0/README.md` & `types-aiobotocore-ram-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [types-aiobotocore-ram docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ram-2.9.0/setup.py` & `types-aiobotocore-ram-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ram",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ram"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.RAM 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.RAM 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ram type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ram": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__init__.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     GetResourceSharesPaginator,
     ListPrincipalsPaginator,
     ListResourcesPaginator,
 )
 
 Client = RAMClient
 
-
 __all__ = (
     "Client",
     "GetResourcePoliciesPaginator",
     "GetResourceShareAssociationsPaginator",
     "GetResourceShareInvitationsPaginator",
     "GetResourceSharesPaginator",
     "ListPrincipalsPaginator",
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__init__.pyi` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/__main__.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.RAM 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.RAM 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM\nOther"
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

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/client.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RAMClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -156,15 +155,15 @@
     async def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share)
         """
@@ -172,15 +171,15 @@
     async def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
-        permissionVersion: int = ...
+        permissionVersion: int = ...,
     ) -> AssociateResourceSharePermissionResponseTypeDef:
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share_permission)
@@ -205,15 +204,15 @@
     async def create_permission(
         self,
         *,
         name: str,
         resourceType: str,
         policyTemplate: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePermissionResponseTypeDef:
         """
         Creates a customer managed permission for a specified resource type that you
         can attach to resource
         shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
@@ -236,15 +235,15 @@
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
         permissionArns: Sequence[str] = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_resource_share)
         """
@@ -284,15 +283,15 @@
     async def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
@@ -345,15 +344,15 @@
 
     async def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Retrieves the resource policies for the specified resources that you own and
         have
         shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
@@ -365,15 +364,15 @@
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
         Retrieves the lists of resources and principals that associated for resource
         shares that you
         own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
@@ -382,15 +381,15 @@
 
     async def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_invitations)
         """
@@ -402,15 +401,15 @@
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         permissionArn: str = ...,
-        permissionVersion: int = ...
+        permissionVersion: int = ...,
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared
         with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
@@ -419,15 +418,15 @@
 
     async def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListPendingInvitationResourcesResponseTypeDef:
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still
         `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
@@ -440,15 +439,15 @@
         permissionArn: str = ...,
         permissionVersion: int = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         resourceType: str = ...,
         featureSet: PermissionFeatureSetType = ...,
         defaultVersion: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPermissionAssociationsResponseTypeDef:
         """
         Lists information about the managed permission and its associations to any
         resource shares that use this managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
@@ -467,15 +466,15 @@
 
     async def list_permissions(
         self,
         *,
         resourceType: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionType: PermissionTypeFilterType = ...
+        permissionType: PermissionTypeFilterType = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the
         supported resource
         types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
@@ -487,15 +486,15 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPrincipalsResponseTypeDef:
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
@@ -504,15 +503,15 @@
 
     async def list_replace_permission_associations_work(
         self,
         *,
         workIds: Sequence[str] = ...,
         status: ReplacePermissionAssociationsWorkStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
         """
         Retrieves the current status of the asynchronous tasks performed by RAM when
         you perform the  ReplacePermissionAssociationsWork
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
@@ -530,15 +529,15 @@
         """
 
     async def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_types)
         """
@@ -549,15 +548,15 @@
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources that you added to a resource share or the resources that
         are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
@@ -603,15 +602,15 @@
 
     async def replace_permission_associations(
         self,
         *,
         fromPermissionArn: str,
         toPermissionArn: str,
         fromPermissionVersion: int = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> ReplacePermissionAssociationsResponseTypeDef:
         """
         Updates all resource shares that use a managed permission to a different
         managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
@@ -655,15 +654,15 @@
 
     async def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#update_resource_share)
         """
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/client.pyi` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     async def associate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> AssociateResourceShareResponseTypeDef:
         """
         Adds the specified list of principals and list of resources to a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share)
         """
@@ -168,15 +168,15 @@
     async def associate_resource_share_permission(
         self,
         *,
         resourceShareArn: str,
         permissionArn: str,
         replace: bool = ...,
         clientToken: str = ...,
-        permissionVersion: int = ...
+        permissionVersion: int = ...,
     ) -> AssociateResourceSharePermissionResponseTypeDef:
         """
         Adds or replaces the RAM permission for a resource type included in a resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.associate_resource_share_permission)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#associate_resource_share_permission)
@@ -201,15 +201,15 @@
     async def create_permission(
         self,
         *,
         name: str,
         resourceType: str,
         policyTemplate: str,
         clientToken: str = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreatePermissionResponseTypeDef:
         """
         Creates a customer managed permission for a specified resource type that you
         can attach to resource
         shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_permission)
@@ -232,15 +232,15 @@
         name: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         tags: Sequence[TagTypeDef] = ...,
         allowExternalPrincipals: bool = ...,
         clientToken: str = ...,
         permissionArns: Sequence[str] = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> CreateResourceShareResponseTypeDef:
         """
         Creates a resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.create_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#create_resource_share)
         """
@@ -280,15 +280,15 @@
     async def disassociate_resource_share(
         self,
         *,
         resourceShareArn: str,
         resourceArns: Sequence[str] = ...,
         principals: Sequence[str] = ...,
         clientToken: str = ...,
-        sources: Sequence[str] = ...
+        sources: Sequence[str] = ...,
     ) -> DisassociateResourceShareResponseTypeDef:
         """
         Removes the specified principals or resources from participating in the
         specified resource
         share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.disassociate_resource_share)
@@ -341,15 +341,15 @@
 
     async def get_resource_policies(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourcePoliciesResponseTypeDef:
         """
         Retrieves the resource policies for the specified resources that you own and
         have
         shared.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_policies)
@@ -361,15 +361,15 @@
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourceShareAssociationsResponseTypeDef:
         """
         Retrieves the lists of resources and principals that associated for resource
         shares that you
         own.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_associations)
@@ -378,15 +378,15 @@
 
     async def get_resource_share_invitations(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetResourceShareInvitationsResponseTypeDef:
         """
         Retrieves details about invitations that you have received for resource shares.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_share_invitations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#get_resource_share_invitations)
         """
@@ -398,15 +398,15 @@
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         permissionArn: str = ...,
-        permissionVersion: int = ...
+        permissionVersion: int = ...,
     ) -> GetResourceSharesResponseTypeDef:
         """
         Retrieves details about the resource shares that you own or that are shared
         with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.get_resource_shares)
@@ -415,15 +415,15 @@
 
     async def list_pending_invitation_resources(
         self,
         *,
         resourceShareInvitationArn: str,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListPendingInvitationResourcesResponseTypeDef:
         """
         Lists the resources in a resource share that is shared with you but for which
         the invitation is still
         `PENDING`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_pending_invitation_resources)
@@ -436,15 +436,15 @@
         permissionArn: str = ...,
         permissionVersion: int = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
         resourceType: str = ...,
         featureSet: PermissionFeatureSetType = ...,
         defaultVersion: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPermissionAssociationsResponseTypeDef:
         """
         Lists information about the managed permission and its associations to any
         resource shares that use this managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permission_associations)
@@ -463,15 +463,15 @@
 
     async def list_permissions(
         self,
         *,
         resourceType: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        permissionType: PermissionTypeFilterType = ...
+        permissionType: PermissionTypeFilterType = ...,
     ) -> ListPermissionsResponseTypeDef:
         """
         Retrieves a list of available RAM permissions that you can use for the
         supported resource
         types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_permissions)
@@ -483,15 +483,15 @@
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPrincipalsResponseTypeDef:
         """
         Lists the principals that you are sharing resources with or that are sharing
         resources with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_principals)
@@ -500,15 +500,15 @@
 
     async def list_replace_permission_associations_work(
         self,
         *,
         workIds: Sequence[str] = ...,
         status: ReplacePermissionAssociationsWorkStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListReplacePermissionAssociationsWorkResponseTypeDef:
         """
         Retrieves the current status of the asynchronous tasks performed by RAM when
         you perform the  ReplacePermissionAssociationsWork
         operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_replace_permission_associations_work)
@@ -526,15 +526,15 @@
         """
 
     async def list_resource_types(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListResourceTypesResponseTypeDef:
         """
         Lists the resource types that can be shared by RAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resource_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#list_resource_types)
         """
@@ -545,15 +545,15 @@
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        resourceRegionScope: ResourceRegionScopeFilterType = ...
+        resourceRegionScope: ResourceRegionScopeFilterType = ...,
     ) -> ListResourcesResponseTypeDef:
         """
         Lists the resources that you added to a resource share or the resources that
         are shared with
         you.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.list_resources)
@@ -599,15 +599,15 @@
 
     async def replace_permission_associations(
         self,
         *,
         fromPermissionArn: str,
         toPermissionArn: str,
         fromPermissionVersion: int = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> ReplacePermissionAssociationsResponseTypeDef:
         """
         Updates all resource shares that use a managed permission to a different
         managed
         permission.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.replace_permission_associations)
@@ -651,15 +651,15 @@
 
     async def update_resource_share(
         self,
         *,
         resourceShareArn: str,
         name: str = ...,
         allowExternalPrincipals: bool = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateResourceShareResponseTypeDef:
         """
         Modifies some of the properties of the specified resource share.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Client.update_resource_share)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/client/#update_resource_share)
         """
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/literals.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/literals.py`

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
     "GetResourcePoliciesPaginatorName",
     "GetResourceShareAssociationsPaginatorName",
     "GetResourceShareInvitationsPaginatorName",
     "GetResourceSharesPaginatorName",
     "ListPrincipalsPaginatorName",
     "ListResourcesPaginatorName",
@@ -44,15 +43,14 @@
     "RAMServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GetResourcePoliciesPaginatorName = Literal["get_resource_policies"]
 GetResourceShareAssociationsPaginatorName = Literal["get_resource_share_associations"]
 GetResourceShareInvitationsPaginatorName = Literal["get_resource_share_invitations"]
 GetResourceSharesPaginatorName = Literal["get_resource_shares"]
 ListPrincipalsPaginatorName = Literal["list_principals"]
 ListResourcesPaginatorName = Literal["list_resources"]
 PermissionFeatureSetType = Literal["CREATED_FROM_POLICY", "PROMOTING_TO_STANDARD", "STANDARD"]
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/literals.pyi` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/paginator.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "GetResourceShareAssociationsPaginator",
     "GetResourceShareInvitationsPaginator",
     "GetResourceSharesPaginator",
     "ListPrincipalsPaginator",
     "ListResourcesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -81,15 +80,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourcepoliciespaginator)
         """
 
 
@@ -103,15 +102,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 
@@ -122,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 
@@ -146,15 +145,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
         permissionVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourcesharespaginator)
         """
 
 
@@ -168,15 +167,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#listprincipalspaginator)
         """
 
 
@@ -191,13 +190,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/paginator.pyi` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceArns: Sequence[str],
         principal: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourcePoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourcepoliciespaginator)
         """
 
 class GetResourceShareAssociationsPaginator(AioPaginator):
@@ -99,15 +99,15 @@
         self,
         *,
         associationType: ResourceShareAssociationTypeType,
         resourceShareArns: Sequence[str] = ...,
         resourceArn: str = ...,
         principal: str = ...,
         associationStatus: ResourceShareAssociationStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceShareAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourceshareassociationspaginator)
         """
 
 class GetResourceShareInvitationsPaginator(AioPaginator):
@@ -117,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceShareInvitationArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceShareInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShareInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourceshareinvitationspaginator)
         """
 
 class GetResourceSharesPaginator(AioPaginator):
@@ -140,15 +140,15 @@
         resourceOwner: ResourceOwnerType,
         resourceShareArns: Sequence[str] = ...,
         resourceShareStatus: ResourceShareStatusType = ...,
         name: str = ...,
         tagFilters: Sequence[TagFilterTypeDef] = ...,
         permissionArn: str = ...,
         permissionVersion: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetResourceSharesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.GetResourceShares.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#getresourcesharespaginator)
         """
 
 class ListPrincipalsPaginator(AioPaginator):
@@ -161,15 +161,15 @@
         self,
         *,
         resourceOwner: ResourceOwnerType,
         resourceArn: str = ...,
         principals: Sequence[str] = ...,
         resourceType: str = ...,
         resourceShareArns: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListPrincipals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#listprincipalspaginator)
         """
 
 class ListResourcesPaginator(AioPaginator):
@@ -183,13 +183,13 @@
         *,
         resourceOwner: ResourceOwnerType,
         principal: str = ...,
         resourceType: str = ...,
         resourceArns: Sequence[str] = ...,
         resourceShareArns: Sequence[str] = ...,
         resourceRegionScope: ResourceRegionScopeFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/type_defs.py` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/type_defs.py`

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
     "AcceptResourceShareInvitationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociateResourceSharePermissionRequestRequestTypeDef",
     "AssociateResourceShareRequestRequestTypeDef",
     "ResourceShareAssociationTypeDef",
     "AssociatedPermissionTypeDef",
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram/type_defs.pyi` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/PKG-INFO` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ram
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.RAM 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.RAM 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/
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
 
 <a id="types-aiobotocore-ram"></a>
 
 # types-aiobotocore-ram
 
 [![PyPI - types-aiobotocore-ram](https://img.shields.io/pypi/v/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ram.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ram)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ram)](https://pepy.tech/project/types-aiobotocore-ram)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.RAM 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
+[aiobotocore.RAM 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
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
 [types-aiobotocore-ram docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ram/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ram-2.9.0/types_aiobotocore_ram.egg-info/SOURCES.txt` & `types-aiobotocore-ram-2.9.1/types_aiobotocore_ram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

