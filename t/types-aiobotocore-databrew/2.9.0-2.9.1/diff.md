# Comparing `tmp/types-aiobotocore-databrew-2.9.0.tar.gz` & `tmp/types-aiobotocore-databrew-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-databrew-2.9.0.tar", last modified: Wed Dec 13 19:59:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-databrew-2.9.1.tar", last modified: Thu Jan 18 01:20:28 2024, max compression
```

## Comparing `types-aiobotocore-databrew-2.9.0.tar` & `types-aiobotocore-databrew-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.089863 types-aiobotocore-databrew-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2023-12-13 19:59:03.089863 types-aiobotocore-databrew-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:03.089863 types-aiobotocore-databrew-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.085863 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36047 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    36043 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11227 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9616 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9606 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    51173 2023-12-13 19:43:44.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    51172 2023-12-13 19:43:44.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:43.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.089863 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13896 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-13 19:59:03.000000 types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.745404 types-aiobotocore-databrew-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-01-18 01:20:28.745404 types-aiobotocore-databrew-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:28.745404 types-aiobotocore-databrew-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.741404 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36058 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36055 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11227 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9616 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    51172 2024-01-18 01:05:39.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51172 2024-01-18 01:05:39.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:38.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:28.745404 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 01:20:28.000000 types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-databrew-2.9.0/LICENSE` & `types-aiobotocore-databrew-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-databrew-2.9.0/PKG-INFO` & `types-aiobotocore-databrew-2.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-databrew
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GlueDataBrew 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GlueDataBrew 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/
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
 
 <a id="types-aiobotocore-databrew"></a>
 
 # types-aiobotocore-databrew
 
 [![PyPI - types-aiobotocore-databrew](https://img.shields.io/pypi/v/types-aiobotocore-databrew.svg?color=blue)](https://pypi.org/project/types-aiobotocore-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-databrew.svg?color=blue)](https://pypi.org/project/types-aiobotocore-databrew)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-databrew)](https://pepy.tech/project/types-aiobotocore-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlueDataBrew 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[aiobotocore.GlueDataBrew 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [types-aiobotocore-databrew docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-databrew-2.9.0/README.md` & `types-aiobotocore-databrew-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-databrew.svg?color=blue)](https://pypi.org/project/types-aiobotocore-databrew)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-databrew)](https://pepy.tech/project/types-aiobotocore-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlueDataBrew 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[aiobotocore.GlueDataBrew 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [types-aiobotocore-databrew docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-databrew-2.9.0/setup.py` & `types-aiobotocore-databrew-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-databrew",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_databrew"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.GlueDataBrew 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.GlueDataBrew 2.9.1 service generated with"
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
     keywords="aiobotocore databrew type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_databrew": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__init__.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     ListRecipeVersionsPaginator,
     ListRulesetsPaginator,
     ListSchedulesPaginator,
 )
 
 Client = GlueDataBrewClient
 
-
 __all__ = (
     "Client",
     "GlueDataBrewClient",
     "ListDatasetsPaginator",
     "ListJobRunsPaginator",
     "ListJobsPaginator",
     "ListProjectsPaginator",
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__init__.pyi` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/__main__.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GlueDataBrew 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.GlueDataBrew 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew\nOther"
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

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/client.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GlueDataBrewClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -166,15 +165,15 @@
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
         FormatOptions: FormatOptionsTypeDef = ...,
         PathOptions: PathOptionsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_dataset)
         """
@@ -191,15 +190,15 @@
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         Configuration: ProfileConfigurationTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
-        JobSample: JobSampleTypeDef = ...
+        JobSample: JobSampleTypeDef = ...,
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_profile_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_profile_job)
         """
@@ -208,30 +207,30 @@
         self,
         *,
         DatasetName: str,
         Name: str,
         RecipeName: str,
         RoleArn: str,
         Sample: SampleTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a new DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_project)
         """
 
     async def create_recipe(
         self,
         *,
         Name: str,
         Steps: Sequence[RecipeStepTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_recipe)
         """
@@ -249,15 +248,15 @@
         MaxRetries: int = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> CreateRecipeJobResponseTypeDef:
         """
         Creates a new job to transform input data, using steps defined in an existing
         Glue DataBrew recipe See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/databrew-2017-07-25/CreateRecipeJob).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe_job)
@@ -267,15 +266,15 @@
     async def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
         Rules: Sequence[RuleTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_ruleset)
@@ -284,15 +283,15 @@
 
     async def create_schedule(
         self,
         *,
         CronExpression: str,
         Name: str,
         JobNames: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateScheduleResponseTypeDef:
         """
         Creates a new schedule for one or more DataBrew jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_schedule)
         """
@@ -443,15 +442,15 @@
 
     async def list_jobs(
         self,
         *,
         DatasetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProjectName: str = ...
+        ProjectName: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Lists all of the DataBrew jobs that are defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#list_jobs)
         """
@@ -532,15 +531,15 @@
         self,
         *,
         Name: str,
         Preview: bool = ...,
         RecipeStep: RecipeStepTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
-        ViewFrame: ViewFrameTypeDef = ...
+        ViewFrame: ViewFrameTypeDef = ...,
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.send_project_session_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#send_project_session_action)
@@ -594,15 +593,15 @@
     async def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
         FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...
+        PathOptions: PathOptionsTypeDef = ...,
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_dataset)
         """
@@ -617,15 +616,15 @@
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
-        JobSample: JobSampleTypeDef = ...
+        JobSample: JobSampleTypeDef = ...,
     ) -> UpdateProfileJobResponseTypeDef:
         """
         Modifies the definition of an existing profile job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_profile_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_profile_job)
         """
@@ -659,15 +658,15 @@
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe_job)
         """
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/client.pyi` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
         FormatOptions: FormatOptionsTypeDef = ...,
         PathOptions: PathOptionsTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates a new DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_dataset)
         """
@@ -187,15 +187,15 @@
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         Configuration: ProfileConfigurationTypeDef = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Tags: Mapping[str, str] = ...,
         Timeout: int = ...,
-        JobSample: JobSampleTypeDef = ...
+        JobSample: JobSampleTypeDef = ...,
     ) -> CreateProfileJobResponseTypeDef:
         """
         Creates a new job to analyze a dataset and create its data profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_profile_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_profile_job)
         """
@@ -204,30 +204,30 @@
         self,
         *,
         DatasetName: str,
         Name: str,
         RecipeName: str,
         RoleArn: str,
         Sample: SampleTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a new DataBrew project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_project)
         """
 
     async def create_recipe(
         self,
         *,
         Name: str,
         Steps: Sequence[RecipeStepTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRecipeResponseTypeDef:
         """
         Creates a new DataBrew recipe.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_recipe)
         """
@@ -245,15 +245,15 @@
         MaxRetries: int = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
         ProjectName: str = ...,
         RecipeReference: RecipeReferenceTypeDef = ...,
         Tags: Mapping[str, str] = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> CreateRecipeJobResponseTypeDef:
         """
         Creates a new job to transform input data, using steps defined in an existing
         Glue DataBrew recipe See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/databrew-2017-07-25/CreateRecipeJob).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_recipe_job)
@@ -263,15 +263,15 @@
     async def create_ruleset(
         self,
         *,
         Name: str,
         TargetArn: str,
         Rules: Sequence[RuleTypeDef],
         Description: str = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateRulesetResponseTypeDef:
         """
         Creates a new ruleset that can be used in a profile job to validate the data
         quality of a
         dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_ruleset)
@@ -280,15 +280,15 @@
 
     async def create_schedule(
         self,
         *,
         CronExpression: str,
         Name: str,
         JobNames: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateScheduleResponseTypeDef:
         """
         Creates a new schedule for one or more DataBrew jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.create_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#create_schedule)
         """
@@ -439,15 +439,15 @@
 
     async def list_jobs(
         self,
         *,
         DatasetName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ProjectName: str = ...
+        ProjectName: str = ...,
     ) -> ListJobsResponseTypeDef:
         """
         Lists all of the DataBrew jobs that are defined.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.list_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#list_jobs)
         """
@@ -528,15 +528,15 @@
         self,
         *,
         Name: str,
         Preview: bool = ...,
         RecipeStep: RecipeStepTypeDef = ...,
         StepIndex: int = ...,
         ClientSessionId: str = ...,
-        ViewFrame: ViewFrameTypeDef = ...
+        ViewFrame: ViewFrameTypeDef = ...,
     ) -> SendProjectSessionActionResponseTypeDef:
         """
         Performs a recipe step within an interactive DataBrew session that's currently
         open.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.send_project_session_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#send_project_session_action)
@@ -590,15 +590,15 @@
     async def update_dataset(
         self,
         *,
         Name: str,
         Input: InputTypeDef,
         Format: InputFormatType = ...,
         FormatOptions: FormatOptionsTypeDef = ...,
-        PathOptions: PathOptionsTypeDef = ...
+        PathOptions: PathOptionsTypeDef = ...,
     ) -> UpdateDatasetResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_dataset)
         """
@@ -613,15 +613,15 @@
         EncryptionKeyArn: str = ...,
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         ValidationConfigurations: Sequence[ValidationConfigurationTypeDef] = ...,
         Timeout: int = ...,
-        JobSample: JobSampleTypeDef = ...
+        JobSample: JobSampleTypeDef = ...,
     ) -> UpdateProfileJobResponseTypeDef:
         """
         Modifies the definition of an existing profile job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_profile_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_profile_job)
         """
