# Comparing `tmp/types-aiobotocore-honeycode-2.9.0.tar.gz` & `tmp/types-aiobotocore-honeycode-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-honeycode-2.9.0.tar", last modified: Wed Dec 13 19:59:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-honeycode-2.9.1.tar", last modified: Thu Jan 18 01:20:50 2024, max compression
```

## Comparing `types-aiobotocore-honeycode-2.9.0.tar` & `types-aiobotocore-honeycode-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.545702 types-aiobotocore-honeycode-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-12-13 19:59:26.545702 types-aiobotocore-honeycode-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11874 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:26.545702 types-aiobotocore-honeycode-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.545702 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16976 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9736 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9734 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5461 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15836 2023-12-13 19:47:15.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15835 2023-12-13 19:47:14.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:47:12.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:26.545702 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 19:59:26.000000 types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.453297 types-aiobotocore-honeycode-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-01-18 01:20:50.449297 types-aiobotocore-honeycode-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11874 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:50.453297 types-aiobotocore-honeycode-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.449297 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16983 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16980 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-01-18 01:09:05.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9734 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5463 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15835 2024-01-18 01:09:05.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15835 2024-01-18 01:09:05.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:09:04.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:50.449297 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13465 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:20:50.000000 types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-honeycode-2.9.0/LICENSE` & `types-aiobotocore-honeycode-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-honeycode-2.9.0/PKG-INFO` & `types-aiobotocore-honeycode-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Honeycode 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Honeycode 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
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
 
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-honeycode-2.9.0/README.md` & `types-aiobotocore-honeycode-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-honeycode-2.9.0/setup.py` & `types-aiobotocore-honeycode-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-honeycode",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Honeycode 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Honeycode 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore honeycode type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_honeycode": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__init__.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListTableRowsPaginator,
     ListTablesPaginator,
     QueryTableRowsPaginator,
 )
 
 Client = HoneycodeClient
 
