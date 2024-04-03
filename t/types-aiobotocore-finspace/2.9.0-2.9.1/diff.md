# Comparing `tmp/types-aiobotocore-finspace-2.9.0.tar.gz` & `tmp/types-aiobotocore-finspace-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-finspace-2.9.0.tar", last modified: Wed Dec 13 19:59:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-finspace-2.9.1.tar", last modified: Thu Jan 18 01:20:43 2024, max compression
```

## Comparing `types-aiobotocore-finspace-2.9.0.tar` & `types-aiobotocore-finspace-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.037747 types-aiobotocore-finspace-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2023-12-13 19:59:19.033747 types-aiobotocore-finspace-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:19.037747 types-aiobotocore-finspace-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.033747 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37129 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37125 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11367 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    47686 2023-12-13 19:46:12.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    47685 2023-12-13 19:46:11.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:09.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:19.033747 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13057 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:19.000000 types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.525329 types-aiobotocore-finspace-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-01-18 01:20:43.525329 types-aiobotocore-finspace-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:43.525329 types-aiobotocore-finspace-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.525329 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37145 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37142 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    47685 2024-01-18 01:08:06.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47685 2024-01-18 01:08:05.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:04.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:43.525329 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13077 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:43.000000 types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-finspace-2.9.0/LICENSE` & `types-aiobotocore-finspace-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-finspace-2.9.0/PKG-INFO` & `types-aiobotocore-finspace-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.finspace 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.finspace 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
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
 
 <a id="types-aiobotocore-finspace"></a>
 
 # types-aiobotocore-finspace
 
 [![PyPI - types-aiobotocore-finspace](https://img.shields.io/pypi/v/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-2.9.0/README.md` & `types-aiobotocore-finspace-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-2.9.0/setup.py` & `types-aiobotocore-finspace-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-finspace",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.finspace 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.finspace 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore finspace type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_finspace": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__init__.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import finspaceClient
 from .paginator import ListKxEnvironmentsPaginator
 
 Client = finspaceClient
 
-
 __all__ = ("Client", "ListKxEnvironmentsPaginator", "finspaceClient")
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__init__.pyi` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/__main__.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.finspace 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.finspace 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/client.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("finspaceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -152,30 +151,30 @@
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
         federationParameters: FederationParametersTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
-        dataBundles: Sequence[str] = ...
+        dataBundles: Sequence[str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_environment)
         """
 
     async def create_kx_changeset(
         self,
         *,
         environmentId: str,
         databaseName: str,
         changeRequests: Sequence[ChangeRequestTypeDef],
-        clientToken: str
+        clientToken: str,
     ) -> CreateKxChangesetResponseTypeDef:
         """
         Creates a changeset for a kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_changeset)
         """
@@ -199,15 +198,15 @@
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...,
-        scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef = ...
+        scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef = ...,
     ) -> CreateKxClusterResponseTypeDef:
         """
         Creates a new kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_cluster)
         """
@@ -215,15 +214,15 @@
     async def create_kx_database(
         self,
         *,
         environmentId: str,
         databaseName: str,
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxDatabaseResponseTypeDef:
         """
         Creates a new kdb database in the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_database)
         """
@@ -237,15 +236,15 @@
         azMode: KxAzModeType,
         clientToken: str,
         availabilityZoneId: str = ...,
         changesetId: str = ...,
         segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...,
         autoUpdate: bool = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxDataviewResponseTypeDef:
         """
         Creates a snapshot of kdb database with tiered storage capabilities and a
         pre-warmed cache, ready for mounting on kdb
         clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_dataview)
@@ -255,15 +254,15 @@
     async def create_kx_environment(
         self,
         *,
         name: str,
         kmsKeyId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateKxEnvironmentResponseTypeDef:
         """
         Creates a managed kdb environment for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_environment)
         """
@@ -272,15 +271,15 @@
         self,
         *,
         clientToken: str,
         environmentId: str,
         scalingGroupName: str,
         hostType: str,
         availabilityZoneId: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxScalingGroupResponseTypeDef:
         """
         Creates a new scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_scaling_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_scaling_group)
         """
@@ -288,15 +287,15 @@
     async def create_kx_user(
         self,
         *,
         environmentId: str,
         userName: str,
         iamRole: str,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateKxUserResponseTypeDef:
         """
         Creates a user in FinSpace kdb environment with an associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_user)
         """
@@ -308,15 +307,15 @@
         volumeType: Literal["NAS_1"],
         volumeName: str,
         azMode: KxAzModeType,
         availabilityZoneIds: Sequence[str],
         clientToken: str = ...,
         description: str = ...,
         nas1Configuration: KxNAS1ConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxVolumeResponseTypeDef:
         """
         Creates a new volume with a specific amount of throughput and storage capacity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_volume)
         """
@@ -539,15 +538,15 @@
 
     async def list_kx_clusters(
         self,
         *,
         environmentId: str,
         clusterType: KxClusterTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListKxClustersResponseTypeDef:
         """
         Returns a list of clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#list_kx_clusters)
         """
@@ -604,15 +603,15 @@
 
     async def list_kx_volumes(
         self,
         *,
         environmentId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        volumeType: Literal["NAS_1"] = ...
+        volumeType: Literal["NAS_1"] = ...,
     ) -> ListKxVolumesResponseTypeDef:
         """
         Lists all the volumes in a kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#list_kx_volumes)
         """
@@ -646,15 +645,15 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: FederationParametersTypeDef = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
@@ -664,15 +663,15 @@
         *,
         environmentId: str,
         clusterName: str,
         code: CodeConfigurationTypeDef,
         clientToken: str = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
-        deploymentConfiguration: KxClusterCodeDeploymentConfigurationTypeDef = ...
+        deploymentConfiguration: KxClusterCodeDeploymentConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Allows you to update code configuration on a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_code_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_cluster_code_configuration)
         """
@@ -680,15 +679,15 @@
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
         databases: Sequence[KxDatabaseConfigurationTypeDef],
         clientToken: str = ...,
-        deploymentConfiguration: KxDeploymentConfigurationTypeDef = ...
+        deploymentConfiguration: KxDeploymentConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the
         `changesetId` and all the dbPaths to be
         cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
@@ -710,15 +709,15 @@
         *,
         environmentId: str,
         databaseName: str,
         dataviewName: str,
         clientToken: str,
         description: str = ...,
         changesetId: str = ...,
-        segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...
+        segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...,
     ) -> UpdateKxDataviewResponseTypeDef:
         """
         Updates the specified dataview.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_dataview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_dataview)
         """
@@ -735,15 +734,15 @@
 
     async def update_kx_environment_network(
         self,
         *,
         environmentId: str,
         transitGatewayConfiguration: TransitGatewayConfigurationTypeDef = ...,
         customDNSConfiguration: Sequence[CustomDNSServerTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateKxEnvironmentNetworkResponseTypeDef:
         """
         Updates environment network to connect to your internal network by using a
         transit
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment_network)
@@ -763,15 +762,15 @@
     async def update_kx_volume(
         self,
         *,
         environmentId: str,
         volumeName: str,
         description: str = ...,
         clientToken: str = ...,
-        nas1Configuration: KxNAS1ConfigurationTypeDef = ...
+        nas1Configuration: KxNAS1ConfigurationTypeDef = ...,
     ) -> UpdateKxVolumeResponseTypeDef:
         """
         Updates the throughput or capacity of a volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_volume)
         """
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/client.pyi` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -148,30 +148,30 @@
         name: str,
         description: str = ...,
         kmsKeyId: str = ...,
         tags: Mapping[str, str] = ...,
         federationMode: FederationModeType = ...,
         federationParameters: FederationParametersTypeDef = ...,
         superuserParameters: SuperuserParametersTypeDef = ...,
-        dataBundles: Sequence[str] = ...
+        dataBundles: Sequence[str] = ...,
     ) -> CreateEnvironmentResponseTypeDef:
         """
         Create a new FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_environment)
         """
 
     async def create_kx_changeset(
         self,
         *,
         environmentId: str,
         databaseName: str,
         changeRequests: Sequence[ChangeRequestTypeDef],
-        clientToken: str
+        clientToken: str,
     ) -> CreateKxChangesetResponseTypeDef:
         """
         Creates a changeset for a kdb database.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_changeset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_changeset)
         """
@@ -195,15 +195,15 @@
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
         code: CodeConfigurationTypeDef = ...,
         executionRole: str = ...,
         savedownStorageConfiguration: KxSavedownStorageConfigurationTypeDef = ...,
         availabilityZoneId: str = ...,
         tags: Mapping[str, str] = ...,
-        scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef = ...
+        scalingGroupConfiguration: KxScalingGroupConfigurationTypeDef = ...,
     ) -> CreateKxClusterResponseTypeDef:
         """
         Creates a new kdb cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_cluster)
         """
