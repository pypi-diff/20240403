# Comparing `tmp/types-aiobotocore-apigatewayv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-apigatewayv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewayv2-2.9.0.tar", last modified: Wed Dec 13 19:58:32 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewayv2-2.9.1.tar", last modified: Thu Jan 18 01:20:01 2024, max compression
```

## Comparing `types-aiobotocore-apigatewayv2-2.9.0.tar` & `types-aiobotocore-apigatewayv2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:32.750111 types-aiobotocore-apigatewayv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2023-12-13 19:58:32.750111 types-aiobotocore-apigatewayv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12805 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:32.750111 types-aiobotocore-apigatewayv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:32.746111 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54788 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54784 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11266 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11926 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    66272 2023-12-13 19:40:57.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    66271 2023-12-13 19:40:55.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:40:54.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:32.750111 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14388 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:32.000000 types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.009524 types-aiobotocore-apigatewayv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-01-18 01:20:01.009524 types-aiobotocore-apigatewayv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12805 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:01.009524 types-aiobotocore-apigatewayv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.005524 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54807 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54804 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11266 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11926 2024-01-18 01:02:54.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    66271 2024-01-18 01:02:56.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66271 2024-01-18 01:02:55.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:02:53.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:01.005524 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:00.000000 types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/LICENSE` & `types-aiobotocore-apigatewayv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
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
 
 <a id="types-aiobotocore-apigatewayv2"></a>
 
 # types-aiobotocore-apigatewayv2
 
 [![PyPI - types-aiobotocore-apigatewayv2](https://img.shields.io/pypi/v/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/README.md` & `types-aiobotocore-apigatewayv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/setup.py` & `types-aiobotocore-apigatewayv2-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewayv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ApiGatewayV2 2.9.1 service generated with"
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
     keywords="aiobotocore apigatewayv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_apigatewayv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__init__.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 
 Client = ApiGatewayV2Client
 
-
 __all__ = (
     "ApiGatewayV2Client",
     "Client",
     "GetApisPaginator",
     "GetAuthorizersPaginator",
     "GetDeploymentsPaginator",
     "GetDomainNamesPaginator",
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__init__.pyi` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/__main__.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ApiGatewayV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/client.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ApiGatewayV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -178,15 +177,15 @@
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
         Target: str = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> CreateApiResponseTypeDef:
         """
         Creates an Api resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_api)
         """
@@ -210,15 +209,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: JWTConfigurationTypeDef = ...,
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -235,15 +234,15 @@
 
     async def create_domain_name(
         self,
         *,
         DomainName: str,
         DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_domain_name)
         """
@@ -264,15 +263,15 @@
         PassthroughBehavior: PassthroughBehaviorType = ...,
         PayloadFormatVersion: str = ...,
         RequestParameters: Mapping[str, str] = ...,
         RequestTemplates: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
         TemplateSelectionExpression: str = ...,
         TimeoutInMillis: int = ...,
-        TlsConfig: TlsConfigInputTypeDef = ...
+        TlsConfig: TlsConfigInputTypeDef = ...,
     ) -> CreateIntegrationResultTypeDef:
         """
         Creates an Integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_integration)
         """
@@ -282,15 +281,15 @@
         *,
         ApiId: str,
         IntegrationId: str,
         IntegrationResponseKey: str,
         ContentHandlingStrategy: ContentHandlingStrategyType = ...,
         ResponseParameters: Mapping[str, str] = ...,
         ResponseTemplates: Mapping[str, str] = ...,
-        TemplateSelectionExpression: str = ...
+        TemplateSelectionExpression: str = ...,
     ) -> CreateIntegrationResponseResponseTypeDef:
         """
         Creates an IntegrationResponses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_integration_response)
         """
@@ -315,15 +314,15 @@
         AuthorizationType: AuthorizationTypeType = ...,
         AuthorizerId: str = ...,
         ModelSelectionExpression: str = ...,
         OperationName: str = ...,
         RequestModels: Mapping[str, str] = ...,
         RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
         RouteResponseSelectionExpression: str = ...,
-        Target: str = ...
+        Target: str = ...,
     ) -> CreateRouteResultTypeDef:
         """
         Creates a Route for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_route)
         """
@@ -332,15 +331,15 @@
         self,
         *,
         ApiId: str,
         RouteId: str,
         RouteResponseKey: str,
         ModelSelectionExpression: str = ...,
         ResponseModels: Mapping[str, str] = ...,
-        ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...
+        ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
     ) -> CreateRouteResponseResponseTypeDef:
         """
         Creates a RouteResponse for a Route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_route_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_route_response)
         """
@@ -354,30 +353,30 @@
         AutoDeploy: bool = ...,
         ClientCertificateId: str = ...,
         DefaultRouteSettings: RouteSettingsTypeDef = ...,
         DeploymentId: str = ...,
         Description: str = ...,
         RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,
         StageVariables: Mapping[str, str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a Stage for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_stage)
         """
 
     async def create_vpc_link(
         self,
         *,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVpcLinkResponseTypeDef:
         """
         Creates a VPC link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_vpc_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_vpc_link)
         """
@@ -532,15 +531,15 @@
         self,
         *,
         ApiId: str,
         OutputType: JSONYAMLType,
         Specification: Literal["OAS30"],
         ExportVersion: str = ...,
         IncludeExtensions: bool = ...,
-        StageName: str = ...
+        StageName: str = ...,
     ) -> ExportApiResponseTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigatewayv2-2018-11-29/ExportApi).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.export_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#export_api)
@@ -866,15 +865,15 @@
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Target: str = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateApiResponseTypeDef:
         """
         Updates an Api resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_api)
         """
@@ -882,15 +881,15 @@
     async def update_api_mapping(
         self,
         *,
         ApiId: str,
         ApiMappingId: str,
         DomainName: str,
         ApiMappingKey: str = ...,
-        Stage: str = ...
+        Stage: str = ...,
     ) -> UpdateApiMappingResponseTypeDef:
         """
         The API mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_api_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_api_mapping)
         """
@@ -905,15 +904,15 @@
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
         JwtConfiguration: JWTConfigurationTypeDef = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
         """
@@ -929,15 +928,15 @@
         """
 
     async def update_domain_name(
         self,
         *,
         DomainName: str,
         DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
-        MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
+        MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
         """
@@ -959,15 +958,15 @@
         PassthroughBehavior: PassthroughBehaviorType = ...,
         PayloadFormatVersion: str = ...,
         RequestParameters: Mapping[str, str] = ...,
         RequestTemplates: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
         TemplateSelectionExpression: str = ...,
         TimeoutInMillis: int = ...,
-        TlsConfig: TlsConfigInputTypeDef = ...
+        TlsConfig: TlsConfigInputTypeDef = ...,
     ) -> UpdateIntegrationResultTypeDef:
         """
         Updates an Integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_integration)
         """
@@ -978,15 +977,15 @@
         ApiId: str,
         IntegrationId: str,
         IntegrationResponseId: str,
         ContentHandlingStrategy: ContentHandlingStrategyType = ...,
         IntegrationResponseKey: str = ...,
         ResponseParameters: Mapping[str, str] = ...,
         ResponseTemplates: Mapping[str, str] = ...,
-        TemplateSelectionExpression: str = ...
+        TemplateSelectionExpression: str = ...,
     ) -> UpdateIntegrationResponseResponseTypeDef:
         """
         Updates an IntegrationResponses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_integration_response)
         """
@@ -995,15 +994,15 @@
         self,
         *,
         ApiId: str,
         ModelId: str,
         ContentType: str = ...,
         Description: str = ...,
         Name: str = ...,
-        Schema: str = ...
+        Schema: str = ...,
     ) -> UpdateModelResponseTypeDef:
         """
         Updates a Model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_model)
         """
@@ -1019,15 +1018,15 @@
         AuthorizerId: str = ...,
         ModelSelectionExpression: str = ...,
         OperationName: str = ...,
         RequestModels: Mapping[str, str] = ...,
         RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
         RouteKey: str = ...,
         RouteResponseSelectionExpression: str = ...,
-        Target: str = ...
+        Target: str = ...,
     ) -> UpdateRouteResultTypeDef:
         """
         Updates a Route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_route)
         """
@@ -1037,15 +1036,15 @@
         *,
         ApiId: str,
         RouteId: str,
         RouteResponseId: str,
         ModelSelectionExpression: str = ...,
         ResponseModels: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
-        RouteResponseKey: str = ...
+        RouteResponseKey: str = ...,
     ) -> UpdateRouteResponseResponseTypeDef:
         """
         Updates a RouteResponse.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_route_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_route_response)
         """
@@ -1058,15 +1057,15 @@
         AccessLogSettings: AccessLogSettingsTypeDef = ...,
         AutoDeploy: bool = ...,
         ClientCertificateId: str = ...,
         DefaultRouteSettings: RouteSettingsTypeDef = ...,
         DeploymentId: str = ...,
         Description: str = ...,
         RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,
-        StageVariables: Mapping[str, str] = ...
+        StageVariables: Mapping[str, str] = ...,
     ) -> UpdateStageResponseTypeDef:
         """
         Updates a Stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_stage)
         """
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/client.pyi` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
         Target: str = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> CreateApiResponseTypeDef:
         """
         Creates an Api resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_api)
         """
@@ -206,15 +206,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: JWTConfigurationTypeDef = ...,
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -231,15 +231,15 @@
 
     async def create_domain_name(
         self,
         *,
         DomainName: str,
         DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_domain_name)
         """
@@ -260,15 +260,15 @@
         PassthroughBehavior: PassthroughBehaviorType = ...,
         PayloadFormatVersion: str = ...,
         RequestParameters: Mapping[str, str] = ...,
         RequestTemplates: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
         TemplateSelectionExpression: str = ...,
         TimeoutInMillis: int = ...,
-        TlsConfig: TlsConfigInputTypeDef = ...
+        TlsConfig: TlsConfigInputTypeDef = ...,
     ) -> CreateIntegrationResultTypeDef:
         """
         Creates an Integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_integration)
         """
@@ -278,15 +278,15 @@
         *,
         ApiId: str,
         IntegrationId: str,
         IntegrationResponseKey: str,
         ContentHandlingStrategy: ContentHandlingStrategyType = ...,
         ResponseParameters: Mapping[str, str] = ...,
         ResponseTemplates: Mapping[str, str] = ...,
-        TemplateSelectionExpression: str = ...
+        TemplateSelectionExpression: str = ...,
     ) -> CreateIntegrationResponseResponseTypeDef:
         """
         Creates an IntegrationResponses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_integration_response)
         """
@@ -311,15 +311,15 @@
         AuthorizationType: AuthorizationTypeType = ...,
         AuthorizerId: str = ...,
         ModelSelectionExpression: str = ...,
         OperationName: str = ...,
         RequestModels: Mapping[str, str] = ...,
         RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
         RouteResponseSelectionExpression: str = ...,
-        Target: str = ...
+        Target: str = ...,
     ) -> CreateRouteResultTypeDef:
         """
         Creates a Route for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_route)
         """
@@ -328,15 +328,15 @@
         self,
         *,
         ApiId: str,
         RouteId: str,
         RouteResponseKey: str,
         ModelSelectionExpression: str = ...,
         ResponseModels: Mapping[str, str] = ...,
-        ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...
+        ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
     ) -> CreateRouteResponseResponseTypeDef:
         """
         Creates a RouteResponse for a Route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_route_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_route_response)
         """
@@ -350,30 +350,30 @@
         AutoDeploy: bool = ...,
         ClientCertificateId: str = ...,
         DefaultRouteSettings: RouteSettingsTypeDef = ...,
         DeploymentId: str = ...,
         Description: str = ...,
         RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,
         StageVariables: Mapping[str, str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateStageResponseTypeDef:
         """
         Creates a Stage for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_stage)
         """
 
     async def create_vpc_link(
         self,
         *,
         Name: str,
         SubnetIds: Sequence[str],
         SecurityGroupIds: Sequence[str] = ...,
-        Tags: Mapping[str, str] = ...
+        Tags: Mapping[str, str] = ...,
     ) -> CreateVpcLinkResponseTypeDef:
         """
         Creates a VPC link.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_vpc_link)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_vpc_link)
         """
@@ -528,15 +528,15 @@
         self,
         *,
         ApiId: str,
         OutputType: JSONYAMLType,
         Specification: Literal["OAS30"],
         ExportVersion: str = ...,
         IncludeExtensions: bool = ...,
-        StageName: str = ...
+        StageName: str = ...,
     ) -> ExportApiResponseTypeDef:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/apigatewayv2-2018-11-29/ExportApi).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.export_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#export_api)
@@ -862,15 +862,15 @@
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Target: str = ...,
-        Version: str = ...
+        Version: str = ...,
     ) -> UpdateApiResponseTypeDef:
         """
         Updates an Api resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_api)
         """
@@ -878,15 +878,15 @@
     async def update_api_mapping(
         self,
         *,
         ApiId: str,
         ApiMappingId: str,
         DomainName: str,
         ApiMappingKey: str = ...,
-        Stage: str = ...
+        Stage: str = ...,
     ) -> UpdateApiMappingResponseTypeDef:
         """
         The API mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_api_mapping)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_api_mapping)
         """
@@ -901,15 +901,15 @@
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
         JwtConfiguration: JWTConfigurationTypeDef = ...,
-        Name: str = ...
+        Name: str = ...,
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
         """
