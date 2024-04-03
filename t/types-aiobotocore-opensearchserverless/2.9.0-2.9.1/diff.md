# Comparing `tmp/types-aiobotocore-opensearchserverless-2.9.0.tar.gz` & `tmp/types-aiobotocore-opensearchserverless-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opensearchserverless-2.9.0.tar", last modified: Wed Dec 13 20:00:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-opensearchserverless-2.9.1.tar", last modified: Thu Jan 18 01:21:24 2024, max compression
```

## Comparing `types-aiobotocore-opensearchserverless-2.9.0.tar` & `types-aiobotocore-opensearchserverless-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.665370 types-aiobotocore-opensearchserverless-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12993 2023-12-13 20:00:03.665370 types-aiobotocore-opensearchserverless-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:03.665370 types-aiobotocore-opensearchserverless-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.665370 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30305 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30301 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    31007 2023-12-13 19:51:13.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2023-12-13 19:51:13.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:51:10.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:03.665370 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12993 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-13 20:00:03.000000 types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.629143 types-aiobotocore-opensearchserverless-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-01-18 01:21:24.629143 types-aiobotocore-opensearchserverless-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:24.629143 types-aiobotocore-opensearchserverless-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.629143 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30320 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30317 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-01-18 01:12:53.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:12:52.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:24.629143 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-18 01:21:24.000000 types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/LICENSE` & `types-aiobotocore-opensearchserverless-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/PKG-INFO` & `types-aiobotocore-opensearchserverless-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearchserverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/
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
 
 <a id="types-aiobotocore-opensearchserverless"></a>
 
 # types-aiobotocore-opensearchserverless
 
 [![PyPI - types-aiobotocore-opensearchserverless](https://img.shields.io/pypi/v/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [types-aiobotocore-opensearchserverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/README.md` & `types-aiobotocore-opensearchserverless-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [types-aiobotocore-opensearchserverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/setup.py` & `types-aiobotocore-opensearchserverless-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opensearchserverless",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_opensearchserverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore opensearchserverless type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opensearchserverless": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__init__.py` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import OpenSearchServiceServerlessClient
 
 Client = OpenSearchServiceServerlessClient
 
-
 __all__ = ("Client", "OpenSearchServiceServerlessClient")
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__init__.pyi` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/__main__.py` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless\nOther"
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

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/client.py` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("OpenSearchServiceServerlessClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -171,15 +170,15 @@
     async def create_access_policy(
         self,
         *,
         name: str,
         policy: str,
         type: Literal["data"],
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateAccessPolicyResponseTypeDef:
         """
         Creates a data access policy for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_access_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_access_policy)
         """
@@ -188,15 +187,15 @@
         self,
         *,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         standbyReplicas: StandbyReplicasType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        type: CollectionTypeType = ...
+        type: CollectionTypeType = ...,
     ) -> CreateCollectionResponseTypeDef:
         """
         Creates a new OpenSearch Serverless collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_collection)
         """
@@ -204,15 +203,15 @@
     async def create_lifecycle_policy(
         self,
         *,
         name: str,
         policy: str,
         type: Literal["retention"],
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a lifecyle policy to be applied to OpenSearch Serverless indexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_lifecycle_policy)
         """
@@ -220,15 +219,15 @@
     async def create_security_config(
         self,
         *,
         name: str,
         type: Literal["saml"],
         clientToken: str = ...,
         description: str = ...,
-        samlOptions: SamlConfigOptionsTypeDef = ...
+        samlOptions: SamlConfigOptionsTypeDef = ...,
     ) -> CreateSecurityConfigResponseTypeDef:
         """
         Specifies a security configuration for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_security_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_security_config)
         """
@@ -236,15 +235,15 @@
     async def create_security_policy(
         self,
         *,
         name: str,
         policy: str,
         type: SecurityPolicyTypeType,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateSecurityPolicyResponseTypeDef:
         """
         Creates a security policy to be used by one or more OpenSearch Serverless
         collections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_security_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_security_policy)
@@ -253,15 +252,15 @@
     async def create_vpc_endpoint(
         self,
         *,
         name: str,
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        securityGroupIds: Sequence[str] = ...
+        securityGroupIds: Sequence[str] = ...,
     ) -> CreateVpcEndpointResponseTypeDef:
         """
         Creates an OpenSearch Serverless-managed interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_vpc_endpoint)
         """
@@ -386,44 +385,44 @@
 
     async def list_access_policies(
         self,
         *,
         type: Literal["data"],
         maxResults: int = ...,
         nextToken: str = ...,
-        resource: Sequence[str] = ...
+        resource: Sequence[str] = ...,
     ) -> ListAccessPoliciesResponseTypeDef:
         """
         Returns information about a list of OpenSearch Serverless access policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_access_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_access_policies)
         """
 
     async def list_collections(
         self,
         *,
         collectionFilters: CollectionFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCollectionsResponseTypeDef:
         """
         Lists all OpenSearch Serverless collections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_collections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_collections)
         """
 
     async def list_lifecycle_policies(
         self,
         *,
         type: Literal["retention"],
         maxResults: int = ...,
         nextToken: str = ...,
-        resources: Sequence[str] = ...
+        resources: Sequence[str] = ...,
     ) -> ListLifecyclePoliciesResponseTypeDef:
         """
         Returns a list of OpenSearch Serverless lifecycle policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_lifecycle_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_lifecycle_policies)
         """
@@ -441,15 +440,15 @@
 
     async def list_security_policies(
         self,
         *,
         type: SecurityPolicyTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        resource: Sequence[str] = ...
+        resource: Sequence[str] = ...,
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
         Returns information about configured OpenSearch Serverless security policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_security_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_security_policies)
         """
@@ -465,15 +464,15 @@
         """
 
     async def list_vpc_endpoints(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        vpcEndpointFilters: VpcEndpointFiltersTypeDef = ...
+        vpcEndpointFilters: VpcEndpointFiltersTypeDef = ...,
     ) -> ListVpcEndpointsResponseTypeDef:
         """
         Returns the OpenSearch Serverless-managed interface VPC endpoints associated
         with the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_vpc_endpoints)
@@ -500,15 +499,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: Literal["data"],
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateAccessPolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless access policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_access_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_access_policy)
         """
@@ -538,15 +537,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: Literal["retention"],
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateLifecyclePolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless access policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_lifecycle_policy)
         """
@@ -554,15 +553,15 @@
     async def update_security_config(
         self,
         *,
         configVersion: str,
         id: str,
         clientToken: str = ...,
         description: str = ...,
-        samlOptions: SamlConfigOptionsTypeDef = ...
+        samlOptions: SamlConfigOptionsTypeDef = ...,
     ) -> UpdateSecurityConfigResponseTypeDef:
         """
         Updates a security configuration for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_security_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_security_config)
         """
@@ -571,15 +570,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: SecurityPolicyTypeType,
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateSecurityPolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless security policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_security_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_security_policy)
         """
@@ -588,15 +587,15 @@
         self,
         *,
         id: str,
         addSecurityGroupIds: Sequence[str] = ...,
         addSubnetIds: Sequence[str] = ...,
         clientToken: str = ...,
         removeSecurityGroupIds: Sequence[str] = ...,
-        removeSubnetIds: Sequence[str] = ...
+        removeSubnetIds: Sequence[str] = ...,
     ) -> UpdateVpcEndpointResponseTypeDef:
         """
         Updates an OpenSearch Serverless-managed interface endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_vpc_endpoint)
         """
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/client.pyi` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     async def create_access_policy(
         self,
         *,
         name: str,
         policy: str,
         type: Literal["data"],
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateAccessPolicyResponseTypeDef:
         """
         Creates a data access policy for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_access_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_access_policy)
         """
@@ -184,15 +184,15 @@
         self,
         *,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         standbyReplicas: StandbyReplicasType = ...,
         tags: Sequence[TagTypeDef] = ...,
-        type: CollectionTypeType = ...
+        type: CollectionTypeType = ...,
     ) -> CreateCollectionResponseTypeDef:
         """
         Creates a new OpenSearch Serverless collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_collection)
         """
@@ -200,15 +200,15 @@
     async def create_lifecycle_policy(
         self,
         *,
         name: str,
         policy: str,
         type: Literal["retention"],
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateLifecyclePolicyResponseTypeDef:
         """
         Creates a lifecyle policy to be applied to OpenSearch Serverless indexes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_lifecycle_policy)
         """
@@ -216,15 +216,15 @@
     async def create_security_config(
         self,
         *,
         name: str,
         type: Literal["saml"],
         clientToken: str = ...,
         description: str = ...,
-        samlOptions: SamlConfigOptionsTypeDef = ...
+        samlOptions: SamlConfigOptionsTypeDef = ...,
     ) -> CreateSecurityConfigResponseTypeDef:
         """
         Specifies a security configuration for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_security_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_security_config)
         """
@@ -232,15 +232,15 @@
     async def create_security_policy(
         self,
         *,
         name: str,
         policy: str,
         type: SecurityPolicyTypeType,
         clientToken: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> CreateSecurityPolicyResponseTypeDef:
         """
         Creates a security policy to be used by one or more OpenSearch Serverless
         collections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_security_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_security_policy)
@@ -249,15 +249,15 @@
     async def create_vpc_endpoint(
         self,
         *,
         name: str,
         subnetIds: Sequence[str],
         vpcId: str,
         clientToken: str = ...,
-        securityGroupIds: Sequence[str] = ...
+        securityGroupIds: Sequence[str] = ...,
     ) -> CreateVpcEndpointResponseTypeDef:
         """
         Creates an OpenSearch Serverless-managed interface VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#create_vpc_endpoint)
         """
@@ -382,44 +382,44 @@
 
     async def list_access_policies(
         self,
         *,
         type: Literal["data"],
         maxResults: int = ...,
         nextToken: str = ...,
-        resource: Sequence[str] = ...
+        resource: Sequence[str] = ...,
     ) -> ListAccessPoliciesResponseTypeDef:
         """
         Returns information about a list of OpenSearch Serverless access policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_access_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_access_policies)
         """
 
     async def list_collections(
         self,
         *,
         collectionFilters: CollectionFiltersTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListCollectionsResponseTypeDef:
         """
         Lists all OpenSearch Serverless collections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_collections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_collections)
         """
 
     async def list_lifecycle_policies(
         self,
         *,
         type: Literal["retention"],
         maxResults: int = ...,
         nextToken: str = ...,
-        resources: Sequence[str] = ...
+        resources: Sequence[str] = ...,
     ) -> ListLifecyclePoliciesResponseTypeDef:
         """
         Returns a list of OpenSearch Serverless lifecycle policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_lifecycle_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_lifecycle_policies)
         """
@@ -437,15 +437,15 @@
 
     async def list_security_policies(
         self,
         *,
         type: SecurityPolicyTypeType,
         maxResults: int = ...,
         nextToken: str = ...,
-        resource: Sequence[str] = ...
+        resource: Sequence[str] = ...,
     ) -> ListSecurityPoliciesResponseTypeDef:
         """
         Returns information about configured OpenSearch Serverless security policies.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_security_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#list_security_policies)
         """
@@ -461,15 +461,15 @@
         """
 
     async def list_vpc_endpoints(
         self,
         *,
         maxResults: int = ...,
         nextToken: str = ...,
-        vpcEndpointFilters: VpcEndpointFiltersTypeDef = ...
+        vpcEndpointFilters: VpcEndpointFiltersTypeDef = ...,
     ) -> ListVpcEndpointsResponseTypeDef:
         """
         Returns the OpenSearch Serverless-managed interface VPC endpoints associated
         with the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.list_vpc_endpoints)
@@ -496,15 +496,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: Literal["data"],
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateAccessPolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless access policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_access_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_access_policy)
         """
@@ -534,15 +534,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: Literal["retention"],
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateLifecyclePolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless access policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_lifecycle_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_lifecycle_policy)
         """
@@ -550,15 +550,15 @@
     async def update_security_config(
         self,
         *,
         configVersion: str,
         id: str,
         clientToken: str = ...,
         description: str = ...,
-        samlOptions: SamlConfigOptionsTypeDef = ...
+        samlOptions: SamlConfigOptionsTypeDef = ...,
     ) -> UpdateSecurityConfigResponseTypeDef:
         """
         Updates a security configuration for OpenSearch Serverless.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_security_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_security_config)
         """
@@ -567,15 +567,15 @@
         self,
         *,
         name: str,
         policyVersion: str,
         type: SecurityPolicyTypeType,
         clientToken: str = ...,
         description: str = ...,
-        policy: str = ...
+        policy: str = ...,
     ) -> UpdateSecurityPolicyResponseTypeDef:
         """
         Updates an OpenSearch Serverless security policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_security_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_security_policy)
         """
@@ -584,15 +584,15 @@
         self,
         *,
         id: str,
         addSecurityGroupIds: Sequence[str] = ...,
         addSubnetIds: Sequence[str] = ...,
         clientToken: str = ...,
         removeSecurityGroupIds: Sequence[str] = ...,
-        removeSubnetIds: Sequence[str] = ...
+        removeSubnetIds: Sequence[str] = ...,
     ) -> UpdateVpcEndpointResponseTypeDef:
         """
         Updates an OpenSearch Serverless-managed interface endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless.Client.update_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/client/#update_vpc_endpoint)
         """
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/literals.py` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/literals.py`

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
     "AccessPolicyTypeType",
     "CollectionStatusType",
     "CollectionTypeType",
     "LifecyclePolicyTypeType",
     "ResourceTypeType",
     "SecurityConfigTypeType",
@@ -32,15 +31,14 @@
     "VpcEndpointStatusType",
     "OpenSearchServiceServerlessServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AccessPolicyTypeType = Literal["data"]
 CollectionStatusType = Literal["ACTIVE", "CREATING", "DELETING", "FAILED"]
 CollectionTypeType = Literal["SEARCH", "TIMESERIES", "VECTORSEARCH"]
 LifecyclePolicyTypeType = Literal["retention"]
 ResourceTypeType = Literal["index"]
 SecurityConfigTypeType = Literal["saml"]
 SecurityPolicyTypeType = Literal["encryption", "network"]
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/literals.pyi` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/type_defs.py` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessPolicyDetailTypeDef",
     "AccessPolicyStatsTypeDef",
     "AccessPolicySummaryTypeDef",
     "CapacityLimitsTypeDef",
     "BatchGetCollectionRequestRequestTypeDef",
     "CollectionDetailTypeDef",
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless/type_defs.pyi` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opensearchserverless
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.OpenSearchServiceServerless 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/
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
 
 <a id="types-aiobotocore-opensearchserverless"></a>
 
 # types-aiobotocore-opensearchserverless
 
 [![PyPI - types-aiobotocore-opensearchserverless](https://img.shields.io/pypi/v/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opensearchserverless.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opensearchserverless)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opensearchserverless)](https://pepy.tech/project/types-aiobotocore-opensearchserverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.OpenSearchServiceServerless 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
+[aiobotocore.OpenSearchServiceServerless 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#OpenSearchServiceServerless)
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
 [types-aiobotocore-opensearchserverless docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opensearchserverless/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-opensearchserverless-2.9.0/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt` & `types-aiobotocore-opensearchserverless-2.9.1/types_aiobotocore_opensearchserverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

