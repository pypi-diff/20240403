# Comparing `tmp/types-aiobotocore-cleanrooms-2.9.0.tar.gz` & `tmp/types-aiobotocore-cleanrooms-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cleanrooms-2.9.0.tar", last modified: Wed Dec 13 19:58:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-cleanrooms-2.9.1.tar", last modified: Thu Jan 18 01:20:13 2024, max compression
```

## Comparing `types-aiobotocore-cleanrooms-2.9.0.tar` & `types-aiobotocore-cleanrooms-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.969993 types-aiobotocore-cleanrooms-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2023-12-13 19:58:46.969993 types-aiobotocore-cleanrooms-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14331 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:46.969993 types-aiobotocore-cleanrooms-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.969993 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55551 2023-12-13 19:42:09.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    55547 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13493 2023-12-13 19:42:09.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13491 2023-12-13 19:42:09.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20401 2023-12-13 19:42:09.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20383 2023-12-13 19:42:09.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    68470 2023-12-13 19:42:11.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    68469 2023-12-13 19:42:10.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:08.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:46.969993 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15913 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:46.000000 types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.937472 types-aiobotocore-cleanrooms-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-01-18 01:20:13.937472 types-aiobotocore-cleanrooms-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14331 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:13.937472 types-aiobotocore-cleanrooms-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.937472 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55572 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55569 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13491 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20404 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20388 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    68469 2024-01-18 01:04:08.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68469 2024-01-18 01:04:07.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:06.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:13.937472 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15933 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:13.000000 types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/LICENSE` & `types-aiobotocore-cleanrooms-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cleanrooms-2.9.0/PKG-INFO` & `types-aiobotocore-cleanrooms-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
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
 
 <a id="types-aiobotocore-cleanrooms"></a>
 
 # types-aiobotocore-cleanrooms
 
 [![PyPI - types-aiobotocore-cleanrooms](https://img.shields.io/pypi/v/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/README.md` & `types-aiobotocore-cleanrooms-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/setup.py` & `types-aiobotocore-cleanrooms-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cleanrooms",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cleanrooms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CleanRoomsService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CleanRoomsService 2.9.1 service generated with"
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
     keywords="aiobotocore cleanrooms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cleanrooms": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__init__.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     ListPrivacyBudgetTemplatesPaginator,
     ListProtectedQueriesPaginator,
     ListSchemasPaginator,
 )
 
 Client = CleanRoomsServiceClient
 
-
 __all__ = (
     "CleanRoomsServiceClient",
     "Client",
     "ListAnalysisTemplatesPaginator",
     "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationConfiguredAudienceModelAssociationsPaginator",
     "ListCollaborationPrivacyBudgetTemplatesPaginator",
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__init__.pyi` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/__main__.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CleanRoomsService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CleanRoomsService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService\nOther"
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

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/client.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CleanRoomsServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -205,15 +204,15 @@
         *,
         membershipIdentifier: str,
         name: str,
         format: Literal["SQL"],
         source: AnalysisSourceTypeDef,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...
+        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...,
     ) -> CreateAnalysisTemplateOutputTypeDef:
         """
         Creates a new analysis template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_analysis_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_analysis_template)
         """
@@ -225,15 +224,15 @@
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
         creatorDisplayName: str,
         queryLogStatus: CollaborationQueryLogStatusType,
         dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        creatorPaymentConfiguration: PaymentConfigurationTypeDef = ...
+        creatorPaymentConfiguration: PaymentConfigurationTypeDef = ...,
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_collaboration)
         """
@@ -242,15 +241,15 @@
         self,
         *,
         membershipIdentifier: str,
         configuredAudienceModelArn: str,
         configuredAudienceModelAssociationName: str,
         manageResourcePolicies: bool,
         tags: Mapping[str, str] = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateConfiguredAudienceModelAssociationOutputTypeDef:
         """
         Provides the details necessary to create a configured audience model
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_audience_model_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_audience_model_association)
@@ -260,29 +259,29 @@
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
 
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -291,15 +290,15 @@
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_association)
         """
@@ -307,15 +306,15 @@
     async def create_membership(
         self,
         *,
         collaborationIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType,
         tags: Mapping[str, str] = ...,
         defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,
-        paymentConfiguration: MembershipPaymentConfigurationTypeDef = ...
+        paymentConfiguration: MembershipPaymentConfigurationTypeDef = ...,
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_membership)
@@ -324,15 +323,15 @@
     async def create_privacy_budget_template(
         self,
         *,
         membershipIdentifier: str,
         autoRefresh: PrivacyBudgetTemplateAutoRefreshType,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         parameters: PrivacyBudgetTemplateParametersInputTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreatePrivacyBudgetTemplateOutputTypeDef:
         """
         Creates a privacy budget template for a specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_privacy_budget_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_privacy_budget_template)
         """
@@ -374,15 +373,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table)
         """
 
     async def delete_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
-        analysisRuleType: ConfiguredTableAnalysisRuleTypeType
+        analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
     ) -> Dict[str, Any]:
         """
         Deletes a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_analysis_rule)
         """
@@ -509,15 +508,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table)
         """
 
     async def get_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
-        analysisRuleType: ConfiguredTableAnalysisRuleTypeType
+        analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
     ) -> GetConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Retrieves a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_analysis_rule)
         """
@@ -623,30 +622,30 @@
 
     async def list_collaboration_privacy_budgets(
         self,
         *,
         collaborationIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCollaborationPrivacyBudgetsOutputTypeDef:
         """
         Returns an array that summarizes each privacy budget in a specified
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaboration_privacy_budgets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaboration_privacy_budgets)
         """
 
     async def list_collaborations(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        memberStatus: FilterableMemberStatusType = ...
+        memberStatus: FilterableMemberStatusType = ...,
     ) -> ListCollaborationsOutputTypeDef:
         """
         Lists collaborations the caller owns, is active in, or has been invited to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaborations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaborations)
         """
@@ -714,15 +713,15 @@
 
     async def list_privacy_budgets(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPrivacyBudgetsOutputTypeDef:
         """
         Returns detailed information about the privacy budgets in a specified
         membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_privacy_budgets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_privacy_budgets)
@@ -730,30 +729,30 @@
 
     async def list_protected_queries(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListProtectedQueriesOutputTypeDef:
         """
         Lists protected queries, sorted by the most recent query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_protected_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_protected_queries)
         """
 
     async def list_schemas(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSchemasOutputTypeDef:
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_schemas)
         """
@@ -780,15 +779,15 @@
 
     async def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
-        resultConfiguration: ProtectedQueryResultConfigurationTypeDef = ...
+        resultConfiguration: ProtectedQueryResultConfigurationTypeDef = ...,
     ) -> StartProtectedQueryOutputTypeDef:
         """
         Creates a protected query that is started by Clean Rooms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#start_protected_query)
         """
@@ -832,15 +831,15 @@
 
     async def update_configured_audience_model_association(
         self,
         *,
         configuredAudienceModelAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateConfiguredAudienceModelAssociationOutputTypeDef:
         """
         Provides the details necessary to update a configured audience model
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_audience_model_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_audience_model_association)
@@ -857,73 +856,73 @@
         """
 
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
 
     async def update_configured_table_association(
         self,
         *,
         configuredTableAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateConfiguredTableAssociationOutputTypeDef:
         """
         Updates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_association)
         """
 
     async def update_membership(
         self,
         *,
         membershipIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType = ...,
-        defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...
+        defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,
     ) -> UpdateMembershipOutputTypeDef:
         """
         Updates a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_membership)
         """
 
     async def update_privacy_budget_template(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetTemplateIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        parameters: PrivacyBudgetTemplateUpdateParametersTypeDef = ...
+        parameters: PrivacyBudgetTemplateUpdateParametersTypeDef = ...,
     ) -> UpdatePrivacyBudgetTemplateOutputTypeDef:
         """
         Updates the privacy budget template for the specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_privacy_budget_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_privacy_budget_template)
         """
 
     async def update_protected_query(
         self,
         *,
         membershipIdentifier: str,
         protectedQueryIdentifier: str,
-        targetStatus: Literal["CANCELLED"]
+        targetStatus: Literal["CANCELLED"],
     ) -> UpdateProtectedQueryOutputTypeDef:
         """
         Updates the processing of a currently running query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_protected_query)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/client.pyi` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         *,
         membershipIdentifier: str,
         name: str,
         format: Literal["SQL"],
         source: AnalysisSourceTypeDef,
         description: str = ...,
         tags: Mapping[str, str] = ...,
-        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...
+        analysisParameters: Sequence[AnalysisParameterTypeDef] = ...,
     ) -> CreateAnalysisTemplateOutputTypeDef:
         """
         Creates a new analysis template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_analysis_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_analysis_template)
         """
@@ -221,15 +221,15 @@
         name: str,
         description: str,
         creatorMemberAbilities: Sequence[MemberAbilityType],
         creatorDisplayName: str,
         queryLogStatus: CollaborationQueryLogStatusType,
         dataEncryptionMetadata: DataEncryptionMetadataTypeDef = ...,
         tags: Mapping[str, str] = ...,
-        creatorPaymentConfiguration: PaymentConfigurationTypeDef = ...
+        creatorPaymentConfiguration: PaymentConfigurationTypeDef = ...,
     ) -> CreateCollaborationOutputTypeDef:
         """
         Creates a new collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_collaboration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_collaboration)
         """
