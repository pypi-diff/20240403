# Comparing `tmp/types-aiobotocore-comprehendmedical-2.9.0.tar.gz` & `tmp/types-aiobotocore-comprehendmedical-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-comprehendmedical-2.9.0.tar", last modified: Wed Dec 13 19:58:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-comprehendmedical-2.9.1.tar", last modified: Thu Jan 18 01:20:24 2024, max compression
```

## Comparing `types-aiobotocore-comprehendmedical-2.9.0.tar` & `types-aiobotocore-comprehendmedical-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.569900 types-aiobotocore-comprehendmedical-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2023-12-13 19:58:58.569900 types-aiobotocore-comprehendmedical-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11136 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:58.569900 types-aiobotocore-comprehendmedical-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.565900 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23346 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23342 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12208 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12206 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24226 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24225 2023-12-13 19:43:14.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:13.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.569900 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12739 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:58.000000 types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.589423 types-aiobotocore-comprehendmedical-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-01-18 01:20:24.589423 types-aiobotocore-comprehendmedical-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11136 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:24.589423 types-aiobotocore-comprehendmedical-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.585423 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23355 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23352 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-01-18 01:05:10.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12206 2024-01-18 01:05:10.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-01-18 01:05:10.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24225 2024-01-18 01:05:10.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:09.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.589423 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:24.000000 types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/LICENSE` & `types-aiobotocore-comprehendmedical-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
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
 
 <a id="types-aiobotocore-comprehendmedical"></a>
 
 # types-aiobotocore-comprehendmedical
 
 [![PyPI - types-aiobotocore-comprehendmedical](https://img.shields.io/pypi/v/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/README.md` & `types-aiobotocore-comprehendmedical-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/setup.py` & `types-aiobotocore-comprehendmedical-2.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-comprehendmedical",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ComprehendMedical 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ComprehendMedical 2.9.1 service generated with"
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
     keywords="aiobotocore comprehendmedical type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_comprehendmedical": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__init__.py` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import ComprehendMedicalClient
 
 Client = ComprehendMedicalClient
 
-
 __all__ = ("Client", "ComprehendMedicalClient")
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__init__.pyi` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/__main__.py` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ComprehendMedical 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ComprehendMedical 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
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

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/client.py` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ComprehendMedicalClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -245,72 +244,72 @@
         """
 
     async def list_entities_detection_v2_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntitiesDetectionV2JobsResponseTypeDef:
         """
         Gets a list of medical entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_entities_detection_v2_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_entities_detection_v2_jobs)
         """
 
     async def list_icd10_cm_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListICD10CMInferenceJobsResponseTypeDef:
         """
         Gets a list of InferICD10CM jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_icd10_cm_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_icd10_cm_inference_jobs)
         """
 
     async def list_phi_detection_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPHIDetectionJobsResponseTypeDef:
         """
         Gets a list of protected health information (PHI) detection jobs you have
         submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_phi_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_phi_detection_jobs)
         """
 
     async def list_rx_norm_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRxNormInferenceJobsResponseTypeDef:
         """
         Gets a list of InferRxNorm jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_rx_norm_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_rx_norm_inference_jobs)
         """
 
     async def list_snomedct_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSNOMEDCTInferenceJobsResponseTypeDef:
         """
         Gets a list of InferSNOMEDCT jobs a user has submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_snomedct_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_snomedct_inference_jobs)
         """
@@ -320,15 +319,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartEntitiesDetectionV2JobResponseTypeDef:
         """
         Starts an asynchronous medical entity detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_entities_detection_v2_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#start_entities_detection_v2_job)
@@ -339,15 +338,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartICD10CMInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medical conditions and link them to the
         ICD-10-CM
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_icd10_cm_inference_job)
@@ -359,15 +358,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartPHIDetectionJobResponseTypeDef:
         """
         Starts an asynchronous job to detect protected health information (PHI).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_phi_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#start_phi_detection_job)
         """
