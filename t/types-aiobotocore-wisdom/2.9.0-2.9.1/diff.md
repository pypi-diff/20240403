# Comparing `tmp/types-aiobotocore-wisdom-2.9.0.tar.gz` & `tmp/types-aiobotocore-wisdom-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-wisdom-2.9.0.tar", last modified: Wed Dec 13 20:00:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-wisdom-2.9.1.tar", last modified: Thu Jan 18 01:22:02 2024, max compression
```

## Comparing `types-aiobotocore-wisdom-2.9.0.tar` & `types-aiobotocore-wisdom-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.005005 types-aiobotocore-wisdom-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2023-12-13 20:00:46.005005 types-aiobotocore-wisdom-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12809 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:46.005005 types-aiobotocore-wisdom-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.001005 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35601 2023-12-13 19:57:56.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    35597 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2023-12-13 19:57:57.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2023-12-13 19:57:56.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2023-12-13 19:57:56.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12603 2023-12-13 19:57:56.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    44416 2023-12-13 19:57:57.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44415 2023-12-13 19:57:57.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:53.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:46.001005 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14382 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 20:00:45.000000 types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.956970 types-aiobotocore-wisdom-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-01-18 01:22:02.956970 types-aiobotocore-wisdom-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12809 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:22:02.956970 types-aiobotocore-wisdom-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.956970 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35612 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35609 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12606 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-01-18 01:19:22.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44415 2024-01-18 01:19:21.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:19:20.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:22:02.956970 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:22:02.000000 types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-wisdom-2.9.0/LICENSE` & `types-aiobotocore-wisdom-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-wisdom-2.9.0/PKG-INFO` & `types-aiobotocore-wisdom-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
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
 
 <a id="types-aiobotocore-wisdom"></a>
 
 # types-aiobotocore-wisdom
 
 [![PyPI - types-aiobotocore-wisdom](https://img.shields.io/pypi/v/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wisdom-2.9.0/README.md` & `types-aiobotocore-wisdom-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wisdom-2.9.0/setup.py` & `types-aiobotocore-wisdom-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-wisdom",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_wisdom"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectWisdomService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ConnectWisdomService 2.9.1 service generated with"
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
     keywords="aiobotocore wisdom type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_wisdom": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__init__.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     SearchContentPaginator,
     SearchQuickResponsesPaginator,
     SearchSessionsPaginator,
 )
 
 Client = ConnectWisdomServiceClient
 
-
 __all__ = (
     "Client",
     "ConnectWisdomServiceClient",
     "ListAssistantAssociationsPaginator",
     "ListAssistantsPaginator",
     "ListContentsPaginator",
     "ListImportJobsPaginator",
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__init__.pyi` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/__main__.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectWisdomService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ConnectWisdomService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService\nOther"
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

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/client.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ConnectWisdomServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -144,15 +143,15 @@
         self,
         *,
         name: str,
         type: Literal["AGENT"],
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantResponseTypeDef:
         """
         Creates an Amazon Connect Wisdom assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_assistant)
         """
@@ -160,15 +159,15 @@
     async def create_assistant_association(
         self,
         *,
         assistantId: str,
         association: AssistantAssociationInputDataTypeDef,
         associationType: Literal["KNOWLEDGE_BASE"],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantAssociationResponseTypeDef:
         """
         Creates an association between an Amazon Connect Wisdom assistant and another
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_assistant_association)
@@ -180,15 +179,15 @@
         knowledgeBaseId: str,
         name: str,
         uploadId: str,
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
-        title: str = ...
+        title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
         Creates Wisdom content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_content)
         """
@@ -199,15 +198,15 @@
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         sourceConfiguration: SourceConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
         """
@@ -222,15 +221,15 @@
         clientToken: str = ...,
         contentType: str = ...,
         description: str = ...,
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
         Creates a Wisdom quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_quick_response)
         """
@@ -238,15 +237,15 @@
     async def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_session)
         """
@@ -503,15 +502,15 @@
 
     async def search_content(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchContentResponseTypeDef:
         """
         Searches for content in a specified knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_content)
         """
@@ -519,30 +518,30 @@
     async def search_quick_responses(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
         Searches existing Wisdom quick responses in a Wisdom knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_quick_responses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_quick_responses)
         """
 
     async def search_sessions(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchSessionsResponseTypeDef:
         """
         Searches for sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_sessions)
         """
@@ -561,15 +560,15 @@
         self,
         *,
         importJobType: Literal["QUICK_RESPONSES"],
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
-        metadata: Mapping[str, str] = ...
+        metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
         Start an asynchronous job to import Wisdom resources from an uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.start_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#start_import_job)
@@ -597,15 +596,15 @@
         contentId: str,
         knowledgeBaseId: str,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         removeOverrideLinkOutUri: bool = ...,
         revisionId: str = ...,
         title: str = ...,
-        uploadId: str = ...
+        uploadId: str = ...,
     ) -> UpdateContentResponseTypeDef:
         """
         Updates information about the content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#update_content)
         """
@@ -632,15 +631,15 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
-        shortcutKey: str = ...
+        shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
         Updates an existing Wisdom quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#update_quick_response)
         """
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/client.pyi` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
         self,
         *,
         name: str,
         type: Literal["AGENT"],
         clientToken: str = ...,
         description: str = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantResponseTypeDef:
         """
         Creates an Amazon Connect Wisdom assistant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_assistant)
         """
@@ -156,15 +156,15 @@
     async def create_assistant_association(
         self,
         *,
         assistantId: str,
         association: AssistantAssociationInputDataTypeDef,
         associationType: Literal["KNOWLEDGE_BASE"],
         clientToken: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAssistantAssociationResponseTypeDef:
         """
         Creates an association between an Amazon Connect Wisdom assistant and another
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_assistant_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_assistant_association)
@@ -176,15 +176,15 @@
         knowledgeBaseId: str,
         name: str,
         uploadId: str,
         clientToken: str = ...,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         tags: Mapping[str, str] = ...,
-        title: str = ...
+        title: str = ...,
     ) -> CreateContentResponseTypeDef:
         """
         Creates Wisdom content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_content)
         """
@@ -195,15 +195,15 @@
         knowledgeBaseType: KnowledgeBaseTypeType,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         renderingConfiguration: RenderingConfigurationTypeDef = ...,
         serverSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef = ...,
         sourceConfiguration: SourceConfigurationTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateKnowledgeBaseResponseTypeDef:
         """
         Creates a knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_knowledge_base)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_knowledge_base)
         """
@@ -218,15 +218,15 @@
         clientToken: str = ...,
         contentType: str = ...,
         description: str = ...,
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         shortcutKey: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateQuickResponseResponseTypeDef:
         """
         Creates a Wisdom quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_quick_response)
         """
@@ -234,15 +234,15 @@
     async def create_session(
         self,
         *,
         assistantId: str,
         name: str,
         clientToken: str = ...,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateSessionResponseTypeDef:
         """
         Creates a session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.create_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#create_session)
         """
@@ -499,15 +499,15 @@
 
     async def search_content(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchContentResponseTypeDef:
         """
         Searches for content in a specified knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_content)
         """
@@ -515,30 +515,30 @@
     async def search_quick_responses(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchQuickResponsesResponseTypeDef:
         """
         Searches existing Wisdom quick responses in a Wisdom knowledge base.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_quick_responses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_quick_responses)
         """
 
     async def search_sessions(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchSessionsResponseTypeDef:
         """
         Searches for sessions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.search_sessions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#search_sessions)
         """
@@ -557,15 +557,15 @@
         self,
         *,
         importJobType: Literal["QUICK_RESPONSES"],
         knowledgeBaseId: str,
         uploadId: str,
         clientToken: str = ...,
         externalSourceConfiguration: ExternalSourceConfigurationTypeDef = ...,
-        metadata: Mapping[str, str] = ...
+        metadata: Mapping[str, str] = ...,
     ) -> StartImportJobResponseTypeDef:
         """
         Start an asynchronous job to import Wisdom resources from an uploaded source
         file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.start_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#start_import_job)
