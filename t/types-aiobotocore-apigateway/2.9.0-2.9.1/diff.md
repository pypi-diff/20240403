# Comparing `tmp/types-aiobotocore-apigateway-2.9.0.tar.gz` & `tmp/types-aiobotocore-apigateway-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigateway-2.9.0.tar", last modified: Wed Dec 13 19:58:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigateway-2.9.1.tar", last modified: Thu Jan 18 01:20:00 2024, max compression
```

## Comparing `types-aiobotocore-apigateway-2.9.0.tar` & `types-aiobotocore-apigateway-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:32.002117 types-aiobotocore-apigateway-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2023-12-13 19:58:32.002117 types-aiobotocore-apigateway-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13891 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:32.002117 types-aiobotocore-apigateway-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:31.998117 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86655 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    86651 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13558 2023-12-13 19:40:51.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13556 2023-12-13 19:40:51.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20981 2023-12-13 19:40:51.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20961 2023-12-13 19:40:51.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    76086 2023-12-13 19:40:52.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    76085 2023-12-13 19:40:52.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:50.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:32.002117 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15466 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 19:58:31.000000 types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:00.321527 types-aiobotocore-apigateway-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-01-18 01:20:00.317527 types-aiobotocore-apigateway-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:00.321527 types-aiobotocore-apigateway-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:00.317527 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86693 2024-01-18 01:02:50.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86690 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-01-18 01:02:50.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13556 2024-01-18 01:02:50.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20985 2024-01-18 01:02:50.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20966 2024-01-18 01:02:50.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    76085 2024-01-18 01:02:52.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76085 2024-01-18 01:02:51.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:49.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:00.317527 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15486 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-18 01:20:00.000000 types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigateway-2.9.0/LICENSE` & `types-aiobotocore-apigateway-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-apigateway-2.9.0/PKG-INFO` & `types-aiobotocore-apigateway-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.APIGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.APIGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/
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
 
 <a id="types-aiobotocore-apigateway"></a>
 
 # types-aiobotocore-apigateway
 
 [![PyPI - types-aiobotocore-apigateway](https://img.shields.io/pypi/v/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigateway)](https://pepy.tech/project/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [types-aiobotocore-apigateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigateway-2.9.0/README.md` & `types-aiobotocore-apigateway-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigateway)](https://pepy.tech/project/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [types-aiobotocore-apigateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigateway-2.9.0/setup.py` & `types-aiobotocore-apigateway-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigateway",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_apigateway"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.APIGateway 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.APIGateway 2.9.1 service generated with"
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
     keywords="aiobotocore apigateway type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_apigateway": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__init__.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     GetUsagePlanKeysPaginator,
     GetUsagePlansPaginator,
     GetVpcLinksPaginator,
 )
 
 Client = APIGatewayClient
 
-
 __all__ = (
     "APIGatewayClient",
     "Client",
     "GetApiKeysPaginator",
     "GetAuthorizersPaginator",
     "GetBasePathMappingsPaginator",
     "GetClientCertificatesPaginator",
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__init__.pyi` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/__main__.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.APIGateway 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.APIGateway 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway\nOther"
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

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/client.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("APIGatewayClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -187,15 +186,15 @@
         name: str = ...,
         description: str = ...,
         enabled: bool = ...,
         generateDistinctId: bool = ...,
         value: str = ...,
         stageKeys: Sequence[StageKeyTypeDef] = ...,
         customerId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApiKeyResponseTypeDef:
         """
         Create an ApiKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_api_key)
         """
@@ -208,15 +207,15 @@
         type: AuthorizerTypeType,
         providerARNs: Sequence[str] = ...,
         authType: str = ...,
         authorizerUri: str = ...,
         authorizerCredentials: str = ...,
         identitySource: str = ...,
         identityValidationExpression: str = ...,
-        authorizerResultTtlInSeconds: int = ...
+        authorizerResultTtlInSeconds: int = ...,
     ) -> AuthorizerResponseTypeDef:
         """
         Adds a new Authorizer resource to an existing RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_authorizer)
         """
@@ -238,15 +237,15 @@
         stageName: str = ...,
         stageDescription: str = ...,
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         canarySettings: DeploymentCanarySettingsTypeDef = ...,
-        tracingEnabled: bool = ...
+        tracingEnabled: bool = ...,
     ) -> DeploymentResponseTypeDef:
         """
         Creates a Deployment resource, which makes a specified RestApi callable over
         the
         internet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_deployment)
@@ -265,15 +264,15 @@
 
     async def create_documentation_version(
         self,
         *,
         restApiId: str,
         documentationVersion: str,
         stageName: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> DocumentationVersionResponseTypeDef:
         """
         Creates a documentation version See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/CreateDocumentationVersion).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_documentation_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_documentation_version)
@@ -290,15 +289,15 @@
         certificateArn: str = ...,
         regionalCertificateName: str = ...,
         regionalCertificateArn: str = ...,
         endpointConfiguration: EndpointConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         securityPolicy: SecurityPolicyType = ...,
         mutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
-        ownershipVerificationCertificateArn: str = ...
+        ownershipVerificationCertificateArn: str = ...,
     ) -> DomainNameResponseTypeDef:
         """
         Creates a new domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_domain_name)
         """
@@ -306,30 +305,30 @@
     async def create_model(
         self,
         *,
         restApiId: str,
         name: str,
         contentType: str,
         description: str = ...,
-        schema: str = ...
+        schema: str = ...,
     ) -> ModelResponseTypeDef:
         """
         Adds a new Model resource to an existing RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_model)
         """
 
     async def create_request_validator(
         self,
         *,
         restApiId: str,
         name: str = ...,
         validateRequestBody: bool = ...,
-        validateRequestParameters: bool = ...
+        validateRequestParameters: bool = ...,
     ) -> RequestValidatorResponseTypeDef:
         """
         Creates a RequestValidator of a given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_request_validator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_request_validator)
         """
@@ -353,15 +352,15 @@
         cloneFrom: str = ...,
         binaryMediaTypes: Sequence[str] = ...,
         minimumCompressionSize: int = ...,
         apiKeySource: ApiKeySourceTypeType = ...,
         endpointConfiguration: EndpointConfigurationTypeDef = ...,
         policy: str = ...,
         tags: Mapping[str, str] = ...,
-        disableExecuteApiEndpoint: bool = ...
+        disableExecuteApiEndpoint: bool = ...,
     ) -> RestApiResponseTypeDef:
         """
         Creates a new RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_rest_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_rest_api)
         """
@@ -375,15 +374,15 @@
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         documentationVersion: str = ...,
         canarySettings: CanarySettingsTypeDef = ...,
         tracingEnabled: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StageResponseTypeDef:
         """
         Creates a new Stage resource that references a pre-existing Deployment for the
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_stage)
@@ -393,15 +392,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         apiStages: Sequence[ApiStageTypeDef] = ...,
         throttle: ThrottleSettingsTypeDef = ...,
         quota: QuotaSettingsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> UsagePlanResponseTypeDef:
         """
         Creates a usage plan with the throttle and quota limits, as well as the
         associated API stages, specified in the
         payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_usage_plan)
@@ -420,15 +419,15 @@
 
     async def create_vpc_link(
         self,
         *,
         name: str,
         targetArns: Sequence[str],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> VpcLinkResponseTypeDef:
         """
         Creates a VPC link, under the caller's account in a selected region, in an
         asynchronous operation that typically takes 2-4 minutes to complete and become
         operational.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_vpc_link)
@@ -699,15 +698,15 @@
     async def get_api_keys(
         self,
         *,
         position: str = ...,
         limit: int = ...,
         nameQuery: str = ...,
         customerId: str = ...,
-        includeValues: bool = ...
+        includeValues: bool = ...,
     ) -> ApiKeysTypeDef:
         """
         Gets information about the current ApiKeys resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_api_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_api_keys)
         """
@@ -807,15 +806,15 @@
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         position: str = ...,
         limit: int = ...,
-        locationStatus: LocationStatusTypeType = ...
+        locationStatus: LocationStatusTypeType = ...,
     ) -> DocumentationPartsTypeDef:
         """
         Gets documentation parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_documentation_parts)
         """
@@ -863,15 +862,15 @@
     async def get_export(
         self,
         *,
         restApiId: str,
         stageName: str,
         exportType: str,
         parameters: Mapping[str, str] = ...,
-        accepts: str = ...
+        accepts: str = ...,
     ) -> ExportResponseTypeDef:
         """
         Exports a deployed version of a RestApi in a specified format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_export)
         """
@@ -1079,15 +1078,15 @@
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
         position: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> UsageTypeDef:
         """
         Gets the usage data of a usage plan in a specified time interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_usage)
         """
@@ -1160,15 +1159,15 @@
 
     async def import_documentation_parts(
         self,
         *,
         restApiId: str,
         body: BlobTypeDef,
         mode: PutModeType = ...,
-        failOnWarnings: bool = ...
+        failOnWarnings: bool = ...,
     ) -> DocumentationPartIdsTypeDef:
         """
         Imports documentation parts See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/ImportDocumentationParts).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.import_documentation_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#import_documentation_parts)
@@ -1189,15 +1188,15 @@
     async def put_gateway_response(
         self,
         *,
         restApiId: str,
         responseType: GatewayResponseTypeType,
         statusCode: str = ...,
         responseParameters: Mapping[str, str] = ...,
-        responseTemplates: Mapping[str, str] = ...
+        responseTemplates: Mapping[str, str] = ...,
     ) -> GatewayResponseResponseTypeDef:
         """
         Creates a customization of a GatewayResponse of a specified response type and
         status code on the given
         RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_gateway_response)
@@ -1219,15 +1218,15 @@
         requestParameters: Mapping[str, str] = ...,
         requestTemplates: Mapping[str, str] = ...,
         passthroughBehavior: str = ...,
         cacheNamespace: str = ...,
         cacheKeyParameters: Sequence[str] = ...,
         contentHandling: ContentHandlingStrategyType = ...,
         timeoutInMillis: int = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> IntegrationExtraResponseTypeDef:
         """
         Sets up a method's integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_integration)
         """
@@ -1238,15 +1237,15 @@
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
         selectionPattern: str = ...,
         responseParameters: Mapping[str, str] = ...,
         responseTemplates: Mapping[str, str] = ...,
-        contentHandling: ContentHandlingStrategyType = ...
+        contentHandling: ContentHandlingStrategyType = ...,
     ) -> IntegrationResponseResponseTypeDef:
         """
         Represents a put integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_integration_response)
         """
@@ -1260,15 +1259,15 @@
         authorizationType: str,
         authorizerId: str = ...,
         apiKeyRequired: bool = ...,
         operationName: str = ...,
         requestParameters: Mapping[str, bool] = ...,
         requestModels: Mapping[str, str] = ...,
         requestValidatorId: str = ...,
-        authorizationScopes: Sequence[str] = ...
+        authorizationScopes: Sequence[str] = ...,
     ) -> MethodExtraResponseTypeDef:
         """
         Add a method to an existing Resource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_method)
         """
@@ -1277,15 +1276,15 @@
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
         responseParameters: Mapping[str, bool] = ...,
-        responseModels: Mapping[str, str] = ...
+        responseModels: Mapping[str, str] = ...,
     ) -> MethodResponseResponseTypeDef:
         """
         Adds a MethodResponse to an existing Method resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_method_response)
         """
@@ -1293,15 +1292,15 @@
     async def put_rest_api(
         self,
         *,
         restApiId: str,
         body: BlobTypeDef,
         mode: PutModeType = ...,
         failOnWarnings: bool = ...,
-        parameters: Mapping[str, str] = ...
+        parameters: Mapping[str, str] = ...,
     ) -> RestApiResponseTypeDef:
         """
         A feature of the API Gateway control service for updating an existing API with
         an input of external API
         definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_rest_api)
@@ -1324,15 +1323,15 @@
         restApiId: str,
         authorizerId: str,
         headers: Mapping[str, str] = ...,
         multiValueHeaders: Mapping[str, Sequence[str]] = ...,
         pathWithQueryString: str = ...,
         body: str = ...,
         stageVariables: Mapping[str, str] = ...,
-        additionalContext: Mapping[str, str] = ...
+        additionalContext: Mapping[str, str] = ...,
     ) -> TestInvokeAuthorizerResponseTypeDef:
         """
         Simulate the execution of an Authorizer in your RestApi with headers,
         parameters, and an incoming request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_authorizer)
@@ -1346,15 +1345,15 @@
         resourceId: str,
         httpMethod: str,
         pathWithQueryString: str = ...,
         body: str = ...,
         headers: Mapping[str, str] = ...,
         multiValueHeaders: Mapping[str, Sequence[str]] = ...,
         clientCertificateId: str = ...,
-        stageVariables: Mapping[str, str] = ...
+        stageVariables: Mapping[str, str] = ...,
     ) -> TestInvokeMethodResponseTypeDef:
         """
         Simulate the invocation of a Method in your RestApi with headers, parameters,
         and an incoming request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_method)
@@ -1392,29 +1391,29 @@
         """
 
     async def update_authorizer(
         self,
         *,
         restApiId: str,
         authorizerId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> AuthorizerResponseTypeDef:
         """
         Updates an existing Authorizer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_authorizer)
         """
 
     async def update_base_path_mapping(
         self,
         *,
         domainName: str,
         basePath: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> BasePathMappingResponseTypeDef:
         """
         Changes information about the BasePathMapping resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_base_path_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_base_path_mapping)
         """
@@ -1430,43 +1429,43 @@
         """
 
     async def update_deployment(
         self,
         *,
         restApiId: str,
         deploymentId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DeploymentResponseTypeDef:
         """
         Changes information about a Deployment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_deployment)
         """
 
     async def update_documentation_part(
         self,
         *,
         restApiId: str,
         documentationPartId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DocumentationPartResponseTypeDef:
         """
         Updates a documentation part.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_documentation_part)
         """
 
     async def update_documentation_version(
         self,
         *,
         restApiId: str,
         documentationVersion: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DocumentationVersionResponseTypeDef:
         """
         Updates a documentation version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_documentation_version)
         """
@@ -1482,30 +1481,30 @@
         """
 
     async def update_gateway_response(
         self,
         *,
         restApiId: str,
         responseType: GatewayResponseTypeType,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> GatewayResponseResponseTypeDef:
         """
         Updates a GatewayResponse of a specified response type on the given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_gateway_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_gateway_response)
         """
 
     async def update_integration(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> IntegrationExtraResponseTypeDef:
         """
         Represents an update integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_integration)
         """
@@ -1513,30 +1512,30 @@
     async def update_integration_response(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> IntegrationResponseResponseTypeDef:
         """
         Represents an update integration response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_integration_response)
         """
 
     async def update_method(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> MethodExtraResponseTypeDef:
         """
         Updates an existing Method resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_method)
         """
@@ -1544,57 +1543,57 @@
     async def update_method_response(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> MethodResponseResponseTypeDef:
         """
         Updates an existing MethodResponse resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_method_response)
         """
 
     async def update_model(
         self,
         *,
         restApiId: str,
         modelName: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> ModelResponseTypeDef:
         """
         Changes information about a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_model)
         """
 
     async def update_request_validator(
         self,
         *,
         restApiId: str,
         requestValidatorId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> RequestValidatorResponseTypeDef:
         """
         Updates a RequestValidator of a given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_request_validator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_request_validator)
         """
 
     async def update_resource(
         self,
         *,
         restApiId: str,
         resourceId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> ResourceResponseTypeDef:
         """
         Changes information about a Resource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_resource)
         """
@@ -1610,29 +1609,29 @@
         """
 
     async def update_stage(
         self,
         *,
         restApiId: str,
         stageName: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> StageResponseTypeDef:
         """
         Changes information about a Stage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_stage)
         """
 
     async def update_usage(
         self,
         *,
         usagePlanId: str,
         keyId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> UsageTypeDef:
         """
         Grants a temporary extension to the remaining quota of a usage plan associated
         with a specified API
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_usage)
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/client.pyi` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         name: str = ...,
         description: str = ...,
         enabled: bool = ...,
         generateDistinctId: bool = ...,
         value: str = ...,
         stageKeys: Sequence[StageKeyTypeDef] = ...,
         customerId: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> ApiKeyResponseTypeDef:
         """
         Create an ApiKey resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_api_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_api_key)
         """
@@ -204,15 +204,15 @@
         type: AuthorizerTypeType,
         providerARNs: Sequence[str] = ...,
         authType: str = ...,
         authorizerUri: str = ...,
         authorizerCredentials: str = ...,
         identitySource: str = ...,
         identityValidationExpression: str = ...,
-        authorizerResultTtlInSeconds: int = ...
+        authorizerResultTtlInSeconds: int = ...,
     ) -> AuthorizerResponseTypeDef:
         """
         Adds a new Authorizer resource to an existing RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_authorizer)
         """
@@ -234,15 +234,15 @@
         stageName: str = ...,
         stageDescription: str = ...,
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         canarySettings: DeploymentCanarySettingsTypeDef = ...,
-        tracingEnabled: bool = ...
+        tracingEnabled: bool = ...,
     ) -> DeploymentResponseTypeDef:
         """
         Creates a Deployment resource, which makes a specified RestApi callable over
         the
         internet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_deployment)
@@ -261,15 +261,15 @@
 
     async def create_documentation_version(
         self,
         *,
         restApiId: str,
         documentationVersion: str,
         stageName: str = ...,
-        description: str = ...
+        description: str = ...,
     ) -> DocumentationVersionResponseTypeDef:
         """
         Creates a documentation version See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/CreateDocumentationVersion).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_documentation_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_documentation_version)