@@ -238,15 +238,15 @@
         self,
         *,
         membershipIdentifier: str,
         configuredAudienceModelArn: str,
         configuredAudienceModelAssociationName: str,
         manageResourcePolicies: bool,
         tags: Mapping[str, str] = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateConfiguredAudienceModelAssociationOutputTypeDef:
         """
         Provides the details necessary to create a configured audience model
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_audience_model_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_audience_model_association)
@@ -256,29 +256,29 @@
         self,
         *,
         name: str,
         tableReference: TableReferenceTypeDef,
         allowedColumns: Sequence[str],
         analysisMethod: Literal["DIRECT_QUERY"],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredTableOutputTypeDef:
         """
         Creates a new configured table resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table)
         """
 
     async def create_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,
     ) -> CreateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Creates a new analysis rule for a configured table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_analysis_rule)
         """
@@ -287,15 +287,15 @@
         self,
         *,
         name: str,
         membershipIdentifier: str,
         configuredTableIdentifier: str,
         roleArn: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateConfiguredTableAssociationOutputTypeDef:
         """
         Creates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_configured_table_association)
         """
@@ -303,15 +303,15 @@
     async def create_membership(
         self,
         *,
         collaborationIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType,
         tags: Mapping[str, str] = ...,
         defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,
-        paymentConfiguration: MembershipPaymentConfigurationTypeDef = ...
+        paymentConfiguration: MembershipPaymentConfigurationTypeDef = ...,
     ) -> CreateMembershipOutputTypeDef:
         """
         Creates a membership for a specific collaboration identifier and joins the
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_membership)
@@ -320,15 +320,15 @@
     async def create_privacy_budget_template(
         self,
         *,
         membershipIdentifier: str,
         autoRefresh: PrivacyBudgetTemplateAutoRefreshType,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         parameters: PrivacyBudgetTemplateParametersInputTypeDef,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreatePrivacyBudgetTemplateOutputTypeDef:
         """
         Creates a privacy budget template for a specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.create_privacy_budget_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#create_privacy_budget_template)
         """
@@ -370,15 +370,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table)
         """
 
     async def delete_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