-
 __all__ = (
     "Client",
     "HoneycodeClient",
     "ListTableColumnsPaginator",
     "ListTableRowsPaginator",
     "ListTablesPaginator",
     "QueryTableRowsPaginator",
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__init__.pyi` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/__main__.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Honeycode 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Honeycode 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/client.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("HoneycodeClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -100,15 +99,15 @@
 
     async def batch_create_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToCreate: Sequence[CreateRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchCreateTableRowsResultTypeDef:
         """
         The BatchCreateTableRows API allows you to create one or more rows at the end
         of a table in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_create_table_rows)
@@ -129,15 +128,15 @@
 
     async def batch_update_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToUpdate: Sequence[UpdateRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchUpdateTableRowsResultTypeDef:
         """
         The BatchUpdateTableRows API allows you to update one or more rows in a table
         in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_update_table_rows)
@@ -146,15 +145,15 @@
 
     async def batch_upsert_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToUpsert: Sequence[UpsertRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchUpsertTableRowsResultTypeDef:
         """
         The BatchUpsertTableRows API allows you to upsert one or more rows in a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_upsert_table_rows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#batch_upsert_table_rows)
         """
@@ -205,15 +204,15 @@
         self,
         *,
         workbookId: str,
         appId: str,
         screenId: str,
         variables: Mapping[str, VariableValueTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetScreenDataResultTypeDef:
         """
         The GetScreenData API allows retrieval of data from a screen in a Honeycode app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.get_screen_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#get_screen_data)
         """
@@ -223,15 +222,15 @@
         *,
         workbookId: str,
         appId: str,
         screenId: str,
         screenAutomationId: str,
         variables: Mapping[str, VariableValueTypeDef] = ...,
         rowId: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> InvokeScreenAutomationResultTypeDef:
         """
         The InvokeScreenAutomation API allows invoking an action defined in a screen in
         a Honeycode
         app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.invoke_screen_automation)
@@ -253,15 +252,15 @@
     async def list_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTableRowsResultTypeDef:
         """
         The ListTableRows API allows you to retrieve a list of all the rows in a table
         in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.list_table_rows)
@@ -290,15 +289,15 @@
     async def query_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> QueryTableRowsResultTypeDef:
         """
         The QueryTableRows API allows you to use a filter formula to query for specific
         rows in a
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.query_table_rows)
@@ -309,15 +308,15 @@
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
         importOptions: ImportOptionsTypeDef,
-        clientRequestToken: str
+        clientRequestToken: str,
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
         """
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/client.pyi` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
     async def batch_create_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToCreate: Sequence[CreateRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchCreateTableRowsResultTypeDef:
         """
         The BatchCreateTableRows API allows you to create one or more rows at the end
         of a table in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_create_table_rows)
@@ -125,15 +125,15 @@
 
     async def batch_update_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToUpdate: Sequence[UpdateRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchUpdateTableRowsResultTypeDef:
         """
         The BatchUpdateTableRows API allows you to update one or more rows in a table
         in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_update_table_rows)
@@ -142,15 +142,15 @@
 
     async def batch_upsert_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowsToUpsert: Sequence[UpsertRowDataTypeDef],
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> BatchUpsertTableRowsResultTypeDef:
         """
         The BatchUpsertTableRows API allows you to upsert one or more rows in a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.batch_upsert_table_rows)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#batch_upsert_table_rows)
         """
@@ -201,15 +201,15 @@
         self,
         *,
         workbookId: str,
         appId: str,
         screenId: str,
         variables: Mapping[str, VariableValueTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> GetScreenDataResultTypeDef:
         """
         The GetScreenData API allows retrieval of data from a screen in a Honeycode app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.get_screen_data)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#get_screen_data)
         """
@@ -219,15 +219,15 @@
         *,
         workbookId: str,
         appId: str,
         screenId: str,
         screenAutomationId: str,
         variables: Mapping[str, VariableValueTypeDef] = ...,
         rowId: str = ...,
-        clientRequestToken: str = ...
+        clientRequestToken: str = ...,
     ) -> InvokeScreenAutomationResultTypeDef:
         """
         The InvokeScreenAutomation API allows invoking an action defined in a screen in
         a Honeycode
         app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.invoke_screen_automation)
@@ -249,15 +249,15 @@
     async def list_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListTableRowsResultTypeDef:
         """
         The ListTableRows API allows you to retrieve a list of all the rows in a table
         in a
         workbook.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.list_table_rows)
@@ -286,15 +286,15 @@
     async def query_table_rows(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> QueryTableRowsResultTypeDef:
         """
         The QueryTableRows API allows you to use a filter formula to query for specific
         rows in a
         table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.query_table_rows)
@@ -305,15 +305,15 @@
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
         importOptions: ImportOptionsTypeDef,
-        clientRequestToken: str
+        clientRequestToken: str,
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
         """
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/literals.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/literals.py`

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
     "ErrorCodeType",
     "FormatType",
     "ImportDataCharacterEncodingType",
     "ImportSourceDataFormatType",
     "ListTableColumnsPaginatorName",
     "ListTableRowsPaginatorName",
@@ -34,15 +33,14 @@
     "HoneycodeServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ErrorCodeType = Literal[
     "ACCESS_DENIED",
     "FILE_EMPTY_ERROR",
     "FILE_NOT_FOUND_ERROR",
     "FILE_PARSING_ERROR",
     "FILE_SIZE_LIMIT_ERROR",
     "INVALID_FILE_TYPE_ERROR",
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/literals.pyi` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/paginator.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 __all__ = (
     "ListTableColumnsPaginator",
     "ListTableRowsPaginator",
     "ListTablesPaginator",
     "QueryTableRowsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -82,15 +81,15 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablerowspaginator)
         """
 
 
@@ -117,13 +116,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/paginator.pyi` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablerowspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
@@ -111,13 +111,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/type_defs.py` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FailedBatchItemTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode/type_defs.pyi` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/PKG-INFO` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Honeycode 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Honeycode 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
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
 
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Honeycode 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[aiobotocore.Honeycode 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-honeycode-2.9.0/types_aiobotocore_honeycode.egg-info/SOURCES.txt` & `types-aiobotocore-honeycode-2.9.1/types_aiobotocore_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

