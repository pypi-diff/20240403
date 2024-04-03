# Comparing `tmp/types-aiobotocore-personalize-2.9.0.tar.gz` & `tmp/types-aiobotocore-personalize-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-personalize-2.9.0.tar", last modified: Wed Dec 13 20:00:07 2023, max compression
+gzip compressed data, was "types-aiobotocore-personalize-2.9.1.tar", last modified: Thu Jan 18 01:21:28 2024, max compression
```

## Comparing `types-aiobotocore-personalize-2.9.0.tar` & `types-aiobotocore-personalize-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.841334 types-aiobotocore-personalize-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2023-12-13 20:00:07.841334 types-aiobotocore-personalize-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:07.841334 types-aiobotocore-personalize-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.841334 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55052 2023-12-13 19:51:30.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    55048 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2023-12-13 19:51:30.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2023-12-13 19:51:30.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    19553 2023-12-13 19:51:30.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    19534 2023-12-13 19:51:30.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    64718 2023-12-13 19:51:33.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    64717 2023-12-13 19:51:32.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:29.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:07.841334 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      889 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:07.000000 types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.341126 types-aiobotocore-personalize-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15483 2024-01-18 01:21:28.341126 types-aiobotocore-personalize-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:28.341126 types-aiobotocore-personalize-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.341126 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55066 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55063 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19535 2024-01-18 01:13:10.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    64717 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64717 2024-01-18 01:13:11.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:13:09.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:28.341126 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15483 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:28.000000 types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-personalize-2.9.0/LICENSE` & `types-aiobotocore-personalize-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-personalize-2.9.0/PKG-INFO` & `types-aiobotocore-personalize-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Personalize 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Personalize 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/
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
 
 <a id="types-aiobotocore-personalize"></a>
 
 # types-aiobotocore-personalize
 
 [![PyPI - types-aiobotocore-personalize](https://img.shields.io/pypi/v/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [types-aiobotocore-personalize docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-2.9.0/README.md` & `types-aiobotocore-personalize-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [types-aiobotocore-personalize docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-2.9.0/setup.py` & `types-aiobotocore-personalize-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-personalize",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_personalize"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Personalize 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Personalize 2.9.1 service generated with"
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
     keywords="aiobotocore personalize type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_personalize": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__init__.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
     ListSchemasPaginator,
     ListSolutionsPaginator,
     ListSolutionVersionsPaginator,
 )
 
 Client = PersonalizeClient
 
-
 __all__ = (
     "Client",
     "ListBatchInferenceJobsPaginator",
     "ListBatchSegmentJobsPaginator",
     "ListCampaignsPaginator",
     "ListDatasetExportJobsPaginator",
     "ListDatasetGroupsPaginator",
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__init__.pyi` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/__main__.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Personalize 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Personalize 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize\nOther"
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

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/client.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PersonalizeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -190,15 +189,15 @@
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         batchInferenceJobMode: BatchInferenceJobModeType = ...,
-        themeGenerationConfig: ThemeGenerationConfigTypeDef = ...
+        themeGenerationConfig: ThemeGenerationConfigTypeDef = ...,
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Generates batch recommendations based on a list of items or users stored in
         Amazon S3 and exports the recommendations to an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
@@ -211,15 +210,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBatchSegmentJobResponseTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_batch_segment_job)
         """
@@ -227,15 +226,15 @@
     async def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_campaign)
         """
@@ -243,15 +242,15 @@
     async def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset)
         """
@@ -260,15 +259,15 @@
         self,
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetExportJobResponseTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset_export_job)
         """
@@ -276,15 +275,15 @@
     async def create_dataset_group(
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset_group)
         """
@@ -294,15 +293,15 @@
         *,
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
-        publishAttributionMetricsToS3: bool = ...
+        publishAttributionMetricsToS3: bool = ...,
     ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
@@ -324,30 +323,30 @@
 
     async def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_filter)
         """
 
     async def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
-        metricsOutputConfig: MetricAttributionOutputTypeDef
+        metricsOutputConfig: MetricAttributionOutputTypeDef,
     ) -> CreateMetricAttributionResponseTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_metric_attribution)
         """
@@ -355,15 +354,15 @@
     async def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_recommender)
@@ -385,30 +384,30 @@
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution)
         """
 
     async def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionVersionResponseTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution_version)
         """
@@ -795,15 +794,15 @@
 
     async def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        domain: DomainType = ...
+        domain: DomainType = ...,
     ) -> ListRecipesResponseTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#list_recipes)
         """
@@ -910,15 +909,15 @@
 
     async def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...
+        campaignConfig: CampaignConfigTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
         configuration, such as the exploration
         configuration.
 
@@ -938,15 +937,15 @@
 
     async def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
-        metricAttributionArn: str = ...
+        metricAttributionArn: str = ...,
     ) -> UpdateMetricAttributionResponseTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_metric_attribution)
         """
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/client.pyi` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         jobOutput: BatchInferenceJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
         batchInferenceJobConfig: BatchInferenceJobConfigTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         batchInferenceJobMode: BatchInferenceJobModeType = ...,
-        themeGenerationConfig: ThemeGenerationConfigTypeDef = ...
+        themeGenerationConfig: ThemeGenerationConfigTypeDef = ...,
     ) -> CreateBatchInferenceJobResponseTypeDef:
         """
         Generates batch recommendations based on a list of items or users stored in
         Amazon S3 and exports the recommendations to an Amazon S3
         bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_inference_job)
@@ -207,15 +207,15 @@
         jobName: str,
         solutionVersionArn: str,
         jobInput: BatchSegmentJobInputTypeDef,
         jobOutput: BatchSegmentJobOutputTypeDef,
         roleArn: str,
         filterArn: str = ...,
         numResults: int = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateBatchSegmentJobResponseTypeDef:
         """
         Creates a batch segment job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_batch_segment_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_batch_segment_job)
         """
@@ -223,15 +223,15 @@
     async def create_campaign(
         self,
         *,
         name: str,
         solutionVersionArn: str,
         minProvisionedTPS: int = ...,
         campaignConfig: CampaignConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCampaignResponseTypeDef:
         """
         Creates a campaign that deploys a solution version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_campaign)
         """
@@ -239,15 +239,15 @@
     async def create_dataset(
         self,
         *,
         name: str,
         schemaArn: str,
         datasetGroupArn: str,
         datasetType: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an empty dataset and adds it to the specified dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset)
         """