@@ -211,15 +211,15 @@
     async def create_kx_database(
         self,
         *,
         environmentId: str,
         databaseName: str,
         clientToken: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxDatabaseResponseTypeDef:
         """
         Creates a new kdb database in the environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_database)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_database)
         """
@@ -233,15 +233,15 @@
         azMode: KxAzModeType,
         clientToken: str,
         availabilityZoneId: str = ...,
         changesetId: str = ...,
         segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...,
         autoUpdate: bool = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxDataviewResponseTypeDef:
         """
         Creates a snapshot of kdb database with tiered storage capabilities and a
         pre-warmed cache, ready for mounting on kdb
         clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_dataview)
@@ -251,15 +251,15 @@
     async def create_kx_environment(
         self,
         *,
         name: str,
         kmsKeyId: str,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateKxEnvironmentResponseTypeDef:
         """
         Creates a managed kdb environment for the account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_environment)
         """
@@ -268,15 +268,15 @@
         self,
         *,
         clientToken: str,
         environmentId: str,
         scalingGroupName: str,
         hostType: str,
         availabilityZoneId: str,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxScalingGroupResponseTypeDef:
         """
         Creates a new scaling group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_scaling_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_scaling_group)
         """
@@ -284,15 +284,15 @@
     async def create_kx_user(
         self,
         *,
         environmentId: str,
         userName: str,
         iamRole: str,
         tags: Mapping[str, str] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateKxUserResponseTypeDef:
         """
         Creates a user in FinSpace kdb environment with an associated IAM role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_user)
         """
@@ -304,15 +304,15 @@
         volumeType: Literal["NAS_1"],
         volumeName: str,
         azMode: KxAzModeType,
         availabilityZoneIds: Sequence[str],
         clientToken: str = ...,
         description: str = ...,
         nas1Configuration: KxNAS1ConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKxVolumeResponseTypeDef:
         """
         Creates a new volume with a specific amount of throughput and storage capacity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.create_kx_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#create_kx_volume)
         """
@@ -535,15 +535,15 @@
 
     async def list_kx_clusters(
         self,
         *,
         environmentId: str,
         clusterType: KxClusterTypeType = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListKxClustersResponseTypeDef:
         """
         Returns a list of clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#list_kx_clusters)
         """
@@ -600,15 +600,15 @@
 
     async def list_kx_volumes(
         self,
         *,
         environmentId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        volumeType: Literal["NAS_1"] = ...
+        volumeType: Literal["NAS_1"] = ...,
     ) -> ListKxVolumesResponseTypeDef:
         """
         Lists all the volumes in a kdb environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.list_kx_volumes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#list_kx_volumes)
         """
@@ -642,15 +642,15 @@
     async def update_environment(
         self,
         *,
         environmentId: str,
         name: str = ...,
         description: str = ...,
         federationMode: FederationModeType = ...,
-        federationParameters: FederationParametersTypeDef = ...
+        federationParameters: FederationParametersTypeDef = ...,
     ) -> UpdateEnvironmentResponseTypeDef:
         """
         Update your FinSpace environment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_environment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_environment)
         """
@@ -660,15 +660,15 @@
         *,
         environmentId: str,
         clusterName: str,
         code: CodeConfigurationTypeDef,
         clientToken: str = ...,
         initializationScript: str = ...,
         commandLineArguments: Sequence[KxCommandLineArgumentTypeDef] = ...,
-        deploymentConfiguration: KxClusterCodeDeploymentConfigurationTypeDef = ...
+        deploymentConfiguration: KxClusterCodeDeploymentConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Allows you to update code configuration on a running cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_code_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_cluster_code_configuration)
         """
