# Comparing `tmp/types-aiobotocore-directconnect-2.9.0.tar.gz` & `tmp/types-aiobotocore-directconnect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-directconnect-2.9.0.tar", last modified: Wed Dec 13 19:59:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-directconnect-2.9.1.tar", last modified: Thu Jan 18 01:20:31 2024, max compression
```

## Comparing `types-aiobotocore-directconnect-2.9.0.tar` & `types-aiobotocore-directconnect-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.457835 types-aiobotocore-directconnect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13887 2023-12-13 19:59:06.457835 types-aiobotocore-directconnect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12300 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:06.457835 types-aiobotocore-directconnect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.453835 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      956 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49903 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    49899 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11411 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11409 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    50222 2023-12-13 19:44:09.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50221 2023-12-13 19:44:08.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:44:07.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:06.457835 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13887 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      927 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-12-13 19:59:06.000000 types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.861387 types-aiobotocore-directconnect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-01-18 01:20:31.861387 types-aiobotocore-directconnect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:31.861387 types-aiobotocore-directconnect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.861387 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49926 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49923 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11409 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    50221 2024-01-18 01:06:04.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50221 2024-01-18 01:06:03.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:06:02.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:31.861387 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-01-18 01:20:31.000000 types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-directconnect-2.9.0/LICENSE` & `types-aiobotocore-directconnect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-directconnect-2.9.0/PKG-INFO` & `types-aiobotocore-directconnect-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-directconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DirectConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DirectConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/
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
 
 <a id="types-aiobotocore-directconnect"></a>
 
 # types-aiobotocore-directconnect
 
 [![PyPI - types-aiobotocore-directconnect](https://img.shields.io/pypi/v/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[aiobotocore.DirectConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-directconnect-2.9.0/README.md` & `types-aiobotocore-directconnect-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[aiobotocore.DirectConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-directconnect-2.9.0/setup.py` & `types-aiobotocore-directconnect-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-directconnect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DirectConnect 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DirectConnect 2.9.1 service generated with"
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
     keywords="aiobotocore directconnect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_directconnect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__init__.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     DescribeDirectConnectGatewayAssociationsPaginator,
     DescribeDirectConnectGatewayAttachmentsPaginator,
     DescribeDirectConnectGatewaysPaginator,
 )
 
 Client = DirectConnectClient
 
-
 __all__ = (
     "Client",
     "DescribeDirectConnectGatewayAssociationsPaginator",
     "DescribeDirectConnectGatewayAttachmentsPaginator",
     "DescribeDirectConnectGatewaysPaginator",
     "DirectConnectClient",
 )
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__init__.pyi` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/__main__.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectConnect 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DirectConnect 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
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

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/client.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DirectConnectClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -127,15 +126,15 @@
 
     async def accept_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         proposalId: str,
         associatedGatewayOwnerAccount: str,
-        overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> AcceptDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Accepts a proposal request to attach a virtual private gateway or transit
         gateway to a Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.accept_direct_connect_gateway_association_proposal)
@@ -145,15 +144,15 @@
     async def allocate_connection_on_interconnect(
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
-        vlan: int
+        vlan: int,
     ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_connection_on_interconnect)
         """
@@ -162,15 +161,15 @@
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of
         interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
@@ -178,15 +177,15 @@
         """
 
     async def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
+        newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
@@ -194,15 +193,15 @@
         """
 
     async def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
+        newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
@@ -210,15 +209,15 @@
         """
 
     async def allocate_transit_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef
+        newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef,
     ) -> AllocateTransitVirtualInterfaceResultTypeDef:
         """
         Provisions a transit virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
@@ -307,15 +306,15 @@
         """
 
     async def confirm_private_virtual_interface(
         self,
         *,
         virtualInterfaceId: str,
         virtualGatewayId: str = ...,
-        directConnectGatewayId: str = ...
+        directConnectGatewayId: str = ...,
     ) -> ConfirmPrivateVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a private virtual interface created by another Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_private_virtual_interface)
@@ -361,15 +360,15 @@
         *,
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
-        requestMACSec: bool = ...
+        requestMACSec: bool = ...,
     ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_connection)
@@ -389,15 +388,15 @@
 
     async def create_direct_connect_gateway_association(
         self,
         *,
         directConnectGatewayId: str,
         gatewayId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> CreateDirectConnectGatewayAssociationResultTypeDef:
         """
         Creates an association between a Direct Connect gateway and a virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association)
@@ -406,15 +405,15 @@
     async def create_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         directConnectGatewayOwnerAccount: str,
         gatewayId: str,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> CreateDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Creates a proposal to associate the specified virtual private gateway or
         transit gateway with the specified Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association_proposal)
@@ -425,15 +424,15 @@
         self,
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        providerName: str = ...
+        providerName: str = ...,
     ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
@@ -447,15 +446,15 @@
         location: str,
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
-        requestMACSec: bool = ...
+        requestMACSec: bool = ...,
     ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect
         location.
 
@@ -495,15 +494,15 @@
 
     async def delete_bgp_peer(
         self,
         *,
         virtualInterfaceId: str = ...,
         asn: int = ...,
         customerAddress: str = ...,
-        bgpPeerId: str = ...
+        bgpPeerId: str = ...,
     ) -> DeleteBGPPeerResponseTypeDef:
         """
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and
         ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
@@ -529,15 +528,15 @@
         """
 
     async def delete_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         directConnectGatewayId: str = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> DeleteDirectConnectGatewayAssociationResultTypeDef:
         """
         Deletes the association between the specified Direct Connect gateway and
         virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association)
@@ -585,15 +584,15 @@
         """
 
     async def describe_connection_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> DescribeConnectionLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connection_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connection_loa)
         """
@@ -629,15 +628,15 @@
     async def describe_direct_connect_gateway_association_proposals(
         self,
         *,
         directConnectGatewayId: str = ...,
         proposalId: str = ...,
         associatedGatewayId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeDirectConnectGatewayAssociationProposalsResultTypeDef:
         """
         Describes one or more association proposals for connection between a virtual
         private gateway or transit gateway and a Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_association_proposals)
@@ -648,15 +647,15 @@
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> DescribeDirectConnectGatewayAssociationsResultTypeDef:
         """
         Lists the associations between your Direct Connect gateways and virtual private
         gateways and transit
         gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_associations)
@@ -665,15 +664,15 @@
 
     async def describe_direct_connect_gateway_attachments(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeDirectConnectGatewayAttachmentsResultTypeDef:
         """
         Lists the attachments between your Direct Connect gateways and virtual
         interfaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_attachments)
@@ -701,15 +700,15 @@
         """
 
     async def describe_interconnect_loa(
         self,
         *,
         interconnectId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> DescribeInterconnectLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnect_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnect_loa)
         """
@@ -733,15 +732,15 @@
         """
 
     async def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_loa)
@@ -831,29 +830,29 @@
         self,
         *,
         testId: str = ...,
         virtualInterfaceId: str = ...,
         bgpPeers: Sequence[str] = ...,
         status: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListVirtualInterfaceTestHistoryResponseTypeDef:
         """
         Lists the virtual interface failover test history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.list_virtual_interface_test_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#list_virtual_interface_test_history)
         """
 
     async def start_bgp_failover_test(
         self,
         *,
         virtualInterfaceId: str,
         bgpPeers: Sequence[str] = ...,
-        testDurationInMinutes: int = ...
+        testDurationInMinutes: int = ...,
     ) -> StartBgpFailoverTestResponseTypeDef:
         """
         Starts the virtual interface failover test that verifies your configuration
         meets your resiliency requirements by placing the BGP peering session in the
         DOWN
         state.
 
@@ -908,15 +907,15 @@
         """
 
     async def update_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> UpdateDirectConnectGatewayAssociationResultTypeDef:
         """
         Updates the specified attributes of the Direct Connect gateway association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway_association)
         """
@@ -933,15 +932,15 @@
 
     async def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
-        virtualInterfaceName: str = ...
+        virtualInterfaceName: str = ...,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_virtual_interface_attributes)
         """
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/client.pyi` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
 
     async def accept_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         proposalId: str,
         associatedGatewayOwnerAccount: str,
-        overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> AcceptDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Accepts a proposal request to attach a virtual private gateway or transit
         gateway to a Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.accept_direct_connect_gateway_association_proposal)