@@ -286,15 +286,15 @@
         certificateArn: str = ...,
         regionalCertificateName: str = ...,
         regionalCertificateArn: str = ...,
         endpointConfiguration: EndpointConfigurationTypeDef = ...,
         tags: Mapping[str, str] = ...,
         securityPolicy: SecurityPolicyType = ...,
         mutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
-        ownershipVerificationCertificateArn: str = ...
+        ownershipVerificationCertificateArn: str = ...,
     ) -> DomainNameResponseTypeDef:
         """
         Creates a new domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_domain_name)
         """
@@ -302,30 +302,30 @@
     async def create_model(
         self,
         *,
         restApiId: str,
         name: str,
         contentType: str,
         description: str = ...,
-        schema: str = ...
+        schema: str = ...,
     ) -> ModelResponseTypeDef:
         """
         Adds a new Model resource to an existing RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_model)
         """
 
     async def create_request_validator(
         self,
         *,
         restApiId: str,
         name: str = ...,
         validateRequestBody: bool = ...,
-        validateRequestParameters: bool = ...
+        validateRequestParameters: bool = ...,
     ) -> RequestValidatorResponseTypeDef:
         """
         Creates a RequestValidator of a given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_request_validator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_request_validator)
         """
@@ -349,15 +349,15 @@
         cloneFrom: str = ...,
         binaryMediaTypes: Sequence[str] = ...,
         minimumCompressionSize: int = ...,
         apiKeySource: ApiKeySourceTypeType = ...,
         endpointConfiguration: EndpointConfigurationTypeDef = ...,
         policy: str = ...,
         tags: Mapping[str, str] = ...,
