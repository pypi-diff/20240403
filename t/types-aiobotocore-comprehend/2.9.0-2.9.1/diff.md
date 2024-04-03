# Comparing `tmp/types-aiobotocore-comprehend-2.9.0.tar.gz` & `tmp/types-aiobotocore-comprehend-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehend-2.9.0.tar", last modified: Wed Dec 13 19:58:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehend-2.9.1.tar", last modified: Thu Jan 18 01:20:24 2024, max compression
```

## Comparing `types-aiobotocore-comprehend-2.9.0.tar` & `types-aiobotocore-comprehend-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.189903 types-aiobotocore-comprehend-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-13 19:58:58.185903 types-aiobotocore-comprehend-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13383 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:58.189903 types-aiobotocore-comprehend-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.185903 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71028 2023-12-13 19:43:10.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    71024 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2023-12-13 19:43:10.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15506 2023-12-13 19:43:10.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14324 2023-12-13 19:43:10.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    14312 2023-12-13 19:43:10.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   107469 2023-12-13 19:43:12.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   107468 2023-12-13 19:43:11.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:09.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.185903 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:58.000000 types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.233425 types-aiobotocore-comprehend-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-01-18 01:20:24.233425 types-aiobotocore-comprehend-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:24.233425 types-aiobotocore-comprehend-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.233425 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71059 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71056 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15506 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14332 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14321 2024-01-18 01:05:06.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   107468 2024-01-18 01:05:09.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   107468 2024-01-18 01:05:08.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:05.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.233425 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:24.000000 types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehend-2.9.0/LICENSE` & `types-aiobotocore-comprehend-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-comprehend-2.9.0/PKG-INFO` & `types-aiobotocore-comprehend-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehend
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Comprehend 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Comprehend 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
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
 
 <a id="types-aiobotocore-comprehend"></a>
 
 # types-aiobotocore-comprehend
 
 [![PyPI - types-aiobotocore-comprehend](https://img.shields.io/pypi/v/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Comprehend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[aiobotocore.Comprehend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehend-2.9.0/README.md` & `types-aiobotocore-comprehend-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Comprehend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[aiobotocore.Comprehend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehend-2.9.0/setup.py` & `types-aiobotocore-comprehend-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehend",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_comprehend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Comprehend 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Comprehend 2.9.1 service generated with"
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
     keywords="aiobotocore comprehend type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_comprehend": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__init__.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     ListPiiEntitiesDetectionJobsPaginator,
     ListSentimentDetectionJobsPaginator,
     ListTopicsDetectionJobsPaginator,
 )
 
 Client = ComprehendClient
 
-
 __all__ = (
     "Client",
     "ComprehendClient",
     "ListDocumentClassificationJobsPaginator",
     "ListDocumentClassifiersPaginator",
     "ListDominantLanguageDetectionJobsPaginator",
     "ListEndpointsPaginator",
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__init__.pyi` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/__main__.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Comprehend 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Comprehend 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend\nOther"
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

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/client.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ComprehendClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -282,15 +281,15 @@
 
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a classification request to analyze a single document in real-time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
         """
@@ -321,15 +320,15 @@
         *,
         FlywheelArn: str,
         DatasetName: str,
         InputDataConfig: DatasetInputDataConfigTypeDef,
         DatasetType: DatasetTypeType = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a dataset to upload training or test data for a model associated with a
         flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_dataset)
@@ -346,15 +345,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
-        ModelPolicy: str = ...
+        ModelPolicy: str = ...,
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_document_classifier)
         """
@@ -364,15 +363,15 @@
         *,
         EndpointName: str,
         DesiredInferenceUnits: int,
         ModelArn: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataAccessRoleArn: str = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates a model-specific endpoint for synchronous inference for a previously
         trained custom model For information about endpoints, see [Managing
         endpoints](https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_endpoint)
@@ -388,15 +387,15 @@
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         ModelKmsKeyId: str = ...,
-        ModelPolicy: str = ...
+        ModelPolicy: str = ...,
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_entity_recognizer)
         """
@@ -408,15 +407,15 @@
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
         TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
         DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity
         recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
@@ -636,15 +635,15 @@
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
@@ -734,15 +733,15 @@
         self,
         *,
         SourceModelArn: str,
         ModelName: str = ...,
         VersionName: str = ...,
         ModelKmsKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportModelResponseTypeDef:
         """
         Creates a new custom model that replicates a source custom model that you
         import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.import_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#import_model)
@@ -750,29 +749,29 @@
 
     async def list_datasets(
         self,
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatasetsResponseTypeDef:
         """
         List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_datasets)
         """
 
     async def list_document_classification_jobs(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentClassificationJobsResponseTypeDef:
         """
         Gets a list of the documentation classification jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classification_jobs)
         """
@@ -790,29 +789,29 @@
         """
 
     async def list_document_classifiers(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentClassifiersResponseTypeDef:
         """
         Gets a list of the document classifiers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifiers)
         """
 
     async def list_dominant_language_detection_jobs(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDominantLanguageDetectionJobsResponseTypeDef:
         """
         Gets a list of the dominant language detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_dominant_language_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_dominant_language_detection_jobs)
         """
@@ -828,15 +827,15 @@
         """
 
     async def list_entities_detection_jobs(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entities_detection_jobs)
         """
@@ -852,15 +851,15 @@
         """
 
     async def list_entity_recognizers(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntityRecognizersResponseTypeDef:
         """
         Gets a list of the properties of all entity recognizers that you created,
         including recognizers currently in
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizers)
@@ -868,30 +867,30 @@
         """
 
     async def list_events_detection_jobs(
         self,
         *,
         Filter: EventsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEventsDetectionJobsResponseTypeDef:
         """
         Gets a list of the events detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_events_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_events_detection_jobs)
         """
 
     async def list_flywheel_iteration_history(
         self,
         *,
         FlywheelArn: str,
         Filter: FlywheelIterationFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlywheelIterationHistoryResponseTypeDef:
         """
         Information about the history of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheel_iteration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheel_iteration_history)
         """
@@ -907,43 +906,43 @@
         """
 
     async def list_key_phrases_detection_jobs(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListKeyPhrasesDetectionJobsResponseTypeDef:
         """
         Get a list of key phrase detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_key_phrases_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_key_phrases_detection_jobs)
         """
 
     async def list_pii_entities_detection_jobs(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPiiEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the PII entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_pii_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_pii_entities_detection_jobs)
         """
 
     async def list_sentiment_detection_jobs(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_sentiment_detection_jobs)
         """
@@ -959,29 +958,29 @@
         """
 
     async def list_targeted_sentiment_detection_jobs(
         self,
         *,
         Filter: TargetedSentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTargetedSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of targeted sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_targeted_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_targeted_sentiment_detection_jobs)
         """
 
     async def list_topics_detection_jobs(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTopicsDetectionJobsResponseTypeDef:
         """
         Gets a list of the topic detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_topics_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_topics_detection_jobs)
         """
@@ -1004,15 +1003,15 @@
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job using a custom
         classification
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
@@ -1025,15 +1024,15 @@
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
@@ -1048,15 +1047,15 @@
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
@@ -1067,15 +1066,15 @@
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartEventsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous event detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_events_detection_job)
         """
@@ -1099,15 +1098,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
@@ -1119,15 +1118,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         RedactionConfig: RedactionConfigTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
@@ -1139,15 +1138,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
@@ -1159,15 +1158,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
@@ -1180,15 +1179,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
         """
@@ -1300,30 +1299,30 @@
     async def update_endpoint(
         self,
         *,
         EndpointArn: str,
         DesiredModelArn: str = ...,
         DesiredInferenceUnits: int = ...,
         DesiredDataAccessRoleArn: str = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> UpdateEndpointResponseTypeDef:
         """
         Updates information about the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_endpoint)
         """
 
     async def update_flywheel(
         self,
         *,
         FlywheelArn: str,
         ActiveModelArn: str = ...,
         DataAccessRoleArn: str = ...,
-        DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...
+        DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...,
     ) -> UpdateFlywheelResponseTypeDef:
         """
         Update the configuration information for an existing flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_flywheel)
         """
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/client.pyi` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
 
     async def classify_document(
         self,
         *,
         EndpointArn: str,
         Text: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,
     ) -> ClassifyDocumentResponseTypeDef:
         """
         Creates a classification request to analyze a single document in real-time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#classify_document)
         """
@@ -317,15 +317,15 @@
         *,
         FlywheelArn: str,
         DatasetName: str,
         InputDataConfig: DatasetInputDataConfigTypeDef,
         DatasetType: DatasetTypeType = ...,
         Description: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a dataset to upload training or test data for a model associated with a
         flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_dataset)
@@ -342,15 +342,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Mode: DocumentClassifierModeType = ...,
         ModelKmsKeyId: str = ...,
-        ModelPolicy: str = ...
+        ModelPolicy: str = ...,
     ) -> CreateDocumentClassifierResponseTypeDef:
         """
         Creates a new document classifier that you can use to categorize documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_document_classifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_document_classifier)
         """
