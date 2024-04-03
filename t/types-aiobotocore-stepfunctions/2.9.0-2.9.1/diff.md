# Comparing `tmp/types-aiobotocore-stepfunctions-2.9.0.tar.gz` & `tmp/types-aiobotocore-stepfunctions-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-stepfunctions-2.9.0.tar", last modified: Wed Dec 13 20:00:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-stepfunctions-2.9.1.tar", last modified: Thu Jan 18 01:21:55 2024, max compression
```

## Comparing `types-aiobotocore-stepfunctions-2.9.0.tar` & `types-aiobotocore-stepfunctions-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.785075 types-aiobotocore-stepfunctions-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-12-13 20:00:37.785075 types-aiobotocore-stepfunctions-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:37.785075 types-aiobotocore-stepfunctions-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2023-12-13 19:57:03.000000 types-aiobotocore-stepfunctions-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.785075 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31976 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31972 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11935 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    39359 2023-12-13 19:57:05.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    39358 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:57:04.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:37.785075 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 20:00:37.000000 types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.469004 types-aiobotocore-stepfunctions-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-01-18 01:21:55.469004 types-aiobotocore-stepfunctions-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:55.469004 types-aiobotocore-stepfunctions-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.469004 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31983 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31980 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11935 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6770 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39358 2024-01-18 01:18:35.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:18:34.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:55.469004 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13811 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:21:55.000000 types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/LICENSE` & `types-aiobotocore-stepfunctions-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-stepfunctions-2.9.0/PKG-INFO` & `types-aiobotocore-stepfunctions-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SFN 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SFN 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
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
 
 <a id="types-aiobotocore-stepfunctions"></a>
 
 # types-aiobotocore-stepfunctions
 
 [![PyPI - types-aiobotocore-stepfunctions](https://img.shields.io/pypi/v/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/README.md` & `types-aiobotocore-stepfunctions-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/setup.py` & `types-aiobotocore-stepfunctions-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-stepfunctions",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SFN 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SFN 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore stepfunctions type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_stepfunctions": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__init__.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 
 Client = SFNClient
 
-
 __all__ = (
     "Client",
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__init__.pyi` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/__main__.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SFN 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SFN 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
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

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/client.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SFNClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -166,29 +165,29 @@
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#create_state_machine)
         """
 
     async def create_state_machine_alias(
         self,
         *,
         name: str,
         routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateStateMachineAliasOutputTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         for a state machine that points to one or two
         [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-version.html)
         of the same state
@@ -323,15 +322,15 @@
     async def get_execution_history(
         self,
         *,
         executionArn: str,
         maxResults: int = ...,
         reverseOrder: bool = ...,
         nextToken: str = ...,
-        includeExecutionData: bool = ...
+        includeExecutionData: bool = ...,
     ) -> GetExecutionHistoryOutputTypeDef:
         """
         Returns the history of the specified execution as a list of events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_execution_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#get_execution_history)
         """
@@ -350,15 +349,15 @@
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         mapRunArn: str = ...,
-        redriveFilter: ExecutionRedriveFilterType = ...
+        redriveFilter: ExecutionRedriveFilterType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Lists all executions of a state machine or a Map Run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#list_executions)
         """
@@ -518,15 +517,15 @@
     async def test_state(
         self,
         *,
         definition: str,
         roleArn: str,
         input: str = ...,
         inspectionLevel: InspectionLevelType = ...,
-        revealSecrets: bool = ...
+        revealSecrets: bool = ...,
     ) -> TestStateOutputTypeDef:
         """
         Accepts the definition of a single state and executes it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.test_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#test_state)
         """
@@ -542,15 +541,15 @@
 
     async def update_map_run(
         self,
         *,
         mapRunArn: str,
         maxConcurrency: int = ...,
         toleratedFailurePercentage: float = ...,
-        toleratedFailureCount: int = ...
+        toleratedFailureCount: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates an in-progress Map Run's configuration to include changes to the
         settings that control maximum concurrency and Map Run
         failure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_map_run)
@@ -562,30 +561,30 @@
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#update_state_machine)
         """
 
     async def update_state_machine_alias(
         self,
         *,
         stateMachineAliasArn: str,
         description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateStateMachineAliasOutputTypeDef:
         """
         Updates the configuration of an existing state machine
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         by modifying its `description` or
         `routingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/client.pyi` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -162,29 +162,29 @@
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#create_state_machine)
         """
 
     async def create_state_machine_alias(
         self,
         *,
         name: str,
         routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
+        description: str = ...,
     ) -> CreateStateMachineAliasOutputTypeDef:
         """
         Creates an
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         for a state machine that points to one or two
         [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-version.html)
         of the same state
@@ -319,15 +319,15 @@
     async def get_execution_history(
         self,
         *,
         executionArn: str,
         maxResults: int = ...,
         reverseOrder: bool = ...,
         nextToken: str = ...,
-        includeExecutionData: bool = ...
+        includeExecutionData: bool = ...,
     ) -> GetExecutionHistoryOutputTypeDef:
         """
         Returns the history of the specified execution as a list of events.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_execution_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#get_execution_history)
         """
@@ -346,15 +346,15 @@
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         mapRunArn: str = ...,
-        redriveFilter: ExecutionRedriveFilterType = ...
+        redriveFilter: ExecutionRedriveFilterType = ...,
     ) -> ListExecutionsOutputTypeDef:
         """
         Lists all executions of a state machine or a Map Run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#list_executions)
         """
@@ -514,15 +514,15 @@
     async def test_state(
         self,
         *,
         definition: str,
         roleArn: str,
         input: str = ...,
         inspectionLevel: InspectionLevelType = ...,
-        revealSecrets: bool = ...
+        revealSecrets: bool = ...,
     ) -> TestStateOutputTypeDef:
         """
         Accepts the definition of a single state and executes it.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.test_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#test_state)
         """
@@ -538,15 +538,15 @@
 
     async def update_map_run(
         self,
         *,
         mapRunArn: str,
         maxConcurrency: int = ...,
         toleratedFailurePercentage: float = ...,
-        toleratedFailureCount: int = ...
+        toleratedFailureCount: int = ...,
     ) -> Dict[str, Any]:
         """
         Updates an in-progress Map Run's configuration to include changes to the
         settings that control maximum concurrency and Map Run
         failure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_map_run)
@@ -558,30 +558,30 @@
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tracingConfiguration: TracingConfigurationTypeDef = ...,
         publish: bool = ...,
-        versionDescription: str = ...
+        versionDescription: str = ...,
     ) -> UpdateStateMachineOutputTypeDef:
         """
         Updates an existing state machine by modifying its `definition`, `roleArn`, or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/client/#update_state_machine)
         """
 
     async def update_state_machine_alias(
         self,
         *,
         stateMachineAliasArn: str,
         description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
+        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...,
     ) -> UpdateStateMachineAliasOutputTypeDef:
         """
         Updates the configuration of an existing state machine
         [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-machine-alias.html)
         by modifying its `description` or
         `routingConfiguration`.
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/literals.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/literals.py`

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
     "ExecutionRedriveFilterType",
     "ExecutionRedriveStatusType",
     "ExecutionStatusType",
     "GetExecutionHistoryPaginatorName",
     "HistoryEventTypeType",
     "InspectionLevelType",
@@ -40,15 +39,14 @@
     "SFNServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ExecutionRedriveFilterType = Literal["NOT_REDRIVEN", "REDRIVEN"]
 ExecutionRedriveStatusType = Literal["NOT_REDRIVABLE", "REDRIVABLE", "REDRIVABLE_BY_MAP_RUN"]
 ExecutionStatusType = Literal[
     "ABORTED", "FAILED", "PENDING_REDRIVE", "RUNNING", "SUCCEEDED", "TIMED_OUT"
 ]
 GetExecutionHistoryPaginatorName = Literal["get_execution_history"]
 HistoryEventTypeType = Literal[
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/literals.pyi` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/paginator.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     "GetExecutionHistoryPaginator",
     "ListActivitiesPaginator",
     "ListExecutionsPaginator",
     "ListMapRunsPaginator",
     "ListStateMachinesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -71,15 +70,15 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 
@@ -107,15 +106,15 @@
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
         redriveFilter: ExecutionRedriveFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
         """
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/paginator.pyi` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     def paginate(
         self,
         *,
         executionArn: str,
         reverseOrder: bool = ...,
         includeExecutionData: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetExecutionHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.GetExecutionHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#getexecutionhistorypaginator)
         """
 
 class ListActivitiesPaginator(AioPaginator):
@@ -102,15 +102,15 @@
     def paginate(
         self,
         *,
         stateMachineArn: str = ...,
         statusFilter: ExecutionStatusType = ...,
         mapRunArn: str = ...,
         redriveFilter: ExecutionRedriveFilterType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Paginator.ListExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/paginators/#listexecutionspaginator)
         """
 
 class ListMapRunsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/type_defs.py` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions/type_defs.pyi` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/PKG-INFO` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-stepfunctions
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SFN 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SFN 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/
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
 
 <a id="types-aiobotocore-stepfunctions"></a>
 
 # types-aiobotocore-stepfunctions
 
 [![PyPI - types-aiobotocore-stepfunctions](https://img.shields.io/pypi/v/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-stepfunctions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-stepfunctions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-stepfunctions)](https://pepy.tech/project/types-aiobotocore-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SFN 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[aiobotocore.SFN 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
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
 [types-aiobotocore-stepfunctions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-stepfunctions-2.9.0/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt` & `types-aiobotocore-stepfunctions-2.9.1/types_aiobotocore_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

