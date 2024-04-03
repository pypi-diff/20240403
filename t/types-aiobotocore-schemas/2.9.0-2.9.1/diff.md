# Comparing `tmp/types-aiobotocore-schemas-2.9.0.tar.gz` & `tmp/types-aiobotocore-schemas-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-schemas-2.9.0.tar", last modified: Wed Dec 13 20:00:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-schemas-2.9.1.tar", last modified: Thu Jan 18 01:21:45 2024, max compression
```

## Comparing `types-aiobotocore-schemas-2.9.0.tar` & `types-aiobotocore-schemas-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.209165 types-aiobotocore-schemas-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2023-12-13 20:00:27.209165 types-aiobotocore-schemas-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:27.209165 types-aiobotocore-schemas-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.209165 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25261 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25257 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2023-12-13 19:55:50.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9672 2023-12-13 19:55:50.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20625 2023-12-13 19:55:50.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20624 2023-12-13 19:55:50.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-12-13 19:55:49.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:27.209165 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14222 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:27.000000 types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.913048 types-aiobotocore-schemas-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-01-18 01:21:45.913048 types-aiobotocore-schemas-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:45.913048 types-aiobotocore-schemas-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.913048 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25263 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-01-18 01:17:21.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9672 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-01-18 01:17:21.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20624 2024-01-18 01:17:21.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-01-18 01:17:20.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:45.913048 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14242 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:45.000000 types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-schemas-2.9.0/LICENSE` & `types-aiobotocore-schemas-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-schemas-2.9.0/PKG-INFO` & `types-aiobotocore-schemas-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Schemas 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Schemas 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
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
 
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-schemas-2.9.0/README.md` & `types-aiobotocore-schemas-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-schemas-2.9.0/setup.py` & `types-aiobotocore-schemas-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-schemas",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Schemas 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Schemas 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore schemas type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_schemas": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__init__.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
     ListSchemaVersionsPaginator,
     SearchSchemasPaginator,
 )
 from .waiter import CodeBindingExistsWaiter
 
 Client = SchemasClient
 