-        disableExecuteApiEndpoint: bool = ...
+        disableExecuteApiEndpoint: bool = ...,
     ) -> RestApiResponseTypeDef:
         """
         Creates a new RestApi resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_rest_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_rest_api)
         """
@@ -371,15 +371,15 @@
         description: str = ...,
         cacheClusterEnabled: bool = ...,
         cacheClusterSize: CacheClusterSizeType = ...,
         variables: Mapping[str, str] = ...,
         documentationVersion: str = ...,
         canarySettings: CanarySettingsTypeDef = ...,
         tracingEnabled: bool = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> StageResponseTypeDef:
         """
         Creates a new Stage resource that references a pre-existing Deployment for the
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#create_stage)
@@ -389,15 +389,15 @@
         self,
         *,
         name: str,
         description: str = ...,
         apiStages: Sequence[ApiStageTypeDef] = ...,
         throttle: ThrottleSettingsTypeDef = ...,
         quota: QuotaSettingsTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> UsagePlanResponseTypeDef:
         """
         Creates a usage plan with the throttle and quota limits, as well as the
         associated API stages, specified in the
         payload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_usage_plan)
@@ -416,15 +416,15 @@
 
     async def create_vpc_link(
         self,
         *,
         name: str,
         targetArns: Sequence[str],
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> VpcLinkResponseTypeDef:
         """
         Creates a VPC link, under the caller's account in a selected region, in an
         asynchronous operation that typically takes 2-4 minutes to complete and become
         operational.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.create_vpc_link)
@@ -695,15 +695,15 @@
     async def get_api_keys(
         self,
         *,
         position: str = ...,
         limit: int = ...,
         nameQuery: str = ...,
         customerId: str = ...,
-        includeValues: bool = ...
+        includeValues: bool = ...,
     ) -> ApiKeysTypeDef:
         """
         Gets information about the current ApiKeys resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_api_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_api_keys)
         """
@@ -803,15 +803,15 @@
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         position: str = ...,
         limit: int = ...,
-        locationStatus: LocationStatusTypeType = ...
+        locationStatus: LocationStatusTypeType = ...,
     ) -> DocumentationPartsTypeDef:
         """
         Gets documentation parts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_documentation_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_documentation_parts)
         """
@@ -859,15 +859,15 @@
     async def get_export(
         self,
         *,
         restApiId: str,
         stageName: str,
         exportType: str,
         parameters: Mapping[str, str] = ...,
-        accepts: str = ...
+        accepts: str = ...,
     ) -> ExportResponseTypeDef:
         """
         Exports a deployed version of a RestApi in a specified format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_export)
         """
@@ -1075,15 +1075,15 @@
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
         position: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> UsageTypeDef:
         """
         Gets the usage data of a usage plan in a specified time interval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.get_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#get_usage)
         """
@@ -1156,15 +1156,15 @@
 
     async def import_documentation_parts(
         self,
         *,
         restApiId: str,
         body: BlobTypeDef,
         mode: PutModeType = ...,
-        failOnWarnings: bool = ...
+        failOnWarnings: bool = ...,
     ) -> DocumentationPartIdsTypeDef:
         """
         Imports documentation parts See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigateway-2015-07-09/ImportDocumentationParts).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.import_documentation_parts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#import_documentation_parts)