@@ -925,15 +925,15 @@
         """
 
     async def update_domain_name(
         self,
         *,
         DomainName: str,
         DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
-        MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
+        MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
         """
@@ -955,15 +955,15 @@
         PassthroughBehavior: PassthroughBehaviorType = ...,
         PayloadFormatVersion: str = ...,
         RequestParameters: Mapping[str, str] = ...,
         RequestTemplates: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, Mapping[str, str]] = ...,
         TemplateSelectionExpression: str = ...,
         TimeoutInMillis: int = ...,
-        TlsConfig: TlsConfigInputTypeDef = ...
+        TlsConfig: TlsConfigInputTypeDef = ...,
     ) -> UpdateIntegrationResultTypeDef:
         """
         Updates an Integration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_integration)
         """
@@ -974,15 +974,15 @@
         ApiId: str,
         IntegrationId: str,
         IntegrationResponseId: str,
         ContentHandlingStrategy: ContentHandlingStrategyType = ...,
         IntegrationResponseKey: str = ...,
         ResponseParameters: Mapping[str, str] = ...,
         ResponseTemplates: Mapping[str, str] = ...,
-        TemplateSelectionExpression: str = ...
+        TemplateSelectionExpression: str = ...,
     ) -> UpdateIntegrationResponseResponseTypeDef:
         """
         Updates an IntegrationResponses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_integration_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_integration_response)
         """