@@ -676,15 +676,15 @@
     async def update_kx_cluster_databases(
         self,
         *,
         environmentId: str,
         clusterName: str,
         databases: Sequence[KxDatabaseConfigurationTypeDef],
         clientToken: str = ...,
-        deploymentConfiguration: KxDeploymentConfigurationTypeDef = ...
+        deploymentConfiguration: KxDeploymentConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the databases mounted on a kdb cluster, which includes the
         `changesetId` and all the dbPaths to be
         cached.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_cluster_databases)
@@ -706,15 +706,15 @@
         *,
         environmentId: str,
         databaseName: str,
         dataviewName: str,
         clientToken: str,
         description: str = ...,
         changesetId: str = ...,
-        segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...
+        segmentConfigurations: Sequence[KxDataviewSegmentConfigurationTypeDef] = ...,
     ) -> UpdateKxDataviewResponseTypeDef:
         """
         Updates the specified dataview.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_dataview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_dataview)
         """
@@ -731,15 +731,15 @@
 
     async def update_kx_environment_network(
         self,
         *,
         environmentId: str,
         transitGatewayConfiguration: TransitGatewayConfigurationTypeDef = ...,
         customDNSConfiguration: Sequence[CustomDNSServerTypeDef] = ...,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> UpdateKxEnvironmentNetworkResponseTypeDef:
         """
         Updates environment network to connect to your internal network by using a
         transit
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_environment_network)
@@ -759,15 +759,15 @@
     async def update_kx_volume(
         self,
         *,
         environmentId: str,
         volumeName: str,
         description: str = ...,
         clientToken: str = ...,
-        nas1Configuration: KxNAS1ConfigurationTypeDef = ...
+        nas1Configuration: KxNAS1ConfigurationTypeDef = ...,
     ) -> UpdateKxVolumeResponseTypeDef:
         """
         Updates the throughput or capacity of a volume.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Client.update_kx_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/client/#update_kx_volume)
         """
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/literals.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/literals.py`

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
     "AutoScalingMetricType",
     "ChangeTypeType",
     "ChangesetStatusType",
     "EnvironmentStatusType",
     "ErrorDetailsType",
     "FederationModeType",
@@ -47,15 +46,14 @@
     "finspaceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AutoScalingMetricType = Literal["CPU_UTILIZATION_PERCENTAGE"]
 ChangeTypeType = Literal["DELETE", "PUT"]
 ChangesetStatusType = Literal["COMPLETED", "FAILED", "PENDING", "PROCESSING"]
 EnvironmentStatusType = Literal[
     "CREATED",
     "CREATE_REQUESTED",
     "CREATING",
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/literals.pyi` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/paginator.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListKxEnvironmentsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListKxEnvironmentsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/paginator.pyi` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/type_defs.py` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AutoScalingConfigurationTypeDef",
     "CapacityConfigurationTypeDef",
     "ChangeRequestTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace/type_defs.pyi` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/PKG-INFO` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-finspace
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.finspace 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.finspace 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/
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
 
 <a id="types-aiobotocore-finspace"></a>
 
 # types-aiobotocore-finspace
 
 [![PyPI - types-aiobotocore-finspace](https://img.shields.io/pypi/v/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-finspace.svg?color=blue)](https://pypi.org/project/types-aiobotocore-finspace)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-finspace)](https://pepy.tech/project/types-aiobotocore-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.finspace 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[aiobotocore.finspace 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [types-aiobotocore-finspace docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_finspace/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-finspace-2.9.0/types_aiobotocore_finspace.egg-info/SOURCES.txt` & `types-aiobotocore-finspace-2.9.1/types_aiobotocore_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