-        analysisRuleType: ConfiguredTableAnalysisRuleTypeType
+        analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
     ) -> Dict[str, Any]:
         """
         Deletes a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.delete_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#delete_configured_table_analysis_rule)
         """
@@ -505,15 +505,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table)
         """
 
     async def get_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
-        analysisRuleType: ConfiguredTableAnalysisRuleTypeType
+        analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
     ) -> GetConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Retrieves a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.get_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#get_configured_table_analysis_rule)
         """
@@ -619,30 +619,30 @@
 
     async def list_collaboration_privacy_budgets(
         self,
         *,
         collaborationIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCollaborationPrivacyBudgetsOutputTypeDef:
         """
         Returns an array that summarizes each privacy budget in a specified
         collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaboration_privacy_budgets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaboration_privacy_budgets)
         """
 
     async def list_collaborations(
         self,
         *,
         nextToken: str = ...,
         maxResults: int = ...,
-        memberStatus: FilterableMemberStatusType = ...
+        memberStatus: FilterableMemberStatusType = ...,
     ) -> ListCollaborationsOutputTypeDef:
         """
         Lists collaborations the caller owns, is active in, or has been invited to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_collaborations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_collaborations)
         """
@@ -710,15 +710,15 @@
 
     async def list_privacy_budgets(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListPrivacyBudgetsOutputTypeDef:
         """
         Returns detailed information about the privacy budgets in a specified
         membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_privacy_budgets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_privacy_budgets)
@@ -726,30 +726,30 @@
 
     async def list_protected_queries(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListProtectedQueriesOutputTypeDef:
         """
         Lists protected queries, sorted by the most recent query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_protected_queries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_protected_queries)
         """
 
     async def list_schemas(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> ListSchemasOutputTypeDef:
         """
         Lists the schemas for relations within a collaboration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.list_schemas)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#list_schemas)
         """
@@ -776,15 +776,15 @@
 
     async def start_protected_query(
         self,
         *,
         type: Literal["SQL"],
         membershipIdentifier: str,
         sqlParameters: ProtectedQuerySQLParametersTypeDef,
-        resultConfiguration: ProtectedQueryResultConfigurationTypeDef = ...
+        resultConfiguration: ProtectedQueryResultConfigurationTypeDef = ...,
     ) -> StartProtectedQueryOutputTypeDef:
         """
         Creates a protected query that is started by Clean Rooms.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.start_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#start_protected_query)
         """
@@ -828,15 +828,15 @@
 
     async def update_configured_audience_model_association(
         self,
         *,
         configuredAudienceModelAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
-        name: str = ...
+        name: str = ...,
     ) -> UpdateConfiguredAudienceModelAssociationOutputTypeDef:
         """
         Provides the details necessary to update a configured audience model
         association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_audience_model_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_audience_model_association)
