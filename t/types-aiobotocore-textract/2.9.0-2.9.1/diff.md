# Comparing `tmp/types-aiobotocore-textract-2.9.0.tar.gz` & `tmp/types-aiobotocore-textract-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-textract-2.9.0.tar", last modified: Wed Dec 13 20:00:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-textract-2.9.1.tar", last modified: Thu Jan 18 01:21:57 2024, max compression
```

## Comparing `types-aiobotocore-textract-2.9.0.tar` & `types-aiobotocore-textract-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.381053 types-aiobotocore-textract-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13163 2023-12-13 20:00:40.381053 types-aiobotocore-textract-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11596 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:40.381053 types-aiobotocore-textract-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.381053 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23269 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10370 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10368 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    29222 2023-12-13 19:57:20.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29221 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:16.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:40.381053 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13163 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 20:00:40.000000 types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.844993 types-aiobotocore-textract-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-01-18 01:21:57.844993 types-aiobotocore-textract-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11596 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:57.844993 types-aiobotocore-textract-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.844993 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23278 2024-01-18 01:18:47.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23275 2024-01-18 01:18:47.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-01-18 01:18:48.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-01-18 01:18:47.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-01-18 01:18:47.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-01-18 01:18:47.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    29221 2024-01-18 01:18:48.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29221 2024-01-18 01:18:48.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:43.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:57.844993 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:21:57.000000 types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-textract-2.9.0/LICENSE` & `types-aiobotocore-textract-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-textract-2.9.0/PKG-INFO` & `types-aiobotocore-textract-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-textract
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Textract 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Textract 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/
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
 
 <a id="types-aiobotocore-textract"></a>
 
 # types-aiobotocore-textract
 
 [![PyPI - types-aiobotocore-textract](https://img.shields.io/pypi/v/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Textract 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[aiobotocore.Textract 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-textract-2.9.0/README.md` & `types-aiobotocore-textract-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Textract 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[aiobotocore.Textract 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-textract-2.9.0/setup.py` & `types-aiobotocore-textract-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-textract",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_textract"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Textract 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Textract 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore textract type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_textract": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__init__.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import TextractClient
 from .paginator import ListAdaptersPaginator, ListAdapterVersionsPaginator
 
 Client = TextractClient
 
-
 __all__ = ("Client", "ListAdapterVersionsPaginator", "ListAdaptersPaginator", "TextractClient")
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__init__.pyi` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/__main__.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Textract 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Textract 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract\nOther"
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

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/client.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TextractClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -115,15 +114,15 @@
     async def analyze_document(
         self,
         *,
         Document: DocumentTypeDef,
         FeatureTypes: Sequence[FeatureTypeType],
         HumanLoopConfig: HumanLoopConfigTypeDef = ...,
         QueriesConfig: QueriesConfigTypeDef = ...,
-        AdaptersConfig: AdaptersConfigTypeDef = ...
+        AdaptersConfig: AdaptersConfigTypeDef = ...,
     ) -> AnalyzeDocumentResponseTypeDef:
         """
         Analyzes an input document for relationships between detected items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.analyze_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#analyze_document)
         """
@@ -168,15 +167,15 @@
         self,
         *,
         AdapterName: str,
         FeatureTypes: Sequence[FeatureTypeType],
         ClientRequestToken: str = ...,
         Description: str = ...,
         AutoUpdate: AutoUpdateType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAdapterResponseTypeDef:
         """
         Creates an adapter, which can be fine-tuned for enhanced performance on user
         provided
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.create_adapter)
@@ -187,15 +186,15 @@
         self,
         *,
         AdapterId: str,
         DatasetConfig: AdapterVersionDatasetConfigTypeDef,
         OutputConfig: OutputConfigTypeDef,
         ClientRequestToken: str = ...,
         KMSKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAdapterVersionResponseTypeDef:
         """
         Creates a new version of an adapter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.create_adapter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#create_adapter_version)
         """
@@ -329,30 +328,30 @@
     async def list_adapter_versions(
         self,
         *,
         AdapterId: str = ...,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAdapterVersionsResponseTypeDef:
         """
         List all version of an adapter that meet the specified filtration criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.list_adapter_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#list_adapter_versions)
         """
 
     async def list_adapters(
         self,
         *,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAdaptersResponseTypeDef:
         """
         Lists all adapters that match the specified filtration criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.list_adapters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#list_adapters)
         """
@@ -374,15 +373,15 @@
         FeatureTypes: Sequence[FeatureTypeType],
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
         KMSKeyId: str = ...,
         QueriesConfig: QueriesConfigTypeDef = ...,
-        AdaptersConfig: AdaptersConfigTypeDef = ...
+        AdaptersConfig: AdaptersConfigTypeDef = ...,
     ) -> StartDocumentAnalysisResponseTypeDef:
         """
         Starts the asynchronous analysis of an input document for relationships between
         detected items such as key-value pairs, tables, and selection
         elements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_analysis)
@@ -393,15 +392,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartDocumentTextDetectionResponseTypeDef:
         """
         Starts the asynchronous detection of text in a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#start_document_text_detection)
         """
@@ -410,15 +409,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartExpenseAnalysisResponseTypeDef:
         """
         Starts the asynchronous analysis of invoices or receipts for data like contact
         information, items purchased, and vendor
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_expense_analysis)
@@ -429,15 +428,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartLendingAnalysisResponseTypeDef:
         """
         Starts the classification and analysis of an input document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_lending_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#start_lending_analysis)
         """
@@ -460,15 +459,15 @@
 
     async def update_adapter(
         self,
         *,
         AdapterId: str,
         Description: str = ...,
         AdapterName: str = ...,
-        AutoUpdate: AutoUpdateType = ...
+        AutoUpdate: AutoUpdateType = ...,
     ) -> UpdateAdapterResponseTypeDef:
         """
         Update the configuration for an adapter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.update_adapter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#update_adapter)
         """
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/client.pyi` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
     async def analyze_document(
         self,
         *,
         Document: DocumentTypeDef,
         FeatureTypes: Sequence[FeatureTypeType],
         HumanLoopConfig: HumanLoopConfigTypeDef = ...,
         QueriesConfig: QueriesConfigTypeDef = ...,
-        AdaptersConfig: AdaptersConfigTypeDef = ...
+        AdaptersConfig: AdaptersConfigTypeDef = ...,
     ) -> AnalyzeDocumentResponseTypeDef:
         """
         Analyzes an input document for relationships between detected items.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.analyze_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#analyze_document)
         """
@@ -164,15 +164,15 @@
         self,
         *,
         AdapterName: str,
         FeatureTypes: Sequence[FeatureTypeType],
         ClientRequestToken: str = ...,
         Description: str = ...,
         AutoUpdate: AutoUpdateType = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAdapterResponseTypeDef:
         """
         Creates an adapter, which can be fine-tuned for enhanced performance on user
         provided
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.create_adapter)
@@ -183,15 +183,15 @@
         self,
         *,
         AdapterId: str,
         DatasetConfig: AdapterVersionDatasetConfigTypeDef,
         OutputConfig: OutputConfigTypeDef,
         ClientRequestToken: str = ...,
         KMSKeyId: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateAdapterVersionResponseTypeDef:
         """
         Creates a new version of an adapter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.create_adapter_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#create_adapter_version)
         """
@@ -325,30 +325,30 @@
     async def list_adapter_versions(
         self,
         *,
         AdapterId: str = ...,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAdapterVersionsResponseTypeDef:
         """
         List all version of an adapter that meet the specified filtration criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.list_adapter_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#list_adapter_versions)
         """
 
     async def list_adapters(
         self,
         *,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAdaptersResponseTypeDef:
         """
         Lists all adapters that match the specified filtration criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.list_adapters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#list_adapters)
         """
@@ -370,15 +370,15 @@
         FeatureTypes: Sequence[FeatureTypeType],
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
         KMSKeyId: str = ...,
         QueriesConfig: QueriesConfigTypeDef = ...,
-        AdaptersConfig: AdaptersConfigTypeDef = ...
+        AdaptersConfig: AdaptersConfigTypeDef = ...,
     ) -> StartDocumentAnalysisResponseTypeDef:
         """
         Starts the asynchronous analysis of an input document for relationships between
         detected items such as key-value pairs, tables, and selection
         elements.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_analysis)
@@ -389,15 +389,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartDocumentTextDetectionResponseTypeDef:
         """
         Starts the asynchronous detection of text in a document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_document_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#start_document_text_detection)
         """
@@ -406,15 +406,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartExpenseAnalysisResponseTypeDef:
         """
         Starts the asynchronous analysis of invoices or receipts for data like contact
         information, items purchased, and vendor
         names.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_expense_analysis)
@@ -425,15 +425,15 @@
         self,
         *,
         DocumentLocation: DocumentLocationTypeDef,
         ClientRequestToken: str = ...,
         JobTag: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         OutputConfig: OutputConfigTypeDef = ...,
-        KMSKeyId: str = ...
+        KMSKeyId: str = ...,
     ) -> StartLendingAnalysisResponseTypeDef:
         """
         Starts the classification and analysis of an input document.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.start_lending_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#start_lending_analysis)
         """
@@ -456,15 +456,15 @@
 
     async def update_adapter(
         self,
         *,
         AdapterId: str,
         Description: str = ...,
         AdapterName: str = ...,
-        AutoUpdate: AutoUpdateType = ...
+        AutoUpdate: AutoUpdateType = ...,
     ) -> UpdateAdapterResponseTypeDef:
         """
         Update the configuration for an adapter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Client.update_adapter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/client/#update_adapter)
         """
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/literals.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AdapterVersionStatusType",
     "AutoUpdateType",
     "BlockTypeType",
     "ContentClassifierType",
     "EntityTypeType",
     "FeatureTypeType",
@@ -37,15 +36,14 @@
     "TextractServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AdapterVersionStatusType = Literal[
     "ACTIVE", "AT_RISK", "CREATION_ERROR", "CREATION_IN_PROGRESS", "DEPRECATED"
 ]
 AutoUpdateType = Literal["DISABLED", "ENABLED"]
 BlockTypeType = Literal[
     "CELL",
     "KEY_VALUE_SET",
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/literals.pyi` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/paginator.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListAdapterVersionsResponseTypeDef,
     PaginatorConfigTypeDef,
     TimestampTypeDef,
 )
 
 __all__ = ("ListAdapterVersionsPaginator", "ListAdaptersPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -56,15 +55,15 @@
 
     def paginate(
         self,
         *,
         AdapterId: str = ...,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAdapterVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/paginators/#listadapterversionspaginator)
         """
 
 
@@ -75,13 +74,13 @@
     """
 
     def paginate(
         self,
         *,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAdaptersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/paginators/#listadapterspaginator)
         """
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/paginator.pyi` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     def paginate(
         self,
         *,
         AdapterId: str = ...,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAdapterVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapterVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/paginators/#listadapterversionspaginator)
         """
 
 class ListAdaptersPaginator(AioPaginator):
@@ -71,13 +71,13 @@
     """
 
     def paginate(
         self,
         *,
         AfterCreationTime: TimestampTypeDef = ...,
         BeforeCreationTime: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAdaptersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract.Paginator.ListAdapters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/paginators/#listadapterspaginator)
         """
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/type_defs.py` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/type_defs.py`

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
     "AdapterOverviewTypeDef",
     "AdapterTypeDef",
     "S3ObjectTypeDef",
     "EvaluationMetricTypeDef",
     "AdapterVersionOverviewTypeDef",
     "DocumentMetadataTypeDef",
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract/type_defs.pyi` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/PKG-INFO` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-textract
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Textract 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Textract 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/
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
 
 <a id="types-aiobotocore-textract"></a>
 
 # types-aiobotocore-textract
 
 [![PyPI - types-aiobotocore-textract](https://img.shields.io/pypi/v/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-textract.svg?color=blue)](https://pypi.org/project/types-aiobotocore-textract)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-textract)](https://pepy.tech/project/types-aiobotocore-textract)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Textract 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
+[aiobotocore.Textract 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#Textract)
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
 [types-aiobotocore-textract docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_textract/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-textract-2.9.0/types_aiobotocore_textract.egg-info/SOURCES.txt` & `types-aiobotocore-textract-2.9.1/types_aiobotocore_textract.egg-info/SOURCES.txt`

 * *Files identical despite different names*