@@ -141,15 +141,15 @@
     async def allocate_connection_on_interconnect(
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
-        vlan: int
+        vlan: int,
     ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_connection_on_interconnect)
         """
@@ -158,15 +158,15 @@
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
-        tags: Sequence[TagTypeDef] = ...
+        tags: Sequence[TagTypeDef] = ...,
     ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of
         interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
@@ -174,15 +174,15 @@
         """
 
     async def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
+        newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
@@ -190,15 +190,15 @@
         """
 
     async def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
+        newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
@@ -206,15 +206,15 @@
         """
 
     async def allocate_transit_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
-        newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef
+        newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef,
     ) -> AllocateTransitVirtualInterfaceResultTypeDef:
         """
         Provisions a transit virtual interface to be owned by the specified Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
@@ -303,15 +303,15 @@
         """
 
     async def confirm_private_virtual_interface(
         self,
         *,
         virtualInterfaceId: str,
         virtualGatewayId: str = ...,
-        directConnectGatewayId: str = ...
+        directConnectGatewayId: str = ...,
     ) -> ConfirmPrivateVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a private virtual interface created by another Amazon Web
         Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_private_virtual_interface)
@@ -357,15 +357,15 @@
         *,
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
-        requestMACSec: bool = ...
+        requestMACSec: bool = ...,
     ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_connection)