@@ -853,73 +853,73 @@
         """
 
     async def update_configured_table_analysis_rule(
         self,
         *,
         configuredTableIdentifier: str,
         analysisRuleType: ConfiguredTableAnalysisRuleTypeType,
-        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef
+        analysisRulePolicy: ConfiguredTableAnalysisRulePolicyTypeDef,
     ) -> UpdateConfiguredTableAnalysisRuleOutputTypeDef:
         """
         Updates a configured table analysis rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_analysis_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_analysis_rule)
         """
 
     async def update_configured_table_association(
         self,
         *,
         configuredTableAssociationIdentifier: str,
         membershipIdentifier: str,
         description: str = ...,
-        roleArn: str = ...
+        roleArn: str = ...,
     ) -> UpdateConfiguredTableAssociationOutputTypeDef:
         """
         Updates a configured table association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_configured_table_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_configured_table_association)
         """
 
     async def update_membership(
         self,
         *,
         membershipIdentifier: str,
         queryLogStatus: MembershipQueryLogStatusType = ...,
-        defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...
+        defaultResultConfiguration: MembershipProtectedQueryResultConfigurationTypeDef = ...,
     ) -> UpdateMembershipOutputTypeDef:
         """
         Updates a membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_membership)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_membership)
         """
 
     async def update_privacy_budget_template(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetTemplateIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        parameters: PrivacyBudgetTemplateUpdateParametersTypeDef = ...
+        parameters: PrivacyBudgetTemplateUpdateParametersTypeDef = ...,
     ) -> UpdatePrivacyBudgetTemplateOutputTypeDef:
         """
         Updates the privacy budget template for the specified membership.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_privacy_budget_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_privacy_budget_template)
         """
 
     async def update_protected_query(
         self,
         *,
         membershipIdentifier: str,
         protectedQueryIdentifier: str,
-        targetStatus: Literal["CANCELLED"]
+        targetStatus: Literal["CANCELLED"],
     ) -> UpdateProtectedQueryOutputTypeDef:
         """
         Updates the processing of a currently running query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Client.update_protected_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/client/#update_protected_query)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/literals.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/literals.py`

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
     "AggregateFunctionNameType",
     "AggregationTypeType",
     "AnalysisFormatType",
     "AnalysisMethodType",
     "AnalysisRuleTypeType",
     "CollaborationQueryLogStatusType",
