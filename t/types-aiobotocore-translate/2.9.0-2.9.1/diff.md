# Comparing `tmp/types-aiobotocore-translate-2.9.0.tar.gz` & `tmp/types-aiobotocore-translate-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-translate-2.9.0.tar", last modified: Wed Dec 13 20:00:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-translate-2.9.1.tar", last modified: Thu Jan 18 01:21:59 2024, max compression
```

## Comparing `types-aiobotocore-translate-2.9.0.tar` & `types-aiobotocore-translate-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.633034 types-aiobotocore-translate-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2023-12-13 20:00:42.633034 types-aiobotocore-translate-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11479 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:42.633034 types-aiobotocore-translate-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.629034 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18192 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18188 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:30.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:42.633034 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13050 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:42.000000 types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.880984 types-aiobotocore-translate-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-01-18 01:21:59.880984 types-aiobotocore-translate-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11479 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:59.880984 types-aiobotocore-translate-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.880984 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18199 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18196 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-01-18 01:18:56.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-01-18 01:18:56.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:55.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.880984 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13070 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:59.000000 types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-translate-2.9.0/LICENSE` & `types-aiobotocore-translate-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-translate-2.9.0/PKG-INFO` & `types-aiobotocore-translate-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Translate 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Translate 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
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
 
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-translate-2.9.0/README.md` & `types-aiobotocore-translate-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-translate-2.9.0/setup.py` & `types-aiobotocore-translate-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-translate",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_translate"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Translate 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Translate 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore translate type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_translate": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__init__.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import TranslateClient
 from .paginator import ListTerminologiesPaginator
 
 Client = TranslateClient
 
-
 __all__ = ("Client", "ListTerminologiesPaginator", "TranslateClient")
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__init__.pyi` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/__main__.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Translate 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Translate 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate\nOther"
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

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/client.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TranslateClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -125,15 +124,15 @@
         self,
         *,
         Name: str,
         ParallelDataConfig: ParallelDataConfigTypeDef,
         ClientToken: str,
         Description: str = ...,
         EncryptionKey: EncryptionKeyTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateParallelDataResponseTypeDef:
         """
         Creates a parallel data resource in Amazon Translate by importing an input file
         from Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.create_parallel_data)
@@ -205,15 +204,15 @@
         self,
         *,
         Name: str,
         MergeStrategy: Literal["OVERWRITE"],
         TerminologyData: TerminologyDataTypeDef,
         Description: str = ...,
         EncryptionKey: EncryptionKeyTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportTerminologyResponseTypeDef:
         """
         Creates or updates a custom terminology, depending on whether one already
         exists for the given terminology
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.import_terminology)
@@ -221,15 +220,15 @@
         """
 
     async def list_languages(
         self,
         *,
         DisplayLanguageCode: DisplayLanguageCodeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguagesResponseTypeDef:
         """
         Provides a list of languages (RFC-5646 codes and names) that Amazon Translate
         supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_languages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#list_languages)
@@ -266,15 +265,15 @@
         """
 
     async def list_text_translation_jobs(
         self,
         *,
         Filter: TextTranslationJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTextTranslationJobsResponseTypeDef:
         """
         Gets a list of the batch translation jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_text_translation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#list_text_translation_jobs)
         """
@@ -287,15 +286,15 @@
         DataAccessRoleArn: str,
         SourceLanguageCode: str,
         TargetLanguageCodes: Sequence[str],
         ClientToken: str,
         JobName: str = ...,
         TerminologyNames: Sequence[str] = ...,
         ParallelDataNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> StartTextTranslationJobResponseTypeDef:
         """
         Starts an asynchronous batch translation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.start_text_translation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#start_text_translation_job)
         """
@@ -321,15 +320,15 @@
     async def translate_document(
         self,
         *,
         Document: DocumentTypeDef,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> TranslateDocumentResponseTypeDef:
         """
         Translates the input document from the source language to the target language.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#translate_document)
         """
@@ -337,15 +336,15 @@
     async def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> TranslateTextResponseTypeDef:
         """
         Translates input text from the source language to the target language.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#translate_text)
         """
@@ -360,15 +359,15 @@
 
     async def update_parallel_data(
         self,
         *,
         Name: str,
         ParallelDataConfig: ParallelDataConfigTypeDef,
         ClientToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateParallelDataResponseTypeDef:
         """
         Updates a previously created parallel data resource by importing a new input
         file from Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.update_parallel_data)
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/client.pyi` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         self,
         *,
         Name: str,
         ParallelDataConfig: ParallelDataConfigTypeDef,
         ClientToken: str,
         Description: str = ...,
         EncryptionKey: EncryptionKeyTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateParallelDataResponseTypeDef:
         """
         Creates a parallel data resource in Amazon Translate by importing an input file
         from Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.create_parallel_data)
@@ -201,15 +201,15 @@
         self,
         *,
         Name: str,
         MergeStrategy: Literal["OVERWRITE"],
         TerminologyData: TerminologyDataTypeDef,
         Description: str = ...,
         EncryptionKey: EncryptionKeyTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportTerminologyResponseTypeDef:
         """
         Creates or updates a custom terminology, depending on whether one already
         exists for the given terminology
         name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.import_terminology)