@@ -360,15 +360,15 @@
         *,
         EndpointName: str,
         DesiredInferenceUnits: int,
         ModelArn: str = ...,
         ClientRequestToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataAccessRoleArn: str = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> CreateEndpointResponseTypeDef:
         """
         Creates a model-specific endpoint for synchronous inference for a previously
         trained custom model For information about endpoints, see [Managing
         endpoints](https://docs.aws.amazon.com/comprehend/latest/dg/manage-endpoints.html).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_endpoint)
@@ -384,15 +384,15 @@
         LanguageCode: LanguageCodeType,
         VersionName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         ModelKmsKeyId: str = ...,
-        ModelPolicy: str = ...
+        ModelPolicy: str = ...,
     ) -> CreateEntityRecognizerResponseTypeDef:
         """
         Creates an entity recognizer using submitted files.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#create_entity_recognizer)
         """
@@ -404,15 +404,15 @@
         DataAccessRoleArn: str,
         DataLakeS3Uri: str,
         ActiveModelArn: str = ...,
         TaskConfig: TaskConfigTypeDef = ...,
         ModelType: ModelTypeType = ...,
         DataSecurityConfig: DataSecurityConfigTypeDef = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlywheelResponseTypeDef:
         """
         A flywheel is an Amazon Web Services resource that orchestrates the ongoing
         training of a model for custom classification or custom entity
         recognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)
