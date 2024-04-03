# Comparing `tmp/types-aiobotocore-polly-2.9.0.tar.gz` & `tmp/types-aiobotocore-polly-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-polly-2.9.0.tar", last modified: Wed Dec 13 20:00:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-polly-2.9.1.tar", last modified: Thu Jan 18 01:21:31 2024, max compression
```

## Comparing `types-aiobotocore-polly-2.9.0.tar` & `types-aiobotocore-polly-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.877308 types-aiobotocore-polly-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2023-12-13 20:00:10.877308 types-aiobotocore-polly-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11616 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:10.877308 types-aiobotocore-polly-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.877308 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12651 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2023-12-13 19:51:55.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11285 2023-12-13 19:51:55.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2023-12-13 19:51:55.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8973 2023-12-13 19:51:55.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:54.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:10.877308 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13171 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-13 20:00:10.000000 types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.069113 types-aiobotocore-polly-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-01-18 01:21:31.069113 types-aiobotocore-polly-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11616 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:31.069113 types-aiobotocore-polly-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.069113 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12650 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-01-18 01:13:32.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11285 2024-01-18 01:13:32.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-01-18 01:13:32.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8973 2024-01-18 01:13:32.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:31.069113 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13191 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-18 01:21:31.000000 types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-polly-2.9.0/LICENSE` & `types-aiobotocore-polly-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-polly-2.9.0/PKG-INFO` & `types-aiobotocore-polly-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Polly 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Polly 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
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
 
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-polly-2.9.0/README.md` & `types-aiobotocore-polly-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-polly-2.9.0/setup.py` & `types-aiobotocore-polly-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-polly",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Polly 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Polly 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore polly type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_polly": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__init__.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     DescribeVoicesPaginator,
     ListLexiconsPaginator,
     ListSpeechSynthesisTasksPaginator,
 )
 
 Client = PollyClient
 
-
 __all__ = (
     "Client",
     "DescribeVoicesPaginator",
     "ListLexiconsPaginator",
     "ListSpeechSynthesisTasksPaginator",
     "PollyClient",
 )
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__init__.pyi` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/__main__.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Polly 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Polly 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/client.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PollyClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -131,15 +130,15 @@
 
     async def describe_voices(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeVoicesOutputTypeDef:
         """
         Returns the list of voices that are available for use when requesting speech
         synthesis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.describe_voices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#describe_voices)
@@ -216,15 +215,15 @@
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         LexiconNames: Sequence[str] = ...,
         OutputS3KeyPrefix: str = ...,
         SampleRate: str = ...,
         SnsTopicArn: str = ...,
         SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,
-        TextType: TextTypeType = ...
+        TextType: TextTypeType = ...,
     ) -> StartSpeechSynthesisTaskOutputTypeDef:
         """
         Allows the creation of an asynchronous synthesis task, by starting a new
         `SpeechSynthesisTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.start_speech_synthesis_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#start_speech_synthesis_task)
@@ -237,15 +236,15 @@
         Text: str,
         VoiceId: VoiceIdType,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         LexiconNames: Sequence[str] = ...,
         SampleRate: str = ...,
         SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,
-        TextType: TextTypeType = ...
+        TextType: TextTypeType = ...,
     ) -> SynthesizeSpeechOutputTypeDef:
         """
         Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.synthesize_speech)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#synthesize_speech)
         """
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/client.pyi` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 
     async def describe_voices(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> DescribeVoicesOutputTypeDef:
         """
         Returns the list of voices that are available for use when requesting speech
         synthesis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.describe_voices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#describe_voices)
@@ -212,15 +212,15 @@
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         LexiconNames: Sequence[str] = ...,
         OutputS3KeyPrefix: str = ...,
         SampleRate: str = ...,
         SnsTopicArn: str = ...,
         SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,
-        TextType: TextTypeType = ...
+        TextType: TextTypeType = ...,
     ) -> StartSpeechSynthesisTaskOutputTypeDef:
         """
         Allows the creation of an asynchronous synthesis task, by starting a new
         `SpeechSynthesisTask`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.start_speech_synthesis_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#start_speech_synthesis_task)
@@ -233,15 +233,15 @@
         Text: str,
         VoiceId: VoiceIdType,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         LexiconNames: Sequence[str] = ...,
         SampleRate: str = ...,
         SpeechMarkTypes: Sequence[SpeechMarkTypeType] = ...,
-        TextType: TextTypeType = ...
+        TextType: TextTypeType = ...,
     ) -> SynthesizeSpeechOutputTypeDef:
         """
         Synthesizes UTF-8 input, plain text or SSML, to a stream of bytes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Client.synthesize_speech)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/client/#synthesize_speech)
         """
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/literals.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/literals.py`

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
     "DescribeVoicesPaginatorName",
     "EngineType",
     "GenderType",
     "LanguageCodeType",
     "ListLexiconsPaginatorName",
     "ListSpeechSynthesisTasksPaginatorName",
@@ -35,15 +34,14 @@
     "PollyServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeVoicesPaginatorName = Literal["describe_voices"]
 EngineType = Literal["long-form", "neural", "standard"]
 GenderType = Literal["Female", "Male"]
 LanguageCodeType = Literal[
     "ar-AE",
     "arb",
     "ca-ES",
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/literals.pyi` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/paginator.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListLexiconsOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeVoicesPaginator", "ListLexiconsPaginator", "ListSpeechSynthesisTasksPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -59,15 +58,15 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#describevoicespaginator)
         """
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/paginator.pyi` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#describevoicespaginator)
         """
 
 class ListLexiconsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/type_defs.py` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/type_defs.py`

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
     "DeleteLexiconInputRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeVoicesInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly/type_defs.pyi` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/PKG-INFO` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Polly 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Polly 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
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
 
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Polly 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[aiobotocore.Polly 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-polly-2.9.0/types_aiobotocore_polly.egg-info/SOURCES.txt` & `types-aiobotocore-polly-2.9.1/types_aiobotocore_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

