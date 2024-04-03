# Comparing `tmp/types-aiobotocore-transcribe-2.9.0.tar.gz` & `tmp/types-aiobotocore-transcribe-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transcribe-2.9.0.tar", last modified: Wed Dec 13 20:00:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-transcribe-2.9.1.tar", last modified: Thu Jan 18 01:21:59 2024, max compression
```

## Comparing `types-aiobotocore-transcribe-2.9.0.tar` & `types-aiobotocore-transcribe-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.861040 types-aiobotocore-transcribe-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2023-12-13 20:00:41.861040 types-aiobotocore-transcribe-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:41.861040 types-aiobotocore-transcribe-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.861040 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34850 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    34846 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42168 2023-12-13 19:57:24.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42167 2023-12-13 19:57:24.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:23.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:41.861040 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 20:00:41.000000 types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.192987 types-aiobotocore-transcribe-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-01-18 01:21:59.192987 types-aiobotocore-transcribe-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:59.192987 types-aiobotocore-transcribe-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.192987 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34866 2024-01-18 01:18:52.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34863 2024-01-18 01:18:52.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-01-18 01:18:52.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-01-18 01:18:52.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    42167 2024-01-18 01:18:53.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42167 2024-01-18 01:18:52.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:51.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:59.192987 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12475 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:21:59.000000 types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transcribe-2.9.0/LICENSE` & `types-aiobotocore-transcribe-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-transcribe-2.9.0/PKG-INFO` & `types-aiobotocore-transcribe-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TranscribeService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TranscribeService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
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
 
 <a id="types-aiobotocore-transcribe"></a>
 
 # types-aiobotocore-transcribe
 
 [![PyPI - types-aiobotocore-transcribe](https://img.shields.io/pypi/v/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transcribe-2.9.0/README.md` & `types-aiobotocore-transcribe-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transcribe-2.9.0/setup.py` & `types-aiobotocore-transcribe-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transcribe",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_transcribe"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.TranscribeService 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.TranscribeService 2.9.1 service generated with"
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
     keywords="aiobotocore transcribe type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_transcribe": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/__main__.py` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TranscribeService 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.TranscribeService 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService\nOther"
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

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/client.py` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TranscribeServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -158,30 +157,30 @@
     async def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_language_model)
         """
 
     async def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_medical_vocabulary)
         """
@@ -190,15 +189,15 @@
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_vocabulary)
         """
@@ -207,15 +206,15 @@
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_vocabulary_filter)
         """