@@ -655,15 +655,15 @@
         EncryptionMode: EncryptionModeType = ...,
         LogSubscription: LogSubscriptionType = ...,
         MaxCapacity: int = ...,
         MaxRetries: int = ...,
         Outputs: Sequence[OutputTypeDef] = ...,
         DataCatalogOutputs: Sequence[DataCatalogOutputTypeDef] = ...,
         DatabaseOutputs: Sequence[DatabaseOutputTypeDef] = ...,
-        Timeout: int = ...
+        Timeout: int = ...,
     ) -> UpdateRecipeJobResponseTypeDef:
         """
         Modifies the definition of an existing DataBrew recipe job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Client.update_recipe_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/client/#update_recipe_job)
         """
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/literals.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/literals.py`

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
     "AnalyticsModeType",
     "CompressionFormatType",
     "DatabaseOutputModeType",
     "EncryptionModeType",
     "InputFormatType",
     "JobRunStateType",
@@ -51,15 +50,14 @@
     "GlueDataBrewServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AnalyticsModeType = Literal["DISABLE", "ENABLE"]
 CompressionFormatType = Literal[
     "BROTLI", "BZIP2", "DEFLATE", "GZIP", "LZ4", "LZO", "SNAPPY", "ZLIB", "ZSTD"
 ]
 DatabaseOutputModeType = Literal["NEW_TABLE"]
 EncryptionModeType = Literal["SSE-KMS", "SSE-S3"]
 InputFormatType = Literal["CSV", "EXCEL", "JSON", "ORC", "PARQUET"]
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/literals.pyi` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/paginator.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
     "ListProjectsPaginator",
     "ListRecipeVersionsPaginator",
     "ListRecipesPaginator",
     "ListRulesetsPaginator",
     "ListSchedulesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -111,15 +110,15 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/paginators/#listjobspaginator)
         """
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/paginator.pyi` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     """
 
     def paginate(
         self,
         *,
         DatasetName: str = ...,
         ProjectName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/paginators/#listjobspaginator)
         """
 
 class ListProjectsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/type_defs.py` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/type_defs.py`

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
     "AllowedStatisticsTypeDef",
     "BatchDeleteRecipeVersionRequestRequestTypeDef",
     "RecipeVersionErrorDetailTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnSelectorTypeDef",
     "ConditionExpressionTypeDef",
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew/type_defs.pyi` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/PKG-INFO` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-databrew
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.GlueDataBrew 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.GlueDataBrew 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/
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
 
 <a id="types-aiobotocore-databrew"></a>
 
 # types-aiobotocore-databrew
 
 [![PyPI - types-aiobotocore-databrew](https://img.shields.io/pypi/v/types-aiobotocore-databrew.svg?color=blue)](https://pypi.org/project/types-aiobotocore-databrew)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-databrew.svg?color=blue)](https://pypi.org/project/types-aiobotocore-databrew)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-databrew)](https://pepy.tech/project/types-aiobotocore-databrew)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.GlueDataBrew 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
+[aiobotocore.GlueDataBrew 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#GlueDataBrew)
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
 [types-aiobotocore-databrew docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_databrew/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-databrew-2.9.0/types_aiobotocore_databrew.egg-info/SOURCES.txt` & `types-aiobotocore-databrew-2.9.1/types_aiobotocore_databrew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