@@ -385,15 +385,15 @@
 
     async def create_direct_connect_gateway_association(
         self,
         *,
         directConnectGatewayId: str,
         gatewayId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> CreateDirectConnectGatewayAssociationResultTypeDef:
         """
         Creates an association between a Direct Connect gateway and a virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association)
@@ -402,15 +402,15 @@
     async def create_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         directConnectGatewayOwnerAccount: str,
         gatewayId: str,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> CreateDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Creates a proposal to associate the specified virtual private gateway or
         transit gateway with the specified Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association_proposal)
@@ -421,15 +421,15 @@
         self,
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        providerName: str = ...
+        providerName: str = ...,
     ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
@@ -443,15 +443,15 @@
         location: str,
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
-        requestMACSec: bool = ...
+        requestMACSec: bool = ...,
     ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect
         location.
 
@@ -491,15 +491,15 @@
 
     async def delete_bgp_peer(
         self,
         *,
         virtualInterfaceId: str = ...,
         asn: int = ...,
         customerAddress: str = ...,
-        bgpPeerId: str = ...
+        bgpPeerId: str = ...,
     ) -> DeleteBGPPeerResponseTypeDef:
         """
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and
         ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
@@ -525,15 +525,15 @@
         """
 
     async def delete_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         directConnectGatewayId: str = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> DeleteDirectConnectGatewayAssociationResultTypeDef:
         """
         Deletes the association between the specified Direct Connect gateway and
         virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association)
@@ -581,15 +581,15 @@
         """
 
     async def describe_connection_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> DescribeConnectionLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connection_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connection_loa)
         """
@@ -625,15 +625,15 @@
     async def describe_direct_connect_gateway_association_proposals(
         self,
         *,
         directConnectGatewayId: str = ...,
         proposalId: str = ...,
         associatedGatewayId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeDirectConnectGatewayAssociationProposalsResultTypeDef:
         """
         Describes one or more association proposals for connection between a virtual
         private gateway or transit gateway and a Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_association_proposals)
@@ -644,15 +644,15 @@
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        virtualGatewayId: str = ...
+        virtualGatewayId: str = ...,
     ) -> DescribeDirectConnectGatewayAssociationsResultTypeDef:
         """
         Lists the associations between your Direct Connect gateways and virtual private
         gateways and transit
         gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_associations)
