# Comparing `tmp/types-aiobotocore-athena-2.9.0.tar.gz` & `tmp/types-aiobotocore-athena-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-athena-2.9.0.tar", last modified: Wed Dec 13 19:58:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-athena-2.9.1.tar", last modified: Thu Jan 18 01:20:05 2024, max compression
```

## Comparing `types-aiobotocore-athena-2.9.0.tar` & `types-aiobotocore-athena-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.962067 types-aiobotocore-athena-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2023-12-13 19:58:37.962067 types-aiobotocore-athena-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12265 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:37.962067 types-aiobotocore-athena-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.962067 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49176 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49172 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2023-12-13 19:41:22.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11186 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8788 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53810 2023-12-13 19:41:22.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53809 2023-12-13 19:41:22.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:21.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.962067 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13824 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:58:37.000000 types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.805504 types-aiobotocore-athena-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-01-18 01:20:05.801504 types-aiobotocore-athena-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12265 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:05.805504 types-aiobotocore-athena-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.801504 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49191 2024-01-18 01:03:20.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49188 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-01-18 01:03:20.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11186 2024-01-18 01:03:20.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8798 2024-01-18 01:03:20.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8790 2024-01-18 01:03:20.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53809 2024-01-18 01:03:21.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53809 2024-01-18 01:03:21.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:19.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.801504 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:05.000000 types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-athena-2.9.0/LICENSE` & `types-aiobotocore-athena-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-athena-2.9.0/PKG-INFO` & `types-aiobotocore-athena-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Athena 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Athena 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
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
 
 <a id="types-aiobotocore-athena"></a>
 
 # types-aiobotocore-athena
 
 [![PyPI - types-aiobotocore-athena](https://img.shields.io/pypi/v/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-athena-2.9.0/README.md` & `types-aiobotocore-athena-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-athena-2.9.0/setup.py` & `types-aiobotocore-athena-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-athena",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Athena 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Athena 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore athena type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_athena": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__init__.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListQueryExecutionsPaginator,
     ListTableMetadataPaginator,
     ListTagsForResourcePaginator,
 )
 
 Client = AthenaClient
 
-
 __all__ = (
     "AthenaClient",
     "Client",
     "GetQueryResultsPaginator",
     "ListDataCatalogsPaginator",
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__init__.pyi` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/__main__.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Athena 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Athena 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/client.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AthenaClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -215,15 +214,15 @@
     async def create_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates (registers) a data catalog with the specified name and properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_data_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_data_catalog)
         """
@@ -232,15 +231,15 @@
         self,
         *,
         Name: str,
         Database: str,
         QueryString: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        WorkGroup: str = ...
+        WorkGroup: str = ...,
     ) -> CreateNamedQueryOutputTypeDef:
         """
         Creates a named query in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_named_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_named_query)
         """
@@ -277,15 +276,15 @@
 
     async def create_work_group(
         self,
         *,
         Name: str,
         Configuration: WorkGroupConfigurationTypeDef = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_work_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_work_group)
         """
@@ -536,15 +535,15 @@
     async def import_notebook(
         self,
         *,
         WorkGroup: str,
         Name: str,
         Payload: str,
         Type: Literal["IPYNB"],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> ImportNotebookOutputTypeDef:
         """
         Imports a single `ipynb` file to a Spark enabled workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.import_notebook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#import_notebook)
         """
@@ -563,15 +562,15 @@
 
     async def list_calculation_executions(
         self,
         *,
         SessionId: str,
         StateFilter: CalculationExecutionStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCalculationExecutionsResponseTypeDef:
         """
         Lists the calculations that have been submitted to a session in descending
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_calculation_executions)
@@ -621,15 +620,15 @@
 
     async def list_executors(
         self,
         *,
         SessionId: str,
         ExecutorStateFilter: ExecutorStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListExecutorsResponseTypeDef:
         """
         Lists, in descending order, the executors that joined a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_executors)
         """
@@ -647,15 +646,15 @@
 
     async def list_notebook_metadata(
         self,
         *,
         WorkGroup: str,
         Filters: FilterDefinitionTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListNotebookMetadataOutputTypeDef:
         """
         Displays the notebook files for the specified workgroup in paginated format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_notebook_metadata)
         """
@@ -696,15 +695,15 @@
 
     async def list_sessions(
         self,
         *,
         WorkGroup: str,
         StateFilter: SessionStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSessionsResponseTypeDef:
         """
         Lists the sessions in a workgroup that are in an active state like `CREATING`,
         `CREATED`, `IDLE`, or
         `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
@@ -715,15 +714,15 @@
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WorkGroup: str = ...
+        WorkGroup: str = ...,
     ) -> ListTableMetadataOutputTypeDef:
         """
         Lists the metadata for the tables in the specified data catalog database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_table_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_table_metadata)
         """
@@ -748,15 +747,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
 
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef],
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -765,15 +764,15 @@
     async def start_calculation_execution(
         self,
         *,
         SessionId: str,
         Description: str = ...,
         CalculationConfiguration: CalculationConfigurationTypeDef = ...,
         CodeBlock: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartCalculationExecutionResponseTypeDef:
         """
         Submits calculations for execution within a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_calculation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_calculation_execution)
         """
@@ -783,15 +782,15 @@
         *,
         QueryString: str,
         ClientRequestToken: str = ...,
         QueryExecutionContext: QueryExecutionContextTypeDef = ...,
         ResultConfiguration: ResultConfigurationTypeDef = ...,
         WorkGroup: str = ...,
         ExecutionParameters: Sequence[str] = ...,
-        ResultReuseConfiguration: ResultReuseConfigurationTypeDef = ...
+        ResultReuseConfiguration: ResultReuseConfigurationTypeDef = ...,
     ) -> StartQueryExecutionOutputTypeDef:
         """
         Runs the SQL query statements contained in the `Query`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
@@ -800,15 +799,15 @@
         self,
         *,
         WorkGroup: str,
         EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_session)
         """