@@ -217,15 +217,15 @@
         """
 
     async def list_languages(
         self,
         *,
         DisplayLanguageCode: DisplayLanguageCodeType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguagesResponseTypeDef:
         """
         Provides a list of languages (RFC-5646 codes and names) that Amazon Translate
         supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_languages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#list_languages)
@@ -262,15 +262,15 @@
         """
 
     async def list_text_translation_jobs(
         self,
         *,
         Filter: TextTranslationJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTextTranslationJobsResponseTypeDef:
         """
         Gets a list of the batch translation jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.list_text_translation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#list_text_translation_jobs)
         """
@@ -283,15 +283,15 @@
         DataAccessRoleArn: str,
         SourceLanguageCode: str,
         TargetLanguageCodes: Sequence[str],
         ClientToken: str,
         JobName: str = ...,
         TerminologyNames: Sequence[str] = ...,
         ParallelDataNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> StartTextTranslationJobResponseTypeDef:
         """
         Starts an asynchronous batch translation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.start_text_translation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#start_text_translation_job)
         """
@@ -317,15 +317,15 @@
     async def translate_document(
         self,
         *,
         Document: DocumentTypeDef,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> TranslateDocumentResponseTypeDef:
         """
         Translates the input document from the source language to the target language.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#translate_document)
         """
@@ -333,15 +333,15 @@
     async def translate_text(
         self,
         *,
         Text: str,
         SourceLanguageCode: str,
         TargetLanguageCode: str,
         TerminologyNames: Sequence[str] = ...,
-        Settings: TranslationSettingsTypeDef = ...
+        Settings: TranslationSettingsTypeDef = ...,
     ) -> TranslateTextResponseTypeDef:
         """
         Translates input text from the source language to the target language.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.translate_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/client/#translate_text)
         """
@@ -356,15 +356,15 @@
 
     async def update_parallel_data(
         self,
         *,
         Name: str,
         ParallelDataConfig: ParallelDataConfigTypeDef,
         ClientToken: str,
-        Description: str = ...
+        Description: str = ...,
     ) -> UpdateParallelDataResponseTypeDef:
         """
         Updates a previously created parallel data resource by importing a new input
         file from Amazon
         S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate.Client.update_parallel_data)
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/literals.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/literals.py`

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
     "BrevityType",
     "DirectionalityType",
     "DisplayLanguageCodeType",
     "EncryptionKeyTypeType",
     "FormalityType",
     "JobStatusType",
@@ -36,15 +35,14 @@
     "TranslateServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BrevityType = Literal["ON"]
 DirectionalityType = Literal["MULTI", "UNI"]
 DisplayLanguageCodeType = Literal["de", "en", "es", "fr", "it", "ja", "ko", "pt", "zh", "zh-TW"]
 EncryptionKeyTypeType = Literal["KMS"]
 FormalityType = Literal["FORMAL", "INFORMAL"]
 JobStatusType = Literal[
     "COMPLETED",
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/literals.pyi` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/paginator.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListTerminologiesResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListTerminologiesPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/paginator.pyi` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/type_defs.py` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TermTypeDef",
     "BlobTypeDef",
     "EncryptionKeyTypeDef",
     "ParallelDataConfigTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate/type_defs.pyi` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/PKG-INFO` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-translate
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Translate 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Translate 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/
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
 
 <a id="types-aiobotocore-translate"></a>
 
 # types-aiobotocore-translate
 
 [![PyPI - types-aiobotocore-translate](https://img.shields.io/pypi/v/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-translate.svg?color=blue)](https://pypi.org/project/types-aiobotocore-translate)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-translate)](https://pepy.tech/project/types-aiobotocore-translate)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Translate 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
+[aiobotocore.Translate 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#Translate)
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
 [types-aiobotocore-translate docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_translate/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-translate-2.9.0/types_aiobotocore_translate.egg-info/SOURCES.txt` & `types-aiobotocore-translate-2.9.1/types_aiobotocore_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

