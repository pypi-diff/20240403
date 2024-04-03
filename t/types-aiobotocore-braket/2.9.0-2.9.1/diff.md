# Comparing `tmp/types-aiobotocore-braket-2.9.0.tar.gz` & `tmp/types-aiobotocore-braket-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-braket-2.9.0.tar", last modified: Wed Dec 13 19:58:43 2023, max compression
+gzip compressed data, was "types-aiobotocore-braket-2.9.1.tar", last modified: Thu Jan 18 01:20:10 2024, max compression
```

## Comparing `types-aiobotocore-braket-2.9.0.tar` & `types-aiobotocore-braket-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.582020 types-aiobotocore-braket-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2023-12-13 19:58:43.582020 types-aiobotocore-braket-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11597 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:43.582020 types-aiobotocore-braket-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.578020 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14019 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11106 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15260 2023-12-13 19:41:49.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15259 2023-12-13 19:41:48.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:41:47.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:43.582020 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13156 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:58:43.000000 types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.865486 types-aiobotocore-braket-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-01-18 01:20:10.865486 types-aiobotocore-braket-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11597 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:10.865486 types-aiobotocore-braket-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.861487 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14020 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15259 2024-01-18 01:03:46.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:03:45.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:10.865486 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13176 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:20:10.000000 types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-braket-2.9.0/LICENSE` & `types-aiobotocore-braket-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-braket-2.9.0/PKG-INFO` & `types-aiobotocore-braket-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Braket 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Braket 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
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
 
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-braket-2.9.0/README.md` & `types-aiobotocore-braket-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-braket-2.9.0/setup.py` & `types-aiobotocore-braket-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-braket",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Braket 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Braket 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore braket type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_braket": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__init__.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import BraketClient
 from .paginator import SearchDevicesPaginator, SearchJobsPaginator, SearchQuantumTasksPaginator
 
 Client = BraketClient
 
-
 __all__ = (
     "BraketClient",
     "Client",
     "SearchDevicesPaginator",
     "SearchJobsPaginator",
     "SearchQuantumTasksPaginator",
 )
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__init__.pyi` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/__main__.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Braket 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Braket 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/client.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BraketClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -139,15 +138,15 @@
         outputDataConfig: JobOutputDataConfigTypeDef,
         roleArn: str,
         associations: Sequence[AssociationTypeDef] = ...,
         checkpointConfig: JobCheckpointConfigTypeDef = ...,
         hyperParameters: Mapping[str, str] = ...,
         inputDataConfig: Sequence[InputFileConfigTypeDef] = ...,
         stoppingCondition: JobStoppingConditionTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates an Amazon Braket job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#create_job)
         """
@@ -160,15 +159,15 @@
         deviceArn: str,
         outputS3Bucket: str,
         outputS3KeyPrefix: str,
         shots: int,
         associations: Sequence[AssociationTypeDef] = ...,
         deviceParameters: str = ...,
         jobToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuantumTaskResponseTypeDef:
         """
         Creates a quantum task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_quantum_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#create_quantum_task)
         """
@@ -226,43 +225,43 @@
         """
 
     async def search_devices(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchDevicesResponseTypeDef:
         """
         Searches for devices using the specified filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_devices)
         """
 
     async def search_jobs(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchJobsResponseTypeDef:
         """
         Searches for Amazon Braket jobs that match the specified filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_jobs)
         """
 
     async def search_quantum_tasks(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuantumTasksResponseTypeDef:
         """
         Searches for tasks that match the specified filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_quantum_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_quantum_tasks)
         """
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/client.pyi` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         outputDataConfig: JobOutputDataConfigTypeDef,
         roleArn: str,
         associations: Sequence[AssociationTypeDef] = ...,
         checkpointConfig: JobCheckpointConfigTypeDef = ...,
         hyperParameters: Mapping[str, str] = ...,
         inputDataConfig: Sequence[InputFileConfigTypeDef] = ...,
         stoppingCondition: JobStoppingConditionTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateJobResponseTypeDef:
         """
         Creates an Amazon Braket job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#create_job)
         """
@@ -156,15 +156,15 @@
         deviceArn: str,
         outputS3Bucket: str,
         outputS3KeyPrefix: str,
         shots: int,
         associations: Sequence[AssociationTypeDef] = ...,
         deviceParameters: str = ...,
         jobToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuantumTaskResponseTypeDef:
         """
         Creates a quantum task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.create_quantum_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#create_quantum_task)
         """
@@ -222,43 +222,43 @@
         """
 
     async def search_devices(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchDevicesResponseTypeDef:
         """
         Searches for devices using the specified filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_devices)
         """
 
     async def search_jobs(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchJobsResponseTypeDef:
         """
         Searches for Amazon Braket jobs that match the specified filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_jobs)
         """
 
     async def search_quantum_tasks(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuantumTasksResponseTypeDef:
         """
         Searches for tasks that match the specified filter values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Client.search_quantum_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/client/#search_quantum_tasks)
         """
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/literals.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AssociationTypeType",
     "CancellationStatusType",
     "CompressionTypeType",
     "DeviceStatusType",
     "DeviceTypeType",
     "HybridJobAdditionalAttributeNameType",
@@ -42,15 +41,14 @@
     "BraketServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssociationTypeType = Literal["RESERVATION_TIME_WINDOW_ARN"]
 CancellationStatusType = Literal["CANCELLED", "CANCELLING"]
 CompressionTypeType = Literal["GZIP", "NONE"]
 DeviceStatusType = Literal["OFFLINE", "ONLINE", "RETIRED"]
 DeviceTypeType = Literal["QPU", "SIMULATOR"]
 HybridJobAdditionalAttributeNameType = Literal["QueueInfo"]
 InstanceTypeType = Literal[
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/literals.pyi` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/paginator.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     SearchJobsResponseTypeDef,
     SearchQuantumTasksFilterTypeDef,
     SearchQuantumTasksResponseTypeDef,
 )
 
 __all__ = ("SearchDevicesPaginator", "SearchJobsPaginator", "SearchQuantumTasksPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
         """
 
 
@@ -77,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
         """
 
 
@@ -95,13 +94,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/paginator.pyi` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchdevicespaginator)
         """
 
 class SearchJobsPaginator(AioPaginator):
@@ -73,15 +73,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchjobspaginator)
         """
 
 class SearchQuantumTasksPaginator(AioPaginator):
@@ -90,13 +90,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/type_defs.py` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/type_defs.py`

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
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "AssociationTypeDef",
     "CancelJobRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket/type_defs.pyi` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/PKG-INFO` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-braket
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Braket 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Braket 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/
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
 
 <a id="types-aiobotocore-braket"></a>
 
 # types-aiobotocore-braket
 
 [![PyPI - types-aiobotocore-braket](https://img.shields.io/pypi/v/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-braket.svg?color=blue)](https://pypi.org/project/types-aiobotocore-braket)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-braket)](https://pepy.tech/project/types-aiobotocore-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Braket 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[aiobotocore.Braket 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [types-aiobotocore-braket docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_braket/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-braket-2.9.0/types_aiobotocore_braket.egg-info/SOURCES.txt` & `types-aiobotocore-braket-2.9.1/types_aiobotocore_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