@@ -256,15 +256,15 @@
         self,
         *,
         jobName: str,
         datasetArn: str,
         roleArn: str,
         jobOutput: DatasetExportJobOutputTypeDef,
         ingestionMode: IngestionModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetExportJobResponseTypeDef:
         """
         Creates a job that exports data from your dataset to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset_export_job)
         """
@@ -272,15 +272,15 @@
     async def create_dataset_group(
         self,
         *,
         name: str,
         roleArn: str = ...,
         kmsKeyArn: str = ...,
         domain: DomainType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDatasetGroupResponseTypeDef:
         """
         Creates an empty dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_dataset_group)
         """
@@ -290,15 +290,15 @@
         *,
         jobName: str,
         datasetArn: str,
         dataSource: DataSourceTypeDef,
         roleArn: str,
         tags: Sequence[TagTypeDef] = ...,
         importMode: ImportModeType = ...,
-        publishAttributionMetricsToS3: bool = ...
+        publishAttributionMetricsToS3: bool = ...,
     ) -> CreateDatasetImportJobResponseTypeDef:
         """
         Creates a job that imports training data from your data source (an Amazon S3
         bucket) to an Amazon Personalize
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_dataset_import_job)
@@ -320,30 +320,30 @@
 
     async def create_filter(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         filterExpression: str,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a recommendation filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_filter)
         """
 
     async def create_metric_attribution(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         metrics: Sequence[MetricAttributeTypeDef],
-        metricsOutputConfig: MetricAttributionOutputTypeDef
+        metricsOutputConfig: MetricAttributionOutputTypeDef,
     ) -> CreateMetricAttributionResponseTypeDef:
         """
         Creates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_metric_attribution)
         """