@@ -63,15 +62,14 @@
     "CleanRoomsServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AggregateFunctionNameType = Literal["AVG", "COUNT", "COUNT_DISTINCT", "SUM", "SUM_DISTINCT"]
 AggregationTypeType = Literal["COUNT_DISTINCT"]
 AnalysisFormatType = Literal["SQL"]
 AnalysisMethodType = Literal["DIRECT_QUERY"]
 AnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
 CollaborationQueryLogStatusType = Literal["DISABLED", "ENABLED"]
 ConfiguredTableAnalysisRuleTypeType = Literal["AGGREGATION", "CUSTOM", "LIST"]
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/literals.pyi` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/paginator.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListAnalysisTemplatesPaginator",
     "ListCollaborationAnalysisTemplatesPaginator",
     "ListCollaborationConfiguredAudienceModelAssociationsPaginator",
     "ListCollaborationPrivacyBudgetTemplatesPaginator",
     "ListCollaborationPrivacyBudgetsPaginator",
     "ListCollaborationsPaginator",
@@ -95,15 +94,14 @@
     "ListMembershipsPaginator",
     "ListPrivacyBudgetTemplatesPaginator",
     "ListPrivacyBudgetsPaginator",
     "ListProtectedQueriesPaginator",
     "ListSchemasPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -177,15 +175,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCollaborationPrivacyBudgetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationPrivacyBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationprivacybudgetspaginator)
         """
 
 
@@ -195,15 +193,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
 
@@ -304,15 +302,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrivacyBudgetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListPrivacyBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprivacybudgetspaginator)
         """
 
 
@@ -323,15 +321,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
 
@@ -342,13 +340,13 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/paginator.pyi` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCollaborationPrivacyBudgetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborationPrivacyBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationprivacybudgetspaginator)
         """
 
 class ListCollaborationsPaginator(AioPaginator):
@@ -186,15 +186,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
     """
 
     def paginate(
         self,
         *,
         memberStatus: FilterableMemberStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCollaborationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListCollaborations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listcollaborationspaginator)
         """
 
 class ListConfiguredAudienceModelAssociationsPaginator(AioPaginator):
@@ -288,15 +288,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         privacyBudgetType: Literal["DIFFERENTIAL_PRIVACY"],
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPrivacyBudgetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListPrivacyBudgets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprivacybudgetspaginator)
         """
 
 class ListProtectedQueriesPaginator(AioPaginator):
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         membershipIdentifier: str,
         status: ProtectedQueryStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProtectedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListProtectedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listprotectedqueriespaginator)
         """
 
 class ListSchemasPaginator(AioPaginator):
@@ -324,13 +324,13 @@
     """
 
     def paginate(
         self,
         *,
         collaborationIdentifier: str,
         schemaType: Literal["TABLE"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSchemasOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/paginators/#listschemaspaginator)
         """
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/type_defs.py` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AggregateColumnTypeDef",
     "AggregationConstraintTypeDef",
     "AnalysisParameterTypeDef",
     "AnalysisRuleListTypeDef",
     "AnalysisSchemaTypeDef",
     "AnalysisSourceTypeDef",
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms/type_defs.pyi` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/PKG-INFO` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cleanrooms
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CleanRoomsService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CleanRoomsService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/
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
 
 <a id="types-aiobotocore-cleanrooms"></a>
 
 # types-aiobotocore-cleanrooms
 
 [![PyPI - types-aiobotocore-cleanrooms](https://img.shields.io/pypi/v/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cleanrooms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cleanrooms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cleanrooms)](https://pepy.tech/project/types-aiobotocore-cleanrooms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CleanRoomsService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
+[aiobotocore.CleanRoomsService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#CleanRoomsService)
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
 [types-aiobotocore-cleanrooms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cleanrooms/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cleanrooms-2.9.0/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt` & `types-aiobotocore-cleanrooms-2.9.1/types_aiobotocore_cleanrooms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