@@ -593,15 +593,15 @@
         contentId: str,
         knowledgeBaseId: str,
         metadata: Mapping[str, str] = ...,
         overrideLinkOutUri: str = ...,
         removeOverrideLinkOutUri: bool = ...,
         revisionId: str = ...,
         title: str = ...,
-        uploadId: str = ...
+        uploadId: str = ...,
     ) -> UpdateContentResponseTypeDef:
         """
         Updates information about the content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#update_content)
         """
@@ -628,15 +628,15 @@
         groupingConfiguration: GroupingConfigurationTypeDef = ...,
         isActive: bool = ...,
         language: str = ...,
         name: str = ...,
         removeDescription: bool = ...,
         removeGroupingConfiguration: bool = ...,
         removeShortcutKey: bool = ...,
-        shortcutKey: str = ...
+        shortcutKey: str = ...,
     ) -> UpdateQuickResponseResponseTypeDef:
         """
         Updates an existing Wisdom quick response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Client.update_quick_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/client/#update_quick_response)
         """
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/literals.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/literals.py`

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
     "AssistantStatusType",
     "AssistantTypeType",
     "AssociationTypeType",
     "ContentStatusType",
     "ExternalSourceType",
     "FilterFieldType",
@@ -54,15 +53,14 @@
     "ConnectWisdomServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AssistantStatusType = Literal[
     "ACTIVE",
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "DELETED",
     "DELETE_FAILED",
     "DELETE_IN_PROGRESS",
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/literals.pyi` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/paginator.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     "ListQuickResponsesPaginator",
     "QueryAssistantPaginator",
     "SearchContentPaginator",
     "SearchQuickResponsesPaginator",
     "SearchSessionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -196,15 +195,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
         """
 
 
@@ -216,15 +215,15 @@
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickResponsesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchQuickResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchquickresponsespaginator)
         """
 
 
