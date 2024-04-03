# Comparing `tmp/types-aiobotocore-appsync-2.9.0.tar.gz` & `tmp/types-aiobotocore-appsync-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appsync-2.9.0.tar", last modified: Wed Dec 13 19:58:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-appsync-2.9.1.tar", last modified: Thu Jan 18 01:20:05 2024, max compression
```

## Comparing `types-aiobotocore-appsync-2.9.0.tar` & `types-aiobotocore-appsync-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.218073 types-aiobotocore-appsync-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2023-12-13 19:58:37.218073 types-aiobotocore-appsync-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12212 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:37.218073 types-aiobotocore-appsync-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:41:17.000000 types-aiobotocore-appsync-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.218073 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47297 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    47293 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12160 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12158 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8752 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51946 2023-12-13 19:41:19.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51945 2023-12-13 19:41:19.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:18.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:37.218073 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:58:37.000000 types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.109506 types-aiobotocore-appsync-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-01-18 01:20:05.109506 types-aiobotocore-appsync-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12212 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:05.109506 types-aiobotocore-appsync-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.105506 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47313 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47310 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-01-18 01:03:17.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12158 2024-01-18 01:03:17.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-01-18 01:03:17.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51945 2024-01-18 01:03:18.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51945 2024-01-18 01:03:18.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:16.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:05.105506 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:05.000000 types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appsync-2.9.0/LICENSE` & `types-aiobotocore-appsync-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-appsync-2.9.0/PKG-INFO` & `types-aiobotocore-appsync-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appsync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/
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
 
 <a id="types-aiobotocore-appsync"></a>
 
 # types-aiobotocore-appsync
 
 [![PyPI - types-aiobotocore-appsync](https://img.shields.io/pypi/v/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[aiobotocore.AppSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appsync-2.9.0/README.md` & `types-aiobotocore-appsync-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[aiobotocore.AppSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appsync-2.9.0/setup.py` & `types-aiobotocore-appsync-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appsync",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.AppSync 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.AppSync 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore appsync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appsync": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__init__.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     ListResolversByFunctionPaginator,
     ListResolversPaginator,
     ListTypesPaginator,
 )
 
 Client = AppSyncClient
 
-
 __all__ = (
     "AppSyncClient",
     "Client",
     "ListApiKeysPaginator",
     "ListDataSourcesPaginator",
     "ListFunctionsPaginator",
     "ListGraphqlApisPaginator",
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__init__.pyi` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/__main__.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppSync 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.AppSync 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
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

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/client.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppSyncClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -173,15 +172,15 @@
 
     async def associate_merged_graphql_api(
         self,
         *,
         sourceApiIdentifier: str,
         mergedApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> AssociateMergedGraphqlApiResponseTypeDef:
         """
         Creates an association between a Merged API and source API using the source
         API's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_merged_graphql_api)
@@ -190,15 +189,15 @@
 
     async def associate_source_graphql_api(
         self,
         *,
         mergedApiIdentifier: str,
         sourceApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> AssociateSourceGraphqlApiResponseTypeDef:
         """
         Creates an association between a Merged API and source API using the Merged
         API's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_source_graphql_api)
@@ -225,15 +224,15 @@
         self,
         *,
         apiId: str,
         ttl: int,
         apiCachingBehavior: ApiCachingBehaviorType,
         type: ApiCacheTypeType,
         transitEncryptionEnabled: bool = ...,
-        atRestEncryptionEnabled: bool = ...
+        atRestEncryptionEnabled: bool = ...,
     ) -> CreateApiCacheResponseTypeDef:
         """
         Creates a cache for the GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_api_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_api_cache)
         """
@@ -258,15 +257,15 @@
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
         relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
-        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_data_source)
         """
@@ -290,15 +289,15 @@
         description: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         functionVersion: str = ...,
         syncConfig: SyncConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> CreateFunctionResponseTypeDef:
         """
         Creates a `Function` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_function)
         """
@@ -314,15 +313,15 @@
         tags: Mapping[str, str] = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         visibility: GraphQLApiVisibilityType = ...,
         apiType: GraphQLApiTypeType = ...,
         mergedApiExecutionRoleArn: str = ...,
-        ownerContact: str = ...
+        ownerContact: str = ...,
     ) -> CreateGraphqlApiResponseTypeDef:
         """
         Creates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_graphql_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_graphql_api)
         """
@@ -338,15 +337,15 @@
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
         pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
         cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_resolver)
         """
@@ -525,15 +524,15 @@
 
     async def get_data_source_introspection(
         self,
         *,
         introspectionId: str,
         includeModelsSDL: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetDataSourceIntrospectionResponseTypeDef:
         """
         Retrieves the record of an existing introspection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_data_source_introspection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#get_data_source_introspection)
         """
@@ -654,15 +653,15 @@
 
     async def list_graphql_apis(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         apiType: GraphQLApiTypeType = ...,
-        owner: OwnershipType = ...
+        owner: OwnershipType = ...,
     ) -> ListGraphqlApisResponseTypeDef:
         """
         Lists your GraphQL APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_graphql_apis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_graphql_apis)
         """
@@ -709,15 +708,15 @@
 
     async def list_types(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTypesResponseTypeDef:
         """
         Lists the types for a given API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types)
         """
@@ -725,15 +724,15 @@
     async def list_types_by_association(
         self,
         *,
         mergedApiIdentifier: str,
         associationId: str,
         format: TypeDefinitionFormatType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTypesByAssociationResponseTypeDef:
         """
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types_by_association)
         """
@@ -786,15 +785,15 @@
 
     async def update_api_cache(
         self,
         *,
         apiId: str,
         ttl: int,
         apiCachingBehavior: ApiCachingBehaviorType,
-        type: ApiCacheTypeType
+        type: ApiCacheTypeType,
     ) -> UpdateApiCacheResponseTypeDef:
         """
         Updates the cache for the GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_api_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_api_cache)
         """
@@ -819,15 +818,15 @@
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
         relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
-        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_data_source)
         """
@@ -852,15 +851,15 @@
         description: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         functionVersion: str = ...,
         syncConfig: SyncConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> UpdateFunctionResponseTypeDef:
         """
         Updates a `Function` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_function)
         """
@@ -874,15 +873,15 @@
         authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         mergedApiExecutionRoleArn: str = ...,
-        ownerContact: str = ...
+        ownerContact: str = ...,
     ) -> UpdateGraphqlApiResponseTypeDef:
         """
         Updates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_graphql_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_graphql_api)
         """
@@ -898,30 +897,30 @@
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
         pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
         cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_resolver)
         """
 
     async def update_source_api_association(
         self,
         *,
         associationId: str,
         mergedApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> UpdateSourceApiAssociationResponseTypeDef:
         """
         Updates some of the configuration choices of a particular source API
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_source_api_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_source_api_association)
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/client.pyi` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
 
     async def associate_merged_graphql_api(
         self,
         *,
         sourceApiIdentifier: str,
         mergedApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> AssociateMergedGraphqlApiResponseTypeDef:
         """
         Creates an association between a Merged API and source API using the source
         API's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_merged_graphql_api)
@@ -186,15 +186,15 @@
 
     async def associate_source_graphql_api(
         self,
         *,
         mergedApiIdentifier: str,
         sourceApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> AssociateSourceGraphqlApiResponseTypeDef:
         """
         Creates an association between a Merged API and source API using the Merged
         API's
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.associate_source_graphql_api)
@@ -221,15 +221,15 @@
         self,
         *,
         apiId: str,
         ttl: int,
         apiCachingBehavior: ApiCachingBehaviorType,
         type: ApiCacheTypeType,
         transitEncryptionEnabled: bool = ...,
-        atRestEncryptionEnabled: bool = ...
+        atRestEncryptionEnabled: bool = ...,
     ) -> CreateApiCacheResponseTypeDef:
         """
         Creates a cache for the GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_api_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_api_cache)
         """
@@ -254,15 +254,15 @@
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
         relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
-        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_data_source)
         """
@@ -286,15 +286,15 @@
         description: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         functionVersion: str = ...,
         syncConfig: SyncConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> CreateFunctionResponseTypeDef:
         """
         Creates a `Function` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_function)
         """
@@ -310,15 +310,15 @@
         tags: Mapping[str, str] = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         visibility: GraphQLApiVisibilityType = ...,
         apiType: GraphQLApiTypeType = ...,
         mergedApiExecutionRoleArn: str = ...,
-        ownerContact: str = ...
+        ownerContact: str = ...,
     ) -> CreateGraphqlApiResponseTypeDef:
         """
         Creates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_graphql_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_graphql_api)
         """
@@ -334,15 +334,15 @@
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
         pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
         cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.create_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#create_resolver)
         """