@@ -377,15 +376,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartRxNormInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medication entities and link them to the
         RxNorm
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_rx_norm_inference_job)
@@ -397,15 +396,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartSNOMEDCTInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medical concepts and link them to the
         SNOMED-CT
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_snomedct_inference_job)
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/client.pyi` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -241,72 +241,72 @@
         """
 
     async def list_entities_detection_v2_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListEntitiesDetectionV2JobsResponseTypeDef:
         """
         Gets a list of medical entity detection jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_entities_detection_v2_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_entities_detection_v2_jobs)
         """
 
     async def list_icd10_cm_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListICD10CMInferenceJobsResponseTypeDef:
         """
         Gets a list of InferICD10CM jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_icd10_cm_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_icd10_cm_inference_jobs)
         """
 
     async def list_phi_detection_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPHIDetectionJobsResponseTypeDef:
         """
         Gets a list of protected health information (PHI) detection jobs you have
         submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_phi_detection_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_phi_detection_jobs)
         """
 
     async def list_rx_norm_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListRxNormInferenceJobsResponseTypeDef:
         """
         Gets a list of InferRxNorm jobs that you have submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_rx_norm_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_rx_norm_inference_jobs)
         """
 
     async def list_snomedct_inference_jobs(
         self,
         *,
         Filter: ComprehendMedicalAsyncJobFilterTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListSNOMEDCTInferenceJobsResponseTypeDef:
         """
         Gets a list of InferSNOMEDCT jobs a user has submitted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.list_snomedct_inference_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#list_snomedct_inference_jobs)
         """
@@ -316,15 +316,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartEntitiesDetectionV2JobResponseTypeDef:
         """
         Starts an asynchronous medical entity detection job for a collection of
         documents.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_entities_detection_v2_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#start_entities_detection_v2_job)
@@ -335,15 +335,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartICD10CMInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medical conditions and link them to the
         ICD-10-CM
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_icd10_cm_inference_job)
@@ -355,15 +355,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartPHIDetectionJobResponseTypeDef:
         """
         Starts an asynchronous job to detect protected health information (PHI).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_phi_detection_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/client/#start_phi_detection_job)
         """
@@ -373,15 +373,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartRxNormInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medication entities and link them to the
         RxNorm
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_rx_norm_inference_job)
@@ -393,15 +393,15 @@
         *,
         InputDataConfig: InputDataConfigTypeDef,
         OutputDataConfig: OutputDataConfigTypeDef,
         DataAccessRoleArn: str,
         LanguageCode: Literal["en"],
         JobName: str = ...,
         ClientRequestToken: str = ...,
-        KMSKey: str = ...
+        KMSKey: str = ...,
     ) -> StartSNOMEDCTInferenceJobResponseTypeDef:
         """
         Starts an asynchronous job to detect medical concepts and link them to the
         SNOMED-CT
         ontology.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical.Client.start_snomedct_inference_job)
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/literals.py` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/literals.py`

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
     "AttributeNameType",
     "EntitySubTypeType",
     "EntityTypeType",
     "ICD10CMAttributeTypeType",
     "ICD10CMEntityCategoryType",
     "ICD10CMEntityTypeType",
@@ -43,15 +42,14 @@
     "SNOMEDCTTraitNameType",
     "ComprehendMedicalServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AttributeNameType = Literal[
     "DIAGNOSIS",
     "FUTURE",
     "HYPOTHETICAL",
     "LOW_CONFIDENCE",
     "NEGATION",
     "PAST_HISTORY",
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/literals.pyi` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/type_defs.py` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/type_defs.py`

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
     "TraitTypeDef",
     "CharactersTypeDef",
     "TimestampTypeDef",
     "InputDataConfigTypeDef",
     "OutputDataConfigTypeDef",
     "DescribeEntitiesDetectionV2JobRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical/type_defs.pyi` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-comprehendmedical
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ComprehendMedical 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ComprehendMedical 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/
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
 
 <a id="types-aiobotocore-comprehendmedical"></a>
 
 # types-aiobotocore-comprehendmedical
 
 [![PyPI - types-aiobotocore-comprehendmedical](https://img.shields.io/pypi/v/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-comprehendmedical.svg?color=blue)](https://pypi.org/project/types-aiobotocore-comprehendmedical)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-comprehendmedical)](https://pepy.tech/project/types-aiobotocore-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComprehendMedical 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[aiobotocore.ComprehendMedical 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
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
 [types-aiobotocore-comprehendmedical docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-comprehendmedical-2.9.0/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt` & `types-aiobotocore-comprehendmedical-2.9.1/types_aiobotocore_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