@@ -632,15 +632,15 @@
     async def detect_entities(
         self,
         *,
         Text: str = ...,
         LanguageCode: LanguageCodeType = ...,
         EndpointArn: str = ...,
         Bytes: BlobTypeDef = ...,
-        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...
+        DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,
     ) -> DetectEntitiesResponseTypeDef:
         """
         Detects named entities in input text when you use the pre-trained model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#detect_entities)
         """
@@ -730,15 +730,15 @@
         self,
         *,
         SourceModelArn: str,
         ModelName: str = ...,
         VersionName: str = ...,
         ModelKmsKeyId: str = ...,
         DataAccessRoleArn: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportModelResponseTypeDef:
         """
         Creates a new custom model that replicates a source custom model that you
         import.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.import_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#import_model)
@@ -746,29 +746,29 @@
 
     async def list_datasets(
         self,
         *,
         FlywheelArn: str = ...,
         Filter: DatasetFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatasetsResponseTypeDef:
         """
         List the datasets that you have configured in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_datasets)
         """
 
     async def list_document_classification_jobs(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentClassificationJobsResponseTypeDef:
         """
         Gets a list of the documentation classification jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classification_jobs)
         """
@@ -786,29 +786,29 @@
         """
 
     async def list_document_classifiers(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDocumentClassifiersResponseTypeDef:
         """
         Gets a list of the document classifiers that you have created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_document_classifiers)
         """
 
     async def list_dominant_language_detection_jobs(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDominantLanguageDetectionJobsResponseTypeDef:
         """
         Gets a list of the dominant language detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_dominant_language_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_dominant_language_detection_jobs)
         """
@@ -824,15 +824,15 @@
         """
 
     async def list_entities_detection_jobs(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_entities_detection_jobs)
         """
@@ -848,15 +848,15 @@
         """
 
     async def list_entity_recognizers(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntityRecognizersResponseTypeDef:
         """
         Gets a list of the properties of all entity recognizers that you created,
         including recognizers currently in
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizers)
@@ -864,30 +864,30 @@
         """
 
     async def list_events_detection_jobs(
         self,
         *,
         Filter: EventsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEventsDetectionJobsResponseTypeDef:
         """
         Gets a list of the events detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_events_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_events_detection_jobs)
         """
 
     async def list_flywheel_iteration_history(
         self,
         *,
         FlywheelArn: str,
         Filter: FlywheelIterationFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlywheelIterationHistoryResponseTypeDef:
         """
         Information about the history of a flywheel iteration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheel_iteration_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_flywheel_iteration_history)
         """
@@ -903,43 +903,43 @@
         """
 
     async def list_key_phrases_detection_jobs(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListKeyPhrasesDetectionJobsResponseTypeDef:
         """
         Get a list of key phrase detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_key_phrases_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_key_phrases_detection_jobs)
         """
 
     async def list_pii_entities_detection_jobs(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPiiEntitiesDetectionJobsResponseTypeDef:
         """
         Gets a list of the PII entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_pii_entities_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_pii_entities_detection_jobs)
         """
 
     async def list_sentiment_detection_jobs(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_sentiment_detection_jobs)
         """
@@ -955,29 +955,29 @@
         """
 
     async def list_targeted_sentiment_detection_jobs(
         self,
         *,
         Filter: TargetedSentimentDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTargetedSentimentDetectionJobsResponseTypeDef:
         """
         Gets a list of targeted sentiment detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_targeted_sentiment_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_targeted_sentiment_detection_jobs)
         """
 
     async def list_topics_detection_jobs(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTopicsDetectionJobsResponseTypeDef:
         """
         Gets a list of the topic detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_topics_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#list_topics_detection_jobs)
         """
@@ -1000,15 +1000,15 @@
         DataAccessRoleArn: str,
         JobName: str = ...,
         DocumentClassifierArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> StartDocumentClassificationJobResponseTypeDef:
         """
         Starts an asynchronous document classification job using a custom
         classification
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)
@@ -1021,15 +1021,15 @@
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartDominantLanguageDetectionJobResponseTypeDef:
         """
         Starts an asynchronous dominant language detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_dominant_language_detection_job)
@@ -1044,15 +1044,15 @@
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         EntityRecognizerArn: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> StartEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_entities_detection_job)
         """
@@ -1063,15 +1063,15 @@
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         TargetEventTypes: Sequence[str],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartEventsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous event detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_events_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_events_detection_job)
         """
@@ -1095,15 +1095,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartKeyPhrasesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous key phrase detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_key_phrases_detection_job)
         """
@@ -1115,15 +1115,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         Mode: PiiEntitiesDetectionModeType,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         RedactionConfig: RedactionConfigTypeDef = ...,
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartPiiEntitiesDetectionJobResponseTypeDef:
         """
         Starts an asynchronous PII entity detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_pii_entities_detection_job)
         """
@@ -1135,15 +1135,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous sentiment detection job for a collection of documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_sentiment_detection_job)
         """