@@ -418,75 +417,75 @@
 
     async def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_call_analytics_jobs)
         """
 
     async def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_language_models)
         """
 
     async def list_medical_scribe_jobs(
         self,
         *,
         Status: MedicalScribeJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalScribeJobsResponseTypeDef:
         """
         Provides a list of Medical Scribe jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_scribe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_scribe_jobs)
         """
 
     async def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_transcription_jobs)
         """
 
     async def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListMedicalVocabulariesResponseTypeDef:
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_vocabularies)
@@ -506,30 +505,30 @@
 
     async def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_transcription_jobs)
         """
 
     async def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_vocabularies)
         """
@@ -549,15 +548,15 @@
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
         Settings: CallAnalyticsJobSettingsTypeDef = ...,
-        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
+        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...,
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -571,15 +570,15 @@
         Media: MediaTypeDef,
         OutputBucketName: str,
         DataAccessRoleArn: str,
         Settings: MedicalScribeSettingsTypeDef,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         ChannelDefinitions: Sequence[MedicalScribeChannelDefinitionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalScribeJobResponseTypeDef:
         """
         Transcribes patient-clinician conversations and generates clinical notes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_scribe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#start_medical_scribe_job)
         """
@@ -596,15 +595,15 @@
         MediaSampleRateHertz: int = ...,
         MediaFormat: MediaFormatType = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: MedicalTranscriptionSettingTypeDef = ...,
         ContentIdentificationType: Literal["PHI"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
@@ -629,15 +628,15 @@
         ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...,
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
@@ -685,30 +684,30 @@
     async def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_vocabulary)
         """
 
     async def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyFilterResponseTypeDef:
         """
         Updates an existing custom vocabulary filter with a new list of words.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_vocabulary_filter)
         """
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/client.pyi` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -154,30 +154,30 @@
     async def create_language_model(
         self,
         *,
         LanguageCode: CLMLanguageCodeType,
         BaseModelName: BaseModelNameType,
         ModelName: str,
         InputDataConfig: InputDataConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLanguageModelResponseTypeDef:
         """
         Creates a new custom language model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_language_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_language_model)
         """
 
     async def create_medical_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         VocabularyFileUri: str,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMedicalVocabularyResponseTypeDef:
         """
         Creates a new custom medical vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_medical_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_medical_vocabulary)
         """
@@ -186,15 +186,15 @@
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyResponseTypeDef:
         """
         Creates a new custom vocabulary.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_vocabulary)
         """
@@ -203,15 +203,15 @@
         self,
         *,
         VocabularyFilterName: str,
         LanguageCode: LanguageCodeType,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> CreateVocabularyFilterResponseTypeDef:
         """
         Creates a new custom vocabulary filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.create_vocabulary_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#create_vocabulary_filter)
         """
@@ -414,75 +414,75 @@
 
     async def list_call_analytics_jobs(
         self,
         *,
         Status: CallAnalyticsJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListCallAnalyticsJobsResponseTypeDef:
         """
         Provides a list of Call Analytics jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_call_analytics_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_call_analytics_jobs)
         """
 
     async def list_language_models(
         self,
         *,
         StatusEquals: ModelStatusType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLanguageModelsResponseTypeDef:
         """
         Provides a list of custom language models that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_language_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_language_models)
         """
 
     async def list_medical_scribe_jobs(
         self,
         *,
         Status: MedicalScribeJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalScribeJobsResponseTypeDef:
         """
         Provides a list of Medical Scribe jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_scribe_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_scribe_jobs)
         """
 
     async def list_medical_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListMedicalTranscriptionJobsResponseTypeDef:
         """
         Provides a list of medical transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_transcription_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_transcription_jobs)
         """
 
     async def list_medical_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListMedicalVocabulariesResponseTypeDef:
         """
         Provides a list of custom medical vocabularies that match the specified
         criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_medical_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_medical_vocabularies)
@@ -502,30 +502,30 @@
 
     async def list_transcription_jobs(
         self,
         *,
         Status: TranscriptionJobStatusType = ...,
         JobNameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTranscriptionJobsResponseTypeDef:
         """
         Provides a list of transcription jobs that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_transcription_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_transcription_jobs)
         """
 
     async def list_vocabularies(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         StateEquals: VocabularyStateType = ...,
-        NameContains: str = ...
+        NameContains: str = ...,
     ) -> ListVocabulariesResponseTypeDef:
         """
         Provides a list of custom vocabularies that match the specified criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.list_vocabularies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#list_vocabularies)
         """
@@ -545,15 +545,15 @@
         *,
         CallAnalyticsJobName: str,
         Media: MediaTypeDef,
         OutputLocation: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         DataAccessRoleArn: str = ...,
         Settings: CallAnalyticsJobSettingsTypeDef = ...,
-        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...
+        ChannelDefinitions: Sequence[ChannelDefinitionTypeDef] = ...,
     ) -> StartCallAnalyticsJobResponseTypeDef:
         """
         Transcribes the audio from a customer service call and applies any additional
         Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_call_analytics_job)
@@ -567,15 +567,15 @@
         Media: MediaTypeDef,
         OutputBucketName: str,
         DataAccessRoleArn: str,
         Settings: MedicalScribeSettingsTypeDef,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         ChannelDefinitions: Sequence[MedicalScribeChannelDefinitionTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalScribeJobResponseTypeDef:
         """
         Transcribes patient-clinician conversations and generates clinical notes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_scribe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#start_medical_scribe_job)
         """
@@ -592,15 +592,15 @@
         MediaSampleRateHertz: int = ...,
         MediaFormat: MediaFormatType = ...,
         OutputKey: str = ...,
         OutputEncryptionKMSKeyId: str = ...,
         KMSEncryptionContext: Mapping[str, str] = ...,
         Settings: MedicalTranscriptionSettingTypeDef = ...,
         ContentIdentificationType: Literal["PHI"] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> StartMedicalTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a medical dictation or conversation and applies any
         additional Request Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_medical_transcription_job)
@@ -625,15 +625,15 @@
         ContentRedaction: ContentRedactionTypeDef = ...,
         IdentifyLanguage: bool = ...,
         IdentifyMultipleLanguages: bool = ...,
         LanguageOptions: Sequence[LanguageCodeType] = ...,
         Subtitles: SubtitlesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         LanguageIdSettings: Mapping[LanguageCodeType, LanguageIdSettingsTypeDef] = ...,
-        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...
+        ToxicityDetection: Sequence[ToxicityDetectionSettingsTypeDef] = ...,
     ) -> StartTranscriptionJobResponseTypeDef:
         """
         Transcribes the audio from a media file and applies any additional Request
         Parameters you choose to include in your
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.start_transcription_job)
@@ -681,30 +681,30 @@
     async def update_vocabulary(
         self,
         *,
         VocabularyName: str,
         LanguageCode: LanguageCodeType,
         Phrases: Sequence[str] = ...,
         VocabularyFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyResponseTypeDef:
         """
         Updates an existing custom vocabulary with new values.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_vocabulary)
         """
 
     async def update_vocabulary_filter(
         self,
         *,
         VocabularyFilterName: str,
         Words: Sequence[str] = ...,
         VocabularyFilterFileUri: str = ...,
-        DataAccessRoleArn: str = ...
+        DataAccessRoleArn: str = ...,
     ) -> UpdateVocabularyFilterResponseTypeDef:
         """
         Updates an existing custom vocabulary filter with a new list of words.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService.Client.update_vocabulary_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/client/#update_vocabulary_filter)
         """
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/literals.py` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/literals.py`

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
     "BaseModelNameType",
     "CLMLanguageCodeType",
     "CallAnalyticsJobStatusType",
     "InputTypeType",
     "LanguageCodeType",
     "MediaFormatType",
@@ -48,15 +47,14 @@
     "VocabularyStateType",
     "TranscribeServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BaseModelNameType = Literal["NarrowBand", "WideBand"]
 CLMLanguageCodeType = Literal["de-DE", "en-AU", "en-GB", "en-US", "es-US", "hi-IN", "ja-JP"]
 CallAnalyticsJobStatusType = Literal["COMPLETED", "FAILED", "IN_PROGRESS", "QUEUED"]
 InputTypeType = Literal["POST_CALL", "REAL_TIME"]
 LanguageCodeType = Literal[
     "ab-GE",
     "af-ZA",
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/literals.pyi` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/type_defs.py` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbsoluteTimeRangeTypeDef",
     "ContentRedactionTypeDef",
     "LanguageIdSettingsTypeDef",
     "SummarizationTypeDef",
     "CallAnalyticsJobSummaryTypeDef",
     "ChannelDefinitionTypeDef",
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe/type_defs.pyi` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/PKG-INFO` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-transcribe
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.TranscribeService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.TranscribeService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/
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
 
 <a id="types-aiobotocore-transcribe"></a>
 
 # types-aiobotocore-transcribe
 
 [![PyPI - types-aiobotocore-transcribe](https://img.shields.io/pypi/v/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-transcribe.svg?color=blue)](https://pypi.org/project/types-aiobotocore-transcribe)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-transcribe)](https://pepy.tech/project/types-aiobotocore-transcribe)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.TranscribeService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
+[aiobotocore.TranscribeService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#TranscribeService)
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
 [types-aiobotocore-transcribe docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transcribe/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-transcribe-2.9.0/types_aiobotocore_transcribe.egg-info/SOURCES.txt` & `types-aiobotocore-transcribe-2.9.1/types_aiobotocore_transcribe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