@@ -521,15 +521,15 @@
 
     async def get_data_source_introspection(
         self,
         *,
         introspectionId: str,
         includeModelsSDL: bool = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetDataSourceIntrospectionResponseTypeDef:
         """
         Retrieves the record of an existing introspection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.get_data_source_introspection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#get_data_source_introspection)
         """
@@ -650,15 +650,15 @@
 
     async def list_graphql_apis(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
         apiType: GraphQLApiTypeType = ...,
-        owner: OwnershipType = ...
+        owner: OwnershipType = ...,
     ) -> ListGraphqlApisResponseTypeDef:
         """
         Lists your GraphQL APIs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_graphql_apis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_graphql_apis)
         """
@@ -705,15 +705,15 @@
 
     async def list_types(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTypesResponseTypeDef:
         """
         Lists the types for a given API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types)
         """
@@ -721,15 +721,15 @@
     async def list_types_by_association(
         self,
         *,
         mergedApiIdentifier: str,
         associationId: str,
         format: TypeDefinitionFormatType,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListTypesByAssociationResponseTypeDef:
         """
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types_by_association)
         """
@@ -782,15 +782,15 @@
 
     async def update_api_cache(
         self,
         *,
         apiId: str,
         ttl: int,
         apiCachingBehavior: ApiCachingBehaviorType,
-        type: ApiCacheTypeType
+        type: ApiCacheTypeType,
     ) -> UpdateApiCacheResponseTypeDef:
         """
         Updates the cache for the GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_api_cache)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_api_cache)
         """
@@ -815,15 +815,15 @@
         serviceRoleArn: str = ...,
         dynamodbConfig: DynamodbDataSourceConfigTypeDef = ...,
         lambdaConfig: LambdaDataSourceConfigTypeDef = ...,
         elasticsearchConfig: ElasticsearchDataSourceConfigTypeDef = ...,
         openSearchServiceConfig: OpenSearchServiceDataSourceConfigTypeDef = ...,
         httpConfig: HttpDataSourceConfigTypeDef = ...,
         relationalDatabaseConfig: RelationalDatabaseDataSourceConfigTypeDef = ...,
-        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...
+        eventBridgeConfig: EventBridgeDataSourceConfigTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_data_source)
         """
@@ -848,15 +848,15 @@
         description: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         functionVersion: str = ...,
         syncConfig: SyncConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> UpdateFunctionResponseTypeDef:
         """
         Updates a `Function` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_function)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_function)
         """
@@ -870,15 +870,15 @@
         authenticationType: AuthenticationTypeType = ...,
         userPoolConfig: UserPoolConfigTypeDef = ...,
         openIDConnectConfig: OpenIDConnectConfigTypeDef = ...,
         additionalAuthenticationProviders: Sequence[AdditionalAuthenticationProviderTypeDef] = ...,
         xrayEnabled: bool = ...,
         lambdaAuthorizerConfig: LambdaAuthorizerConfigTypeDef = ...,
         mergedApiExecutionRoleArn: str = ...,
-        ownerContact: str = ...
+        ownerContact: str = ...,
     ) -> UpdateGraphqlApiResponseTypeDef:
         """
         Updates a `GraphqlApi` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_graphql_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_graphql_api)
         """
@@ -894,30 +894,30 @@
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
         pipelineConfig: PipelineConfigTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
         cachingConfig: CachingConfigTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
-        code: str = ...
+        code: str = ...,
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_resolver)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_resolver)
         """
 
     async def update_source_api_association(
         self,
         *,
         associationId: str,
         mergedApiIdentifier: str,
         description: str = ...,
-        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...
+        sourceApiAssociationConfig: SourceApiAssociationConfigTypeDef = ...,
     ) -> UpdateSourceApiAssociationResponseTypeDef:
         """
         Updates some of the configuration choices of a particular source API
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.update_source_api_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#update_source_api_association)
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/literals.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/literals.py`

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
     "ApiCacheStatusType",
     "ApiCacheTypeType",
     "ApiCachingBehaviorType",
     "AssociationStatusType",
     "AuthenticationTypeType",
     "AuthorizationTypeType",
@@ -54,15 +53,14 @@
     "AppSyncServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiCacheStatusType = Literal["AVAILABLE", "CREATING", "DELETING", "FAILED", "MODIFYING"]
 ApiCacheTypeType = Literal[
     "LARGE",
     "LARGE_12X",
     "LARGE_2X",
     "LARGE_4X",
     "LARGE_8X",
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/literals.pyi` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/paginator.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     "ListFunctionsPaginator",
     "ListGraphqlApisPaginator",
     "ListResolversPaginator",
     "ListResolversByFunctionPaginator",
     "ListTypesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -123,15 +122,15 @@
     """
 
     def paginate(
         self,
         *,
         apiType: GraphQLApiTypeType = ...,
         owner: OwnershipType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listgraphqlapispaginator)
         """
 
 
@@ -172,13 +171,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/paginator.pyi` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         apiType: GraphQLApiTypeType = ...,
         owner: OwnershipType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listgraphqlapispaginator)
         """
 
 class ListResolversPaginator(AioPaginator):
@@ -163,13 +163,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/type_defs.py` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CognitoUserPoolConfigTypeDef",
     "LambdaAuthorizerConfigTypeDef",
     "OpenIDConnectConfigTypeDef",
     "ApiAssociationTypeDef",
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync/type_defs.pyi` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/PKG-INFO` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appsync
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.AppSync 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.AppSync 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/
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
 
 <a id="types-aiobotocore-appsync"></a>
 
 # types-aiobotocore-appsync
 
 [![PyPI - types-aiobotocore-appsync](https://img.shields.io/pypi/v/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.AppSync 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
+[aiobotocore.AppSync 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-appsync-2.9.0/types_aiobotocore_appsync.egg-info/SOURCES.txt` & `types-aiobotocore-appsync-2.9.1/types_aiobotocore_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