@@ -991,15 +991,15 @@
         self,
         *,
         ApiId: str,
         ModelId: str,
         ContentType: str = ...,
         Description: str = ...,
         Name: str = ...,
-        Schema: str = ...
+        Schema: str = ...,
     ) -> UpdateModelResponseTypeDef:
         """
         Updates a Model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_model)
         """
@@ -1015,15 +1015,15 @@
         AuthorizerId: str = ...,
         ModelSelectionExpression: str = ...,
         OperationName: str = ...,
         RequestModels: Mapping[str, str] = ...,
         RequestParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
         RouteKey: str = ...,
         RouteResponseSelectionExpression: str = ...,
-        Target: str = ...
+        Target: str = ...,
     ) -> UpdateRouteResultTypeDef:
         """
         Updates a Route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_route)
         """
@@ -1033,15 +1033,15 @@
         *,
         ApiId: str,
         RouteId: str,
         RouteResponseId: str,
         ModelSelectionExpression: str = ...,
         ResponseModels: Mapping[str, str] = ...,
         ResponseParameters: Mapping[str, ParameterConstraintsTypeDef] = ...,
-        RouteResponseKey: str = ...
+        RouteResponseKey: str = ...,
     ) -> UpdateRouteResponseResponseTypeDef:
         """
         Updates a RouteResponse.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_route_response)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_route_response)
         """