@@ -1185,15 +1185,15 @@
     async def put_gateway_response(
         self,
         *,
         restApiId: str,
         responseType: GatewayResponseTypeType,
         statusCode: str = ...,
         responseParameters: Mapping[str, str] = ...,
-        responseTemplates: Mapping[str, str] = ...
+        responseTemplates: Mapping[str, str] = ...,
     ) -> GatewayResponseResponseTypeDef:
         """
         Creates a customization of a GatewayResponse of a specified response type and
         status code on the given
         RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_gateway_response)
@@ -1215,15 +1215,15 @@
         requestParameters: Mapping[str, str] = ...,
         requestTemplates: Mapping[str, str] = ...,
         passthroughBehavior: str = ...,
         cacheNamespace: str = ...,
         cacheKeyParameters: Sequence[str] = ...,
         contentHandling: ContentHandlingStrategyType = ...,
         timeoutInMillis: int = ...,
-        tlsConfig: TlsConfigTypeDef = ...
+        tlsConfig: TlsConfigTypeDef = ...,
     ) -> IntegrationExtraResponseTypeDef:
         """
         Sets up a method's integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_integration)
         """
@@ -1234,15 +1234,15 @@
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
         selectionPattern: str = ...,
         responseParameters: Mapping[str, str] = ...,
         responseTemplates: Mapping[str, str] = ...,
-        contentHandling: ContentHandlingStrategyType = ...
+        contentHandling: ContentHandlingStrategyType = ...,
     ) -> IntegrationResponseResponseTypeDef:
         """
         Represents a put integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_integration_response)
         """
@@ -1256,15 +1256,15 @@
         authorizationType: str,
         authorizerId: str = ...,
         apiKeyRequired: bool = ...,
         operationName: str = ...,
         requestParameters: Mapping[str, bool] = ...,
         requestModels: Mapping[str, str] = ...,
         requestValidatorId: str = ...,
-        authorizationScopes: Sequence[str] = ...
+        authorizationScopes: Sequence[str] = ...,
     ) -> MethodExtraResponseTypeDef:
         """
         Add a method to an existing Resource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_method)
         """
@@ -1273,15 +1273,15 @@
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
         responseParameters: Mapping[str, bool] = ...,
-        responseModels: Mapping[str, str] = ...
+        responseModels: Mapping[str, str] = ...,
     ) -> MethodResponseResponseTypeDef:
         """
         Adds a MethodResponse to an existing Method resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_method_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#put_method_response)
         """
@@ -1289,15 +1289,15 @@
     async def put_rest_api(
         self,
         *,
         restApiId: str,
         body: BlobTypeDef,
         mode: PutModeType = ...,
         failOnWarnings: bool = ...,
-        parameters: Mapping[str, str] = ...
+        parameters: Mapping[str, str] = ...,
     ) -> RestApiResponseTypeDef:
         """
         A feature of the API Gateway control service for updating an existing API with
         an input of external API
         definitions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.put_rest_api)
