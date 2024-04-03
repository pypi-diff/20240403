# Comparing `tmp/types-aiobotocore-keyspaces-2.9.0.tar.gz` & `tmp/types-aiobotocore-keyspaces-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-keyspaces-2.9.0.tar", last modified: Wed Dec 13 19:59:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-keyspaces-2.9.1.tar", last modified: Thu Jan 18 01:21:01 2024, max compression
```

## Comparing `types-aiobotocore-keyspaces-2.9.0.tar` & `types-aiobotocore-keyspaces-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.885581 types-aiobotocore-keyspaces-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2023-12-13 19:59:38.885581 types-aiobotocore-keyspaces-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:38.885581 types-aiobotocore-keyspaces-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.881581 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14828 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2023-12-13 19:48:31.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9647 2023-12-13 19:48:31.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4191 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12676 2023-12-13 19:48:31.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12675 2023-12-13 19:48:31.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:29.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:38.885581 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13389 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:38.000000 types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.837246 types-aiobotocore-keyspaces-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-01-18 01:21:01.837246 types-aiobotocore-keyspaces-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:01.837246 types-aiobotocore-keyspaces-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.833246 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14831 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14828 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9647 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12675 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:18.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:01.837246 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13409 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:01.000000 types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/LICENSE` & `types-aiobotocore-keyspaces-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-keyspaces-2.9.0/PKG-INFO` & `types-aiobotocore-keyspaces-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-keyspaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Keyspaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Keyspaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/
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
 
 <a id="types-aiobotocore-keyspaces"></a>
 
 # types-aiobotocore-keyspaces
 
 [![PyPI - types-aiobotocore-keyspaces](https://img.shields.io/pypi/v/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [types-aiobotocore-keyspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/README.md` & `types-aiobotocore-keyspaces-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [types-aiobotocore-keyspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/setup.py` & `types-aiobotocore-keyspaces-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-keyspaces",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Keyspaces 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Keyspaces 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore keyspaces type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_keyspaces": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__init__.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import KeyspacesClient
 from .paginator import ListKeyspacesPaginator, ListTablesPaginator, ListTagsForResourcePaginator
 
 Client = KeyspacesClient
 
-
 __all__ = (
     "Client",
     "KeyspacesClient",
     "ListKeyspacesPaginator",
     "ListTablesPaginator",
     "ListTagsForResourcePaginator",
 )
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__init__.pyi` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/__main__.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Keyspaces 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Keyspaces 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
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

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/client.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KeyspacesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -106,15 +105,15 @@
         """
 
     async def create_keyspace(
         self,
         *,
         keyspaceName: str,
         tags: Sequence[TagTypeDef] = ...,
-        replicationSpecification: ReplicationSpecificationTypeDef = ...
+        replicationSpecification: ReplicationSpecificationTypeDef = ...,
     ) -> CreateKeyspaceResponseTypeDef:
         """
         The `CreateKeyspace` operation adds a new keyspace to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_keyspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/client/#create_keyspace)
         """
@@ -128,15 +127,15 @@
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
         tags: Sequence[TagTypeDef] = ...,
-        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...,
     ) -> CreateTableResponseTypeDef:
         """
         The `CreateTable` operation adds a new table to the specified keyspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/client/#create_table)
         """
@@ -227,15 +226,15 @@
         sourceTableName: str,
         targetKeyspaceName: str,
         targetTableName: str,
         restoreTimestamp: TimestampTypeDef = ...,
         capacitySpecificationOverride: CapacitySpecificationTypeDef = ...,
         encryptionSpecificationOverride: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecoveryOverride: PointInTimeRecoveryTypeDef = ...,
-        tagsOverride: Sequence[TagTypeDef] = ...
+        tagsOverride: Sequence[TagTypeDef] = ...,
     ) -> RestoreTableResponseTypeDef:
         """
         Restores the specified table to the specified point in time within the
         `earliest_restorable_timestamp` and the current
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.restore_table)
@@ -267,15 +266,15 @@
         tableName: str,
         addColumns: Sequence[ColumnDefinitionTypeDef] = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
-        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...,
     ) -> UpdateTableResponseTypeDef:
         """
         Adds new columns to the table or updates one of the table's settings, for
         example capacity mode, encryption, point-in-time recovery, or ttl
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.update_table)
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/client.pyi` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         """
 
     async def create_keyspace(
         self,
         *,
         keyspaceName: str,
         tags: Sequence[TagTypeDef] = ...,
-        replicationSpecification: ReplicationSpecificationTypeDef = ...
+        replicationSpecification: ReplicationSpecificationTypeDef = ...,
     ) -> CreateKeyspaceResponseTypeDef:
         """
         The `CreateKeyspace` operation adds a new keyspace to your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_keyspace)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/client/#create_keyspace)
         """
@@ -124,15 +124,15 @@
         comment: CommentTypeDef = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
         tags: Sequence[TagTypeDef] = ...,
-        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...,
     ) -> CreateTableResponseTypeDef:
         """
         The `CreateTable` operation adds a new table to the specified keyspace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/client/#create_table)
         """
@@ -223,15 +223,15 @@
         sourceTableName: str,
         targetKeyspaceName: str,
         targetTableName: str,
         restoreTimestamp: TimestampTypeDef = ...,
         capacitySpecificationOverride: CapacitySpecificationTypeDef = ...,
         encryptionSpecificationOverride: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecoveryOverride: PointInTimeRecoveryTypeDef = ...,
-        tagsOverride: Sequence[TagTypeDef] = ...
+        tagsOverride: Sequence[TagTypeDef] = ...,
     ) -> RestoreTableResponseTypeDef:
         """
         Restores the specified table to the specified point in time within the
         `earliest_restorable_timestamp` and the current
         time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.restore_table)