@@ -1155,15 +1155,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: LanguageCodeType,
         JobName: str = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartTargetedSentimentDetectionJobResponseTypeDef:
         """
         Starts an asynchronous targeted sentiment detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_targeted_sentiment_detection_job)
@@ -1176,15 +1176,15 @@
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         JobName: str = ...,
         NumberOfTopics: int = ...,
         ClientRequestToken: str = ...,
         VolumeKmsKeyId: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartTopicsDetectionJobResponseTypeDef:
         """
         Starts an asynchronous topic detection job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#start_topics_detection_job)
         """
@@ -1296,30 +1296,30 @@
     async def update_endpoint(
         self,
         *,
         EndpointArn: str,
         DesiredModelArn: str = ...,
         DesiredInferenceUnits: int = ...,
         DesiredDataAccessRoleArn: str = ...,
-        FlywheelArn: str = ...
+        FlywheelArn: str = ...,
     ) -> UpdateEndpointResponseTypeDef:
         """
         Updates information about the specified endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_endpoint)
         """
 
     async def update_flywheel(
         self,
         *,
         FlywheelArn: str,
         ActiveModelArn: str = ...,
         DataAccessRoleArn: str = ...,
-        DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...
+        DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...,
     ) -> UpdateFlywheelResponseTypeDef:
         """
         Update the configuration information for an existing flywheel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_flywheel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/client/#update_flywheel)
         """
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/literals.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/literals.py`

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
     "AugmentedManifestsDocumentTypeFormatType",
     "BlockTypeType",
     "DatasetDataFormatType",
     "DatasetStatusType",
     "DatasetTypeType",
     "DocumentClassifierDataFormatType",
@@ -68,15 +67,14 @@
     "ComprehendServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AugmentedManifestsDocumentTypeFormatType = Literal[
     "PLAIN_TEXT_DOCUMENT", "SEMI_STRUCTURED_DOCUMENT"
 ]
 BlockTypeType = Literal["LINE", "WORD"]
 DatasetDataFormatType = Literal["AUGMENTED_MANIFEST", "COMPREHEND_CSV"]
 DatasetStatusType = Literal["COMPLETED", "CREATING", "FAILED"]
 DatasetTypeType = Literal["TEST", "TRAIN"]
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/literals.pyi` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/paginator.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     "ListEntityRecognizersPaginator",
     "ListKeyPhrasesDetectionJobsPaginator",
     "ListPiiEntitiesDetectionJobsPaginator",
     "ListSentimentDetectionJobsPaginator",
     "ListTopicsDetectionJobsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -98,15 +97,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentClassificationJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 
@@ -116,15 +115,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentClassifiersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 
@@ -134,15 +133,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDominantLanguageDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 
@@ -167,15 +166,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 
@@ -185,15 +184,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntityRecognizersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 
@@ -203,15 +202,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 
@@ -221,15 +220,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 
@@ -239,15 +238,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSentimentDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 
@@ -257,13 +256,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTopicsDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/paginator.pyi` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassificationJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentClassificationJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassificationjobspaginator)
         """
 
 class ListDocumentClassifiersPaginator(AioPaginator):