@@ -661,15 +661,15 @@
 
     async def describe_direct_connect_gateway_attachments(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeDirectConnectGatewayAttachmentsResultTypeDef:
         """
         Lists the attachments between your Direct Connect gateways and virtual
         interfaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_attachments)
@@ -697,15 +697,15 @@
         """
 
     async def describe_interconnect_loa(
         self,
         *,
         interconnectId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> DescribeInterconnectLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnect_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnect_loa)
         """
@@ -729,15 +729,15 @@
         """
 
     async def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
-        loaContentType: Literal["application/pdf"] = ...
+        loaContentType: Literal["application/pdf"] = ...,
     ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_loa)
@@ -827,29 +827,29 @@
         self,
         *,
         testId: str = ...,
         virtualInterfaceId: str = ...,
         bgpPeers: Sequence[str] = ...,
         status: str = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListVirtualInterfaceTestHistoryResponseTypeDef:
         """
         Lists the virtual interface failover test history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.list_virtual_interface_test_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#list_virtual_interface_test_history)
         """
 
     async def start_bgp_failover_test(
         self,
         *,
         virtualInterfaceId: str,
         bgpPeers: Sequence[str] = ...,
-        testDurationInMinutes: int = ...
+        testDurationInMinutes: int = ...,
     ) -> StartBgpFailoverTestResponseTypeDef:
         """
         Starts the virtual interface failover test that verifies your configuration
         meets your resiliency requirements by placing the BGP peering session in the
         DOWN
         state.
 
@@ -904,15 +904,15 @@
         """
 
     async def update_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
-        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
+        removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
     ) -> UpdateDirectConnectGatewayAssociationResultTypeDef:
         """
         Updates the specified attributes of the Direct Connect gateway association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway_association)
         """
@@ -929,15 +929,15 @@
 
     async def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
-        virtualInterfaceName: str = ...
+        virtualInterfaceName: str = ...,
     ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_virtual_interface_attributes)
         """
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/literals.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/literals.py`

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
     "AddressFamilyType",
     "BGPPeerStateType",
     "BGPStatusType",
     "ConnectionStateType",
     "DescribeDirectConnectGatewayAssociationsPaginatorName",
     "DescribeDirectConnectGatewayAttachmentsPaginatorName",
@@ -43,15 +42,14 @@
     "DirectConnectServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AddressFamilyType = Literal["ipv4", "ipv6"]
 BGPPeerStateType = Literal["available", "deleted", "deleting", "pending", "verifying"]
 BGPStatusType = Literal["down", "unknown", "up"]
 ConnectionStateType = Literal[
     "available",
     "deleted",
     "deleting",
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/literals.pyi` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/paginator.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -39,65 +39,60 @@
 
 __all__ = (
     "DescribeDirectConnectGatewayAssociationsPaginator",
     "DescribeDirectConnectGatewayAttachmentsPaginator",
     "DescribeDirectConnectGatewaysPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeDirectConnectGatewayAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
-
 class DescribeDirectConnectGatewayAttachmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
-
 class DescribeDirectConnectGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/paginator.pyi` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,58 +41,62 @@
     "DescribeDirectConnectGatewayAssociationsPaginator",
     "DescribeDirectConnectGatewayAttachmentsPaginator",
     "DescribeDirectConnectGatewaysPaginator",
 )
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeDirectConnectGatewayAssociationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
+
 class DescribeDirectConnectGatewayAttachmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
+
 class DescribeDirectConnectGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/type_defs.py` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "RouteFilterPrefixTypeDef",
     "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect/type_defs.pyi` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/PKG-INFO` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-directconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DirectConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DirectConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/
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
 
 <a id="types-aiobotocore-directconnect"></a>
 
 # types-aiobotocore-directconnect
 
 [![PyPI - types-aiobotocore-directconnect](https://img.shields.io/pypi/v/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DirectConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[aiobotocore.DirectConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-directconnect-2.9.0/types_aiobotocore_directconnect.egg-info/SOURCES.txt` & `types-aiobotocore-directconnect-2.9.1/types_aiobotocore_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