@@ -263,15 +263,15 @@
         tableName: str,
         addColumns: Sequence[ColumnDefinitionTypeDef] = ...,
         capacitySpecification: CapacitySpecificationTypeDef = ...,
         encryptionSpecification: EncryptionSpecificationTypeDef = ...,
         pointInTimeRecovery: PointInTimeRecoveryTypeDef = ...,
         ttl: TimeToLiveTypeDef = ...,
         defaultTimeToLive: int = ...,
-        clientSideTimestamps: ClientSideTimestampsTypeDef = ...
+        clientSideTimestamps: ClientSideTimestampsTypeDef = ...,
     ) -> UpdateTableResponseTypeDef:
         """
         Adds new columns to the table or updates one of the table's settings, for
         example capacity mode, encryption, point-in-time recovery, or ttl
         settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Client.update_table)
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/literals.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/literals.py`

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
     "ClientSideTimestampsStatusType",
     "EncryptionTypeType",
     "ListKeyspacesPaginatorName",
     "ListTablesPaginatorName",
     "ListTagsForResourcePaginatorName",
     "PointInTimeRecoveryStatusType",
@@ -35,15 +34,14 @@
     "KeyspacesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ClientSideTimestampsStatusType = Literal["ENABLED"]
 EncryptionTypeType = Literal["AWS_OWNED_KMS_KEY", "CUSTOMER_MANAGED_KMS_KEY"]
 ListKeyspacesPaginatorName = Literal["list_keyspaces"]
 ListTablesPaginatorName = Literal["list_tables"]
 ListTagsForResourcePaginatorName = Literal["list_tags_for_resource"]
 PointInTimeRecoveryStatusType = Literal["DISABLED", "ENABLED"]
 SortOrderType = Literal["ASC", "DESC"]
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/literals.pyi` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/paginator.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListKeyspacesPaginator", "ListTablesPaginator", "ListTagsForResourcePaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/paginator.pyi` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/type_defs.py` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
     "ClientSideTimestampsTypeDef",
     "ClusteringKeyTypeDef",
     "ColumnDefinitionTypeDef",
     "CommentTypeDef",
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces/type_defs.pyi` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/PKG-INFO` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-keyspaces
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Keyspaces 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Keyspaces 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/
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
 
 <a id="types-aiobotocore-keyspaces"></a>
 
 # types-aiobotocore-keyspaces
 
 [![PyPI - types-aiobotocore-keyspaces](https://img.shields.io/pypi/v/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-keyspaces.svg?color=blue)](https://pypi.org/project/types-aiobotocore-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-keyspaces)](https://pepy.tech/project/types-aiobotocore-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Keyspaces 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[aiobotocore.Keyspaces 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [types-aiobotocore-keyspaces docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_keyspaces/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-keyspaces-2.9.0/types_aiobotocore_keyspaces.egg-info/SOURCES.txt` & `types-aiobotocore-keyspaces-2.9.1/types_aiobotocore_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