@@ -112,15 +112,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DocumentClassifierFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDocumentClassifiersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDocumentClassifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdocumentclassifierspaginator)
         """
 
 class ListDominantLanguageDetectionJobsPaginator(AioPaginator):
@@ -129,15 +129,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: DominantLanguageDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDominantLanguageDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListDominantLanguageDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listdominantlanguagedetectionjobspaginator)
         """
 
 class ListEndpointsPaginator(AioPaginator):
@@ -160,15 +160,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentitiesdetectionjobspaginator)
         """
 
 class ListEntityRecognizersPaginator(AioPaginator):
@@ -177,15 +177,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: EntityRecognizerFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntityRecognizersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListEntityRecognizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listentityrecognizerspaginator)
         """
 
 class ListKeyPhrasesDetectionJobsPaginator(AioPaginator):
@@ -194,15 +194,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListKeyPhrasesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListKeyPhrasesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listkeyphrasesdetectionjobspaginator)
         """
 
 class ListPiiEntitiesDetectionJobsPaginator(AioPaginator):
@@ -211,15 +211,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPiiEntitiesDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListPiiEntitiesDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listpiientitiesdetectionjobspaginator)
         """
 
 class ListSentimentDetectionJobsPaginator(AioPaginator):
@@ -228,15 +228,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: SentimentDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSentimentDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListSentimentDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listsentimentdetectionjobspaginator)
         """
 
 class ListTopicsDetectionJobsPaginator(AioPaginator):
@@ -245,13 +245,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filter: TopicsDetectionJobFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTopicsDetectionJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Paginator.ListTopicsDetectionJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/paginators/#listtopicsdetectionjobspaginator)
         """
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/type_defs.py` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AugmentedManifestsListItemPaginatorTypeDef",
     "AugmentedManifestsListItemTypeDef",
     "DominantLanguageTypeDef",
     "BatchDetectDominantLanguageRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend/type_defs.pyi` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/PKG-INFO` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehend
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Comprehend 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Comprehend 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/
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
 
 <a id="types-aiobotocore-comprehend"></a>
 
 # types-aiobotocore-comprehend
 
 [![PyPI - types-aiobotocore-comprehend](https://img.shields.io/pypi/v/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehend.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehend)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehend)](https://pepy.tech/project/types-aiobotocore-comprehend)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Comprehend 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
+[aiobotocore.Comprehend 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
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
 [types-aiobotocore-comprehend docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehend/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehend-2.9.0/types_aiobotocore_comprehend.egg-info/SOURCES.txt` & `types-aiobotocore-comprehend-2.9.1/types_aiobotocore_comprehend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