@@ -867,15 +866,15 @@
 
     async def update_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
-        Parameters: Mapping[str, str] = ...
+        Parameters: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data catalog that has the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_data_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_data_catalog)
         """
@@ -893,15 +892,15 @@
     async def update_notebook(
         self,
         *,
         NotebookId: str,
         Payload: str,
         Type: Literal["IPYNB"],
         SessionId: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the contents of a Spark notebook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_notebook)
         """
@@ -928,15 +927,15 @@
 
     async def update_work_group(
         self,
         *,
         WorkGroup: str,
         Description: str = ...,
         ConfigurationUpdates: WorkGroupConfigurationUpdatesTypeDef = ...,
-        State: WorkGroupStateType = ...
+        State: WorkGroupStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_work_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_work_group)
         """
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/client.pyi` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -211,15 +211,15 @@
     async def create_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
         Parameters: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates (registers) a data catalog with the specified name and properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_data_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_data_catalog)
         """
@@ -228,15 +228,15 @@
         self,
         *,
         Name: str,
         Database: str,
         QueryString: str,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        WorkGroup: str = ...
+        WorkGroup: str = ...,
     ) -> CreateNamedQueryOutputTypeDef:
         """
         Creates a named query in the specified workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_named_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_named_query)
         """
@@ -273,15 +273,15 @@
 
     async def create_work_group(
         self,
         *,
         Name: str,
         Configuration: WorkGroupConfigurationTypeDef = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Creates a workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.create_work_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#create_work_group)
         """
@@ -532,15 +532,15 @@
     async def import_notebook(
         self,
         *,
         WorkGroup: str,
         Name: str,
         Payload: str,
         Type: Literal["IPYNB"],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> ImportNotebookOutputTypeDef:
         """
         Imports a single `ipynb` file to a Spark enabled workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.import_notebook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#import_notebook)
         """
@@ -559,15 +559,15 @@
 
     async def list_calculation_executions(
         self,
         *,
         SessionId: str,
         StateFilter: CalculationExecutionStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCalculationExecutionsResponseTypeDef:
         """
         Lists the calculations that have been submitted to a session in descending
         order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_calculation_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_calculation_executions)