-
 __all__ = (
     "Client",
     "CodeBindingExistsWaiter",
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__init__.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/__main__.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Schemas 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Schemas 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/client.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 from .waiter import CodeBindingExistsWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SchemasClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -124,15 +123,15 @@
 
     async def create_discoverer(
         self,
         *,
         SourceArn: str,
         Description: str = ...,
         CrossAccount: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDiscovererResponseTypeDef:
         """
         Creates a discoverer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_discoverer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#create_discoverer)
         """
@@ -151,15 +150,15 @@
         self,
         *,
         Content: str,
         RegistryName: str,
         SchemaName: str,
         Type: TypeType,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSchemaResponseTypeDef:
         """
         Creates a schema definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#create_schema)
         """
@@ -304,30 +303,30 @@
 
     async def list_discoverers(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        SourceArnPrefix: str = ...
+        SourceArnPrefix: str = ...,
     ) -> ListDiscoverersResponseTypeDef:
         """
         List the discoverers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_discoverers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_discoverers)
         """
 
     async def list_registries(
         self,
         *,
         Limit: int = ...,
         NextToken: str = ...,
         RegistryNamePrefix: str = ...,
-        Scope: str = ...
+        Scope: str = ...,
     ) -> ListRegistriesResponseTypeDef:
         """
         List the registries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_registries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_registries)
         """
@@ -344,15 +343,15 @@
 
     async def list_schemas(
         self,
         *,
         RegistryName: str,
         Limit: int = ...,
         NextToken: str = ...,
-        SchemaNamePrefix: str = ...
+        SchemaNamePrefix: str = ...,
     ) -> ListSchemasResponseTypeDef:
         """
         List the schemas.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_schemas)
         """
@@ -462,15 +461,15 @@
         self,
         *,
         RegistryName: str,
         SchemaName: str,
         ClientTokenId: str = ...,
         Content: str = ...,
         Description: str = ...,
-        Type: TypeType = ...
+        Type: TypeType = ...,
     ) -> UpdateSchemaResponseTypeDef:
         """
         Updates the schema definition .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.update_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#update_schema)
         """
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/client.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     async def create_discoverer(
         self,
         *,
         SourceArn: str,
         Description: str = ...,
         CrossAccount: bool = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDiscovererResponseTypeDef:
         """
         Creates a discoverer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_discoverer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#create_discoverer)
         """
@@ -147,15 +147,15 @@
         self,
         *,
         Content: str,
         RegistryName: str,
         SchemaName: str,
         Type: TypeType,
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateSchemaResponseTypeDef:
         """
         Creates a schema definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.create_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#create_schema)
         """
@@ -300,30 +300,30 @@
 
     async def list_discoverers(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         Limit: int = ...,
         NextToken: str = ...,
-        SourceArnPrefix: str = ...
+        SourceArnPrefix: str = ...,
     ) -> ListDiscoverersResponseTypeDef:
         """
         List the discoverers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_discoverers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_discoverers)
         """
 
     async def list_registries(
         self,
         *,
         Limit: int = ...,
         NextToken: str = ...,
         RegistryNamePrefix: str = ...,
-        Scope: str = ...
+        Scope: str = ...,
     ) -> ListRegistriesResponseTypeDef:
         """
         List the registries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_registries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_registries)
         """
@@ -340,15 +340,15 @@
 
     async def list_schemas(
         self,
         *,
         RegistryName: str,
         Limit: int = ...,
         NextToken: str = ...,
-        SchemaNamePrefix: str = ...
+        SchemaNamePrefix: str = ...,
     ) -> ListSchemasResponseTypeDef:
         """
         List the schemas.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#list_schemas)
         """
@@ -458,15 +458,15 @@
         self,
         *,
         RegistryName: str,
         SchemaName: str,
         ClientTokenId: str = ...,
         Content: str = ...,
         Description: str = ...,
-        Type: TypeType = ...
+        Type: TypeType = ...,
     ) -> UpdateSchemaResponseTypeDef:
         """
         Updates the schema definition .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Client.update_schema)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/client/#update_schema)
         """
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/literals.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/literals.py`

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
     "CodeBindingExistsWaiterName",
     "CodeGenerationStatusType",
     "DiscovererStateType",
     "ListDiscoverersPaginatorName",
     "ListRegistriesPaginatorName",
     "ListSchemaVersionsPaginatorName",
@@ -34,15 +33,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 CodeBindingExistsWaiterName = Literal["code_binding_exists"]
 CodeGenerationStatusType = Literal["CREATE_COMPLETE", "CREATE_FAILED", "CREATE_IN_PROGRESS"]
 DiscovererStateType = Literal["STARTED", "STOPPED"]
 ListDiscoverersPaginatorName = Literal["list_discoverers"]
 ListRegistriesPaginatorName = Literal["list_registries"]
 ListSchemaVersionsPaginatorName = Literal["list_schema_versions"]
 ListSchemasPaginatorName = Literal["list_schemas"]
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/literals.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/paginator.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
     "SearchSchemasPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -69,15 +68,15 @@
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
         """
 
 
@@ -88,15 +87,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
         """
 
 
@@ -122,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
         """
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/paginator.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
         """
 
 class ListRegistriesPaginator(AioPaginator):
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
         """
 
 class ListSchemaVersionsPaginator(AioPaginator):
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
         """
 
 class SearchSchemasPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/type_defs.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/type_defs.py`

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
     "CreateDiscovererRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateRegistryRequestRequestTypeDef",
     "CreateSchemaRequestRequestTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/type_defs.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/waiter.py` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/waiter.py`

 * *Files 13% similar despite different names*

```diff
@@ -37,13 +37,13 @@
     async def wait(
         self,
         *,
         Language: str,
         RegistryName: str,
         SchemaName: str,
         SchemaVersion: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Waiter.CodeBindingExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/waiters/#codebindingexistswaiter)
         """
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas/waiter.pyi` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas/waiter.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -36,13 +36,13 @@
     async def wait(
         self,
         *,
         Language: str,
         RegistryName: str,
         SchemaName: str,
         SchemaVersion: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Waiter.CodeBindingExists.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/waiters/#codebindingexistswaiter)
         """
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/PKG-INFO` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Schemas 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Schemas 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
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
 
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Schemas 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
+[aiobotocore.Schemas 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-schemas-2.9.0/types_aiobotocore_schemas.egg-info/SOURCES.txt` & `types-aiobotocore-schemas-2.9.1/types_aiobotocore_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