@@ -1320,15 +1320,15 @@
         restApiId: str,
         authorizerId: str,
         headers: Mapping[str, str] = ...,
         multiValueHeaders: Mapping[str, Sequence[str]] = ...,
         pathWithQueryString: str = ...,
         body: str = ...,
         stageVariables: Mapping[str, str] = ...,
-        additionalContext: Mapping[str, str] = ...
+        additionalContext: Mapping[str, str] = ...,
     ) -> TestInvokeAuthorizerResponseTypeDef:
         """
         Simulate the execution of an Authorizer in your RestApi with headers,
         parameters, and an incoming request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_authorizer)
@@ -1342,15 +1342,15 @@
         resourceId: str,
         httpMethod: str,
         pathWithQueryString: str = ...,
         body: str = ...,
         headers: Mapping[str, str] = ...,
         multiValueHeaders: Mapping[str, Sequence[str]] = ...,
         clientCertificateId: str = ...,
-        stageVariables: Mapping[str, str] = ...
+        stageVariables: Mapping[str, str] = ...,
     ) -> TestInvokeMethodResponseTypeDef:
         """
         Simulate the invocation of a Method in your RestApi with headers, parameters,
         and an incoming request
         body.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.test_invoke_method)
@@ -1388,29 +1388,29 @@
         """
 
     async def update_authorizer(
         self,
         *,
         restApiId: str,
         authorizerId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> AuthorizerResponseTypeDef:
         """
         Updates an existing Authorizer resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_authorizer)
         """
 
     async def update_base_path_mapping(
         self,
         *,
         domainName: str,
         basePath: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> BasePathMappingResponseTypeDef:
         """
         Changes information about the BasePathMapping resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_base_path_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_base_path_mapping)
         """
@@ -1426,43 +1426,43 @@
         """
 
     async def update_deployment(
         self,
         *,
         restApiId: str,
         deploymentId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DeploymentResponseTypeDef:
         """
         Changes information about a Deployment resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_deployment)
         """
 
     async def update_documentation_part(
         self,
         *,
         restApiId: str,
         documentationPartId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DocumentationPartResponseTypeDef:
         """
         Updates a documentation part.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_documentation_part)
         """
 
     async def update_documentation_version(
         self,
         *,
         restApiId: str,
         documentationVersion: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> DocumentationVersionResponseTypeDef:
         """
         Updates a documentation version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_documentation_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_documentation_version)
         """
@@ -1478,30 +1478,30 @@
         """
 
     async def update_gateway_response(
         self,
         *,
         restApiId: str,
         responseType: GatewayResponseTypeType,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> GatewayResponseResponseTypeDef:
         """
         Updates a GatewayResponse of a specified response type on the given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_gateway_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_gateway_response)
         """
 
     async def update_integration(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> IntegrationExtraResponseTypeDef:
         """
         Represents an update integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_integration)
         """
@@ -1509,30 +1509,30 @@
     async def update_integration_response(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> IntegrationResponseResponseTypeDef:
         """
         Represents an update integration response.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_integration_response)
         """
 
     async def update_method(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> MethodExtraResponseTypeDef:
         """
         Updates an existing Method resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_method)
         """
@@ -1540,57 +1540,57 @@
     async def update_method_response(
         self,
         *,
         restApiId: str,
         resourceId: str,
         httpMethod: str,
         statusCode: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> MethodResponseResponseTypeDef:
         """
         Updates an existing MethodResponse resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_method_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_method_response)
         """
 
     async def update_model(
         self,
         *,
         restApiId: str,
         modelName: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> ModelResponseTypeDef:
         """
         Changes information about a model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_model)
         """
 
     async def update_request_validator(
         self,
         *,
         restApiId: str,
         requestValidatorId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> RequestValidatorResponseTypeDef:
         """
         Updates a RequestValidator of a given RestApi.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_request_validator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_request_validator)
         """
 
     async def update_resource(
         self,
         *,
         restApiId: str,
         resourceId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> ResourceResponseTypeDef:
         """
         Changes information about a Resource resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_resource)
         """
@@ -1606,29 +1606,29 @@
         """
 
     async def update_stage(
         self,
         *,
         restApiId: str,
         stageName: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> StageResponseTypeDef:
         """
         Changes information about a Stage resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/client/#update_stage)
         """
 
     async def update_usage(
         self,
         *,
         usagePlanId: str,
         keyId: str,
-        patchOperations: Sequence[PatchOperationTypeDef] = ...
+        patchOperations: Sequence[PatchOperationTypeDef] = ...,
     ) -> UsageTypeDef:
         """
         Grants a temporary extension to the remaining quota of a usage plan associated
         with a specified API
         key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Client.update_usage)
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/literals.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/literals.py`

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
     "ApiKeySourceTypeType",
     "ApiKeysFormatType",
     "AuthorizerTypeType",
     "CacheClusterSizeType",
     "CacheClusterStatusType",
     "ConnectionTypeType",
@@ -61,15 +60,14 @@
     "APIGatewayServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApiKeySourceTypeType = Literal["AUTHORIZER", "HEADER"]
 ApiKeysFormatType = Literal["csv"]
 AuthorizerTypeType = Literal["COGNITO_USER_POOLS", "REQUEST", "TOKEN"]
 CacheClusterSizeType = Literal["0.5", "1.6", "118", "13.5", "237", "28.4", "58.2", "6.1"]
 CacheClusterStatusType = Literal[
     "AVAILABLE", "CREATE_IN_PROGRESS", "DELETE_IN_PROGRESS", "FLUSH_IN_PROGRESS", "NOT_AVAILABLE"
 ]
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/literals.pyi` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/paginator.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,14 @@
     "GetSdkTypesPaginator",
     "GetUsagePaginator",
     "GetUsagePlanKeysPaginator",
     "GetUsagePlansPaginator",
     "GetVpcLinksPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -123,15 +122,15 @@
 
     def paginate(
         self,
         *,
         nameQuery: str = ...,
         customerId: str = ...,
         includeValues: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ApiKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getapikeyspaginator)
         """
 
 
@@ -205,15 +204,15 @@
         self,
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         locationStatus: LocationStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DocumentationPartsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getdocumentationpartspaginator)
         """
 
 
@@ -299,15 +298,15 @@
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         embed: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ResourcesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getresourcespaginator)
         """
 
 
