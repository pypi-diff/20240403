# Comparing `tmp/types-aiobotocore-connectcases-2.9.0.tar.gz` & `tmp/types-aiobotocore-connectcases-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcases-2.9.0.tar", last modified: Wed Dec 13 19:59:00 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcases-2.9.1.tar", last modified: Thu Jan 18 01:20:26 2024, max compression
```

## Comparing `types-aiobotocore-connectcases-2.9.0.tar` & `types-aiobotocore-connectcases-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.885881 types-aiobotocore-connectcases-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2023-12-13 19:59:00.885881 types-aiobotocore-connectcases-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:00.885881 types-aiobotocore-connectcases-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.881881 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23821 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    23817 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24006 2023-12-13 19:43:35.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24005 2023-12-13 19:43:34.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:33.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:00.885881 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:00.000000 types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:26.705414 types-aiobotocore-connectcases-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-01-18 01:20:26.705414 types-aiobotocore-connectcases-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:26.705414 types-aiobotocore-connectcases-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:05:29.000000 types-aiobotocore-connectcases-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:26.705414 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23829 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23826 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24005 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:30.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:26.705414 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:26.000000 types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcases-2.9.0/LICENSE` & `types-aiobotocore-connectcases-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-connectcases-2.9.0/PKG-INFO` & `types-aiobotocore-connectcases-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConnectCases 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConnectCases 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
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
 
 <a id="types-aiobotocore-connectcases"></a>
 
 # types-aiobotocore-connectcases
 
 [![PyPI - types-aiobotocore-connectcases](https://img.shields.io/pypi/v/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connectcases-2.9.0/README.md` & `types-aiobotocore-connectcases-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connectcases-2.9.0/setup.py` & `types-aiobotocore-connectcases-2.9.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcases",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ConnectCases 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ConnectCases 2.9.1 service generated with"
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
     keywords="aiobotocore connectcases type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_connectcases": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__init__.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import ConnectCasesClient
 from .paginator import SearchCasesPaginator, SearchRelatedItemsPaginator
 
 Client = ConnectCasesClient
 
-
 __all__ = ("Client", "ConnectCasesClient", "SearchCasesPaginator", "SearchRelatedItemsPaginator")
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__init__.pyi` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/__main__.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCases 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ConnectCases 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/client.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ConnectCasesClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -145,15 +144,15 @@
 
     async def create_case(
         self,
         *,
         domainId: str,
         fields: Sequence[FieldValueTypeDef],
         templateId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_case)
         """
@@ -191,15 +190,15 @@
     async def create_related_item(
         self,
         *,
         caseId: str,
         content: RelatedItemInputContentTypeDef,
         domainId: str,
         type: RelatedItemTypeType,
-        performedBy: UserUnionTypeDef = ...
+        performedBy: UserUnionTypeDef = ...,
     ) -> CreateRelatedItemResponseTypeDef:
         """
         Creates a related item (comments, tasks, and contacts) and associates it with a
         case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_related_item)
@@ -209,15 +208,15 @@
         self,
         *,
         domainId: str,
         name: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
         requiredFields: Sequence[RequiredFieldTypeDef] = ...,
-        status: TemplateStatusType = ...
+        status: TemplateStatusType = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_template)
         """
@@ -246,15 +245,15 @@
 
     async def get_case(
         self,
         *,
         caseId: str,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef],
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetCaseResponseTypeDef:
         """
         Returns information about a specific case if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#get_case)
         """
@@ -316,15 +315,15 @@
     async def list_field_options(
         self,
         *,
         domainId: str,
         fieldId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        values: Sequence[str] = ...
+        values: Sequence[str] = ...,
     ) -> ListFieldOptionsResponseTypeDef:
         """
         Lists all of the field options for a field identifier in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_field_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_field_options)
         """
@@ -359,15 +358,15 @@
 
     async def list_templates(
         self,
         *,
         domainId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: Sequence[TemplateStatusType] = ...
+        status: Sequence[TemplateStatusType] = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
@@ -387,15 +386,15 @@
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchTerm: str = ...,
-        sorts: Sequence[SortTypeDef] = ...
+        sorts: Sequence[SortTypeDef] = ...,
     ) -> SearchCasesResponseTypeDef:
         """
         Searches for cases within their associated Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#search_cases)
         """
@@ -403,15 +402,15 @@
     async def search_related_items(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchRelatedItemsResponseTypeDef:
         """
         Searches for related items that are associated with a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#search_related_items)
         """
@@ -471,15 +470,15 @@
         *,
         domainId: str,
         templateId: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
         name: str = ...,
         requiredFields: Sequence[RequiredFieldTypeDef] = ...,
-        status: TemplateStatusType = ...
+        status: TemplateStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_template)
         """
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/client.pyi` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     async def create_case(
         self,
         *,
         domainId: str,
         fields: Sequence[FieldValueTypeDef],
         templateId: str,
-        clientToken: str = ...
+        clientToken: str = ...,
     ) -> CreateCaseResponseTypeDef:
         """
         Creates a case in the specified Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_case)
         """
@@ -187,15 +187,15 @@
     async def create_related_item(
         self,
         *,
         caseId: str,
         content: RelatedItemInputContentTypeDef,
         domainId: str,
         type: RelatedItemTypeType,
-        performedBy: UserUnionTypeDef = ...
+        performedBy: UserUnionTypeDef = ...,
     ) -> CreateRelatedItemResponseTypeDef:
         """
         Creates a related item (comments, tasks, and contacts) and associates it with a
         case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_related_item)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_related_item)
@@ -205,15 +205,15 @@
         self,
         *,
         domainId: str,
         name: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
         requiredFields: Sequence[RequiredFieldTypeDef] = ...,
-        status: TemplateStatusType = ...
+        status: TemplateStatusType = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_template)
         """
@@ -242,15 +242,15 @@
 
     async def get_case(
         self,
         *,
         caseId: str,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef],
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetCaseResponseTypeDef:
         """
         Returns information about a specific case if it exists.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.get_case)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#get_case)
         """
@@ -312,15 +312,15 @@
     async def list_field_options(
         self,
         *,
         domainId: str,
         fieldId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        values: Sequence[str] = ...
+        values: Sequence[str] = ...,
     ) -> ListFieldOptionsResponseTypeDef:
         """
         Lists all of the field options for a field identifier in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_field_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_field_options)
         """
@@ -355,15 +355,15 @@
 
     async def list_templates(
         self,
         *,
         domainId: str,
         maxResults: int = ...,
         nextToken: str = ...,
-        status: Sequence[TemplateStatusType] = ...
+        status: Sequence[TemplateStatusType] = ...,
     ) -> ListTemplatesResponseTypeDef:
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
@@ -383,15 +383,15 @@
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchTerm: str = ...,
-        sorts: Sequence[SortTypeDef] = ...
+        sorts: Sequence[SortTypeDef] = ...,
     ) -> SearchCasesResponseTypeDef:
         """
         Searches for cases within their associated Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_cases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#search_cases)
         """
@@ -399,15 +399,15 @@
     async def search_related_items(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> SearchRelatedItemsResponseTypeDef:
         """
         Searches for related items that are associated with a case.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.search_related_items)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#search_related_items)
         """
@@ -467,15 +467,15 @@
         *,
         domainId: str,
         templateId: str,
         description: str = ...,
         layoutConfiguration: LayoutConfigurationTypeDef = ...,
         name: str = ...,
         requiredFields: Sequence[RequiredFieldTypeDef] = ...,
-        status: TemplateStatusType = ...
+        status: TemplateStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_template)
         """
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/literals.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/literals.py`

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
     "CommentBodyTextTypeType",
     "DomainStatusType",
     "FieldNamespaceType",
     "FieldTypeType",
     "OrderType",
     "RelatedItemTypeType",
@@ -33,15 +32,14 @@
     "ConnectCasesServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 CommentBodyTextTypeType = Literal["Text/Plain"]
 DomainStatusType = Literal["Active", "CreationFailed", "CreationInProgress"]
 FieldNamespaceType = Literal["Custom", "System"]
 FieldTypeType = Literal["Boolean", "DateTime", "Number", "SingleSelect", "Text", "Url"]
 OrderType = Literal["Asc", "Desc"]
 RelatedItemTypeType = Literal["Comment", "Contact"]
 SearchCasesPaginatorName = Literal["search_cases"]
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/literals.pyi` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/paginator.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     SearchCasesResponseTypeDef,
     SearchRelatedItemsResponseTypeDef,
     SortTypeDef,
 )
 
 __all__ = ("SearchCasesPaginator", "SearchRelatedItemsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -61,15 +60,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: CaseFilterTypeDef = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchcasespaginator)
         """
 
 
@@ -81,13 +80,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/paginator.pyi` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: CaseFilterTypeDef = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchcasespaginator)
         """
 
 class SearchRelatedItemsPaginator(AioPaginator):
@@ -77,13 +77,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/type_defs.py` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/type_defs.py`

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
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
     "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases/type_defs.pyi` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/PKG-INFO` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ConnectCases 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ConnectCases 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
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
 
 <a id="types-aiobotocore-connectcases"></a>
 
 # types-aiobotocore-connectcases
 
 [![PyPI - types-aiobotocore-connectcases](https://img.shields.io/pypi/v/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ConnectCases 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
+[aiobotocore.ConnectCases 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-connectcases-2.9.0/types_aiobotocore_connectcases.egg-info/SOURCES.txt` & `types-aiobotocore-connectcases-2.9.1/types_aiobotocore_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*