@@ -235,13 +234,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/paginator.pyi` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
     """
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchContentResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchContent.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchcontentpaginator)
         """
 
 class SearchQuickResponsesPaginator(AioPaginator):
@@ -205,15 +205,15 @@
 
     def paginate(
         self,
         *,
         knowledgeBaseId: str,
         searchExpression: QuickResponseSearchExpressionTypeDef,
         attributes: Mapping[str, str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchQuickResponsesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchQuickResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchquickresponsespaginator)
         """
 
 class SearchSessionsPaginator(AioPaginator):
@@ -223,13 +223,13 @@
     """
 
     def paginate(
         self,
         *,
         assistantId: str,
         searchExpression: SearchExpressionTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchSessionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService.Paginator.SearchSessions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/paginators/#searchsessionspaginator)
         """
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/type_defs.py` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/type_defs.py`

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
     "AppIntegrationsConfigurationPaginatorTypeDef",
     "AppIntegrationsConfigurationTypeDef",
     "AssistantAssociationInputDataTypeDef",
     "KnowledgeBaseAssociationDataTypeDef",
     "AssistantIntegrationConfigurationTypeDef",
     "ServerSideEncryptionConfigurationTypeDef",
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom/type_defs.pyi` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/PKG-INFO` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-wisdom
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConnectWisdomService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConnectWisdomService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/
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
 
 <a id="types-aiobotocore-wisdom"></a>
 
 # types-aiobotocore-wisdom
 
 [![PyPI - types-aiobotocore-wisdom](https://img.shields.io/pypi/v/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-wisdom.svg?color=blue)](https://pypi.org/project/types-aiobotocore-wisdom)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-wisdom)](https://pepy.tech/project/types-aiobotocore-wisdom)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectWisdomService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
+[aiobotocore.ConnectWisdomService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#ConnectWisdomService)
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
 [types-aiobotocore-wisdom docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_wisdom/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-wisdom-2.9.0/types_aiobotocore_wisdom.egg-info/SOURCES.txt` & `types-aiobotocore-wisdom-2.9.1/types_aiobotocore_wisdom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