@@ -351,15 +351,15 @@
     async def create_recommender(
         self,
         *,
         name: str,
         datasetGroupArn: str,
         recipeArn: str,
         recommenderConfig: RecommenderConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateRecommenderResponseTypeDef:
         """
         Creates a recommender with the recipe (a Domain dataset group use case) you
         specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_recommender)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_recommender)
@@ -381,30 +381,30 @@
         name: str,
         datasetGroupArn: str,
         performHPO: bool = ...,
         performAutoML: bool = ...,
         recipeArn: str = ...,
         eventType: str = ...,
         solutionConfig: SolutionConfigTypeDef = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionResponseTypeDef:
         """
         Creates the configuration for training a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution)
         """
 
     async def create_solution_version(
         self,
         *,
         solutionArn: str,
         name: str = ...,
         trainingMode: TrainingModeType = ...,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> CreateSolutionVersionResponseTypeDef:
         """
         Trains or retrains an active solution in a Custom dataset group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.create_solution_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#create_solution_version)
         """
@@ -791,15 +791,15 @@
 
     async def list_recipes(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        domain: DomainType = ...
+        domain: DomainType = ...,
     ) -> ListRecipesResponseTypeDef:
         """
         Returns a list of available recipes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.list_recipes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#list_recipes)
         """
@@ -906,15 +906,15 @@
 
     async def update_campaign(
         self,
         *,
         campaignArn: str,
         solutionVersionArn: str = ...,
         minProvisionedTPS: int = ...,
-        campaignConfig: CampaignConfigTypeDef = ...
+        campaignConfig: CampaignConfigTypeDef = ...,
     ) -> UpdateCampaignResponseTypeDef:
         """
         Updates a campaign to deploy a retrained solution version with an existing
         campaign, change your campaign's `minProvisionedTPS`, or modify your campaign's
         configuration, such as the exploration
         configuration.
 
@@ -934,15 +934,15 @@
 
     async def update_metric_attribution(
         self,
         *,
         addMetrics: Sequence[MetricAttributeTypeDef] = ...,
         removeMetrics: Sequence[str] = ...,
         metricsOutputConfig: MetricAttributionOutputTypeDef = ...,
-        metricAttributionArn: str = ...
+        metricAttributionArn: str = ...,
     ) -> UpdateMetricAttributionResponseTypeDef:
         """
         Updates a metric attribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Client.update_metric_attribution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/client/#update_metric_attribution)
         """
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/literals.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/literals.py`

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
     "BatchInferenceJobModeType",
     "DomainType",
     "ImportModeType",
     "IngestionModeType",
     "ListBatchInferenceJobsPaginatorName",
     "ListBatchSegmentJobsPaginatorName",
@@ -47,15 +46,14 @@
     "PersonalizeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 BatchInferenceJobModeType = Literal["BATCH_INFERENCE", "THEME_GENERATION"]
 DomainType = Literal["ECOMMERCE", "VIDEO_ON_DEMAND"]
 ImportModeType = Literal["FULL", "INCREMENTAL"]
 IngestionModeType = Literal["ALL", "BULK", "PUT"]
 ListBatchInferenceJobsPaginatorName = Literal["list_batch_inference_jobs"]
 ListBatchSegmentJobsPaginatorName = Literal["list_batch_segment_jobs"]
 ListCampaignsPaginatorName = Literal["list_campaigns"]
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/literals.pyi` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/paginator.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListBatchInferenceJobsPaginator",
     "ListBatchSegmentJobsPaginator",
     "ListCampaignsPaginator",
     "ListDatasetExportJobsPaginator",
     "ListDatasetGroupsPaginator",
     "ListDatasetImportJobsPaginator",
@@ -99,15 +98,14 @@
     "ListRecipesPaginator",
     "ListRecommendersPaginator",
     "ListSchemasPaginator",
     "ListSolutionVersionsPaginator",
     "ListSolutionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -286,15 +284,15 @@
     """
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/paginators/#listrecipespaginator)
         """
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/paginator.pyi` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -271,15 +271,15 @@
     """
 
     def paginate(
         self,
         *,
         recipeProvider: Literal["SERVICE"] = ...,
         domain: DomainType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecipesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize.Paginator.ListRecipes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/paginators/#listrecipespaginator)
         """
 
 class ListRecommendersPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/type_defs.py` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/type_defs.py`

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
     "AlgorithmImageTypeDef",
     "AutoMLConfigTypeDef",
     "AutoMLResultTypeDef",
     "BatchInferenceJobConfigTypeDef",
     "S3DataConfigTypeDef",
     "BatchInferenceJobSummaryTypeDef",
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize/type_defs.pyi` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/PKG-INFO` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Personalize 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Personalize 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/
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
 
 <a id="types-aiobotocore-personalize"></a>
 
 # types-aiobotocore-personalize
 
 [![PyPI - types-aiobotocore-personalize](https://img.shields.io/pypi/v/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-personalize.svg?color=blue)](https://pypi.org/project/types-aiobotocore-personalize)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-personalize)](https://pepy.tech/project/types-aiobotocore-personalize)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Personalize 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
+[aiobotocore.Personalize 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#Personalize)
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
 [types-aiobotocore-personalize docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-personalize-2.9.0/types_aiobotocore_personalize.egg-info/SOURCES.txt` & `types-aiobotocore-personalize-2.9.1/types_aiobotocore_personalize.egg-info/SOURCES.txt`

 * *Files identical despite different names*