@@ -617,15 +617,15 @@
 
     async def list_executors(
         self,
         *,
         SessionId: str,
         ExecutorStateFilter: ExecutorStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListExecutorsResponseTypeDef:
         """
         Lists, in descending order, the executors that joined a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_executors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_executors)
         """
@@ -643,15 +643,15 @@
 
     async def list_notebook_metadata(
         self,
         *,
         WorkGroup: str,
         Filters: FilterDefinitionTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListNotebookMetadataOutputTypeDef:
         """
         Displays the notebook files for the specified workgroup in paginated format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_notebook_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_notebook_metadata)
         """
@@ -692,15 +692,15 @@
 
     async def list_sessions(
         self,
         *,
         WorkGroup: str,
         StateFilter: SessionStateType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListSessionsResponseTypeDef:
         """
         Lists the sessions in a workgroup that are in an active state like `CREATING`,
         `CREATED`, `IDLE`, or
         `BUSY`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_sessions)
@@ -711,15 +711,15 @@
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WorkGroup: str = ...
+        WorkGroup: str = ...,
     ) -> ListTableMetadataOutputTypeDef:
         """
         Lists the metadata for the tables in the specified data catalog database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_table_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_table_metadata)
         """
@@ -744,15 +744,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
 
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef],
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -761,15 +761,15 @@
     async def start_calculation_execution(
         self,
         *,
         SessionId: str,
         Description: str = ...,
         CalculationConfiguration: CalculationConfigurationTypeDef = ...,
         CodeBlock: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartCalculationExecutionResponseTypeDef:
         """
         Submits calculations for execution within a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_calculation_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_calculation_execution)
         """
@@ -779,15 +779,15 @@
         *,
         QueryString: str,
         ClientRequestToken: str = ...,
         QueryExecutionContext: QueryExecutionContextTypeDef = ...,
         ResultConfiguration: ResultConfigurationTypeDef = ...,
         WorkGroup: str = ...,
         ExecutionParameters: Sequence[str] = ...,
-        ResultReuseConfiguration: ResultReuseConfigurationTypeDef = ...
+        ResultReuseConfiguration: ResultReuseConfigurationTypeDef = ...,
     ) -> StartQueryExecutionOutputTypeDef:
         """
         Runs the SQL query statements contained in the `Query`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
@@ -796,15 +796,15 @@
         self,
         *,
         WorkGroup: str,
         EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_session)
         """
@@ -863,15 +863,15 @@
 
     async def update_data_catalog(
         self,
         *,
         Name: str,
         Type: DataCatalogTypeType,
         Description: str = ...,
-        Parameters: Mapping[str, str] = ...
+        Parameters: Mapping[str, str] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the data catalog that has the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_data_catalog)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_data_catalog)
         """
@@ -889,15 +889,15 @@
     async def update_notebook(
         self,
         *,
         NotebookId: str,
         Payload: str,
         Type: Literal["IPYNB"],
         SessionId: str = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> Dict[str, Any]:
         """
         Updates the contents of a Spark notebook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_notebook)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_notebook)
         """
@@ -924,15 +924,15 @@
 
     async def update_work_group(
         self,
         *,
         WorkGroup: str,
         Description: str = ...,
         ConfigurationUpdates: WorkGroupConfigurationUpdatesTypeDef = ...,
-        State: WorkGroupStateType = ...
+        State: WorkGroupStateType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the workgroup with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.update_work_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#update_work_group)
         """
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/literals.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/literals.py`

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
     "AuthenticationTypeType",
     "CalculationExecutionStateType",
     "CapacityAllocationStatusType",
     "CapacityReservationStatusType",
     "ColumnNullableType",
     "DataCatalogTypeType",
@@ -46,15 +45,14 @@
     "AthenaServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthenticationTypeType = Literal["DIRECTORY_IDENTITY"]
 CalculationExecutionStateType = Literal[
     "CANCELED", "CANCELING", "COMPLETED", "CREATED", "CREATING", "FAILED", "QUEUED", "RUNNING"
 ]
 CapacityAllocationStatusType = Literal["FAILED", "PENDING", "SUCCEEDED"]
 CapacityReservationStatusType = Literal[
     "ACTIVE", "CANCELLED", "CANCELLING", "FAILED", "PENDING", "UPDATE_PENDING"
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/literals.pyi` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/paginator.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
     "ListQueryExecutionsPaginator",
     "ListTableMetadataPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -107,15 +106,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         WorkGroup: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
         """
 
 
@@ -158,15 +157,15 @@
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         WorkGroup: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
         """
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/paginator.pyi` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         WorkGroup: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
         """
 
 class ListNamedQueriesPaginator(AioPaginator):
@@ -150,15 +150,15 @@
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
         WorkGroup: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/type_defs.py` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena/type_defs.pyi` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/PKG-INFO` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Athena 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Athena 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
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
 
 <a id="types-aiobotocore-athena"></a>
 
 # types-aiobotocore-athena
 
 [![PyPI - types-aiobotocore-athena](https://img.shields.io/pypi/v/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Athena 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[aiobotocore.Athena 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-athena-2.9.0/types_aiobotocore_athena.egg-info/SOURCES.txt` & `types-aiobotocore-athena-2.9.1/types_aiobotocore_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