@@ -350,15 +349,15 @@
     def paginate(
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getusagepaginator)
         """
 
 
@@ -369,15 +368,15 @@
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         nameQuery: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsagePlanKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getusageplankeyspaginator)
         """
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/paginator.pyi` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     def paginate(
         self,
         *,
         nameQuery: str = ...,
         customerId: str = ...,
         includeValues: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ApiKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetApiKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getapikeyspaginator)
         """
 
 class GetAuthorizersPaginator(AioPaginator):
@@ -197,15 +197,15 @@
         self,
         *,
         restApiId: str,
         type: DocumentationPartTypeType = ...,
         nameQuery: str = ...,
         path: str = ...,
         locationStatus: LocationStatusTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DocumentationPartsTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetDocumentationParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getdocumentationpartspaginator)
         """
 
 class GetDocumentationVersionsPaginator(AioPaginator):
@@ -285,15 +285,15 @@
     """
 
     def paginate(
         self,
         *,
         restApiId: str,
         embed: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ResourcesTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getresourcespaginator)
         """
 
 class GetRestApisPaginator(AioPaginator):
@@ -333,15 +333,15 @@
     def paginate(
         self,
         *,
         usagePlanId: str,
         startDate: str,
         endDate: str,
         keyId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsageTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getusagepaginator)
         """
 
 class GetUsagePlanKeysPaginator(AioPaginator):
@@ -351,15 +351,15 @@
     """
 
     def paginate(
         self,
         *,
         usagePlanId: str,
         nameQuery: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[UsagePlanKeysTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway.Paginator.GetUsagePlanKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/paginators/#getusageplankeyspaginator)
         """
 
 class GetUsagePlansPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/type_defs.py` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogSettingsTypeDef",
     "ResponseMetadataTypeDef",
     "ThrottleSettingsTypeDef",
     "ApiKeyTypeDef",
     "AuthorizerTypeDef",
     "BasePathMappingTypeDef",
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway/type_defs.pyi` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/PKG-INFO` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigateway
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.APIGateway 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.APIGateway 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/
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
 
 <a id="types-aiobotocore-apigateway"></a>
 
 # types-aiobotocore-apigateway
 
 [![PyPI - types-aiobotocore-apigateway](https://img.shields.io/pypi/v/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigateway.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigateway)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigateway)](https://pepy.tech/project/types-aiobotocore-apigateway)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.APIGateway 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
+[aiobotocore.APIGateway 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#APIGateway)
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
 [types-aiobotocore-apigateway docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigateway/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigateway-2.9.0/types_aiobotocore_apigateway.egg-info/SOURCES.txt` & `types-aiobotocore-apigateway-2.9.1/types_aiobotocore_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