@@ -1054,15 +1054,15 @@
         AccessLogSettings: AccessLogSettingsTypeDef = ...,
         AutoDeploy: bool = ...,
         ClientCertificateId: str = ...,
         DefaultRouteSettings: RouteSettingsTypeDef = ...,
         DeploymentId: str = ...,
         Description: str = ...,
         RouteSettings: Mapping[str, RouteSettingsTypeDef] = ...,
-        StageVariables: Mapping[str, str] = ...
+        StageVariables: Mapping[str, str] = ...,
     ) -> UpdateStageResponseTypeDef:
         """
         Updates a Stage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_stage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_stage)
         """
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/literals.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/literals.py`

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
     "AuthorizationTypeType",
     "AuthorizerTypeType",
     "ConnectionTypeType",
     "ContentHandlingStrategyType",
     "DeploymentStatusType",
     "DomainNameStatusType",
@@ -50,15 +49,14 @@
     "ApiGatewayV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AuthorizationTypeType = Literal["AWS_IAM", "CUSTOM", "JWT", "NONE"]
 AuthorizerTypeType = Literal["JWT", "REQUEST"]
 ConnectionTypeType = Literal["INTERNET", "VPC_LINK"]
 ContentHandlingStrategyType = Literal["CONVERT_TO_BINARY", "CONVERT_TO_TEXT"]
 DeploymentStatusType = Literal["DEPLOYED", "FAILED", "PENDING"]
 DomainNameStatusType = Literal[
     "AVAILABLE", "PENDING_CERTIFICATE_REIMPORT", "PENDING_OWNERSHIP_VERIFICATION", "UPDATING"
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/literals.pyi` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/paginator.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     "GetIntegrationsPaginator",
     "GetModelsPaginator",
     "GetRouteResponsesPaginator",
     "GetRoutesPaginator",
     "GetStagesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/paginator.pyi` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/type_defs.py` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/type_defs.py`

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
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
     "CorsPaginatorTypeDef",
     "CorsTypeDef",
     "JWTConfigurationPaginatorTypeDef",
     "JWTConfigurationTypeDef",
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2/type_defs.pyi` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
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
 
 <a id="types-aiobotocore-apigatewayv2"></a>
 
 # types-aiobotocore-apigatewayv2
 
 [![PyPI - types-aiobotocore-apigatewayv2](https://img.shields.io/pypi/v/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ApiGatewayV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
+[aiobotocore.ApiGatewayV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-apigatewayv2-2.9.0/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewayv2-2.9.1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

