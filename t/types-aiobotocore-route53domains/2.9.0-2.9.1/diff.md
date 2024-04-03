# Comparing `tmp/types-aiobotocore-route53domains-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53domains-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53domains-2.9.0.tar", last modified: Wed Dec 13 20:00:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53domains-2.9.1.tar", last modified: Thu Jan 18 01:21:40 2024, max compression
```

## Comparing `types-aiobotocore-route53domains-2.9.0.tar` & `types-aiobotocore-route53domains-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.493214 types-aiobotocore-route53domains-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2023-12-13 20:00:21.493214 types-aiobotocore-route53domains-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12194 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:21.493214 types-aiobotocore-route53domains-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.493214 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30922 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30918 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13800 2023-12-13 19:54:57.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13798 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    25448 2023-12-13 19:54:57.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25447 2023-12-13 19:54:57.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:56.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:21.493214 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13785 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      946 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-12-13 20:00:21.000000 types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.713071 types-aiobotocore-route53domains-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-01-18 01:21:40.713071 types-aiobotocore-route53domains-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12194 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:40.713071 types-aiobotocore-route53domains-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.709071 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30928 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30925 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13798 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25447 2024-01-18 01:16:31.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25447 2024-01-18 01:16:31.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:30.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:40.713071 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13805 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-18 01:21:40.000000 types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53domains-2.9.0/LICENSE` & `types-aiobotocore-route53domains-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53domains-2.9.0/PKG-INFO` & `types-aiobotocore-route53domains-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53domains
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53Domains 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53Domains 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/
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
 
 <a id="types-aiobotocore-route53domains"></a>
 
 # types-aiobotocore-route53domains
 
 [![PyPI - types-aiobotocore-route53domains](https://img.shields.io/pypi/v/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Domains 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[aiobotocore.Route53Domains 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53domains-2.9.0/README.md` & `types-aiobotocore-route53domains-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Domains 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[aiobotocore.Route53Domains 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53domains-2.9.0/setup.py` & `types-aiobotocore-route53domains-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53domains",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53Domains 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Route53Domains 2.9.1 service generated with"
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
     keywords="aiobotocore route53domains type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53domains": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__init__.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListOperationsPaginator,
     ListPricesPaginator,
     ViewBillingPaginator,
 )
 
 Client = Route53DomainsClient
 
-
 __all__ = (
     "Client",
     "ListDomainsPaginator",
     "ListOperationsPaginator",
     "ListPricesPaginator",
     "Route53DomainsClient",
     "ViewBillingPaginator",
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__init__.pyi` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/__main__.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/__main__.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53Domains 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53Domains 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
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

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/client.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53DomainsClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -314,15 +313,15 @@
 
     async def list_domains(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListDomainsResponseTypeDef:
         """
         This operation returns all the domain names registered with Amazon Route 53 for
         the current Amazon Web Services account if no filtering conditions are
         used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
@@ -334,15 +333,15 @@
         *,
         SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListOperationsResponseTypeDef:
         """
         Returns information about all of the operations that return an operation ID and
         that have ever been performed on domains that were registered by the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_operations)
@@ -387,15 +386,15 @@
         AdminContact: ContactDetailTypeDef,
         RegistrantContact: ContactDetailTypeDef,
         TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
-        PrivacyProtectTechContact: bool = ...
+        PrivacyProtectTechContact: bool = ...,
     ) -> RegisterDomainResponseTypeDef:
         """
         This operation registers a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.register_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#register_domain)
         """
@@ -465,15 +464,15 @@
         TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         Nameservers: Sequence[NameserverTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
-        PrivacyProtectTechContact: bool = ...
+        PrivacyProtectTechContact: bool = ...,
     ) -> TransferDomainResponseTypeDef:
         """
         Transfers a domain from another registrar to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain)
         """
@@ -493,30 +492,30 @@
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
         AdminContact: ContactDetailTypeDef = ...,
         RegistrantContact: ContactDetailTypeDef = ...,
         TechContact: ContactDetailTypeDef = ...,
-        Consent: ConsentTypeDef = ...
+        Consent: ConsentTypeDef = ...,
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
         """
 
     async def update_domain_contact_privacy(
         self,
         *,
         DomainName: str,
         AdminPrivacy: bool = ...,
         RegistrantPrivacy: bool = ...,
-        TechPrivacy: bool = ...
+        TechPrivacy: bool = ...,
     ) -> UpdateDomainContactPrivacyResponseTypeDef:
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
@@ -545,15 +544,15 @@
 
     async def view_billing(
         self,
         *,
         Start: TimestampTypeDef = ...,
         End: TimestampTypeDef = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.view_billing)
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/client.pyi` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,15 @@
 
     async def list_domains(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ListDomainsResponseTypeDef:
         """
         This operation returns all the domain names registered with Amazon Route 53 for
         the current Amazon Web Services account if no filtering conditions are
         used.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_domains)
@@ -330,15 +330,15 @@
         *,
         SubmittedSince: TimestampTypeDef = ...,
         Marker: str = ...,
         MaxItems: int = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListOperationsResponseTypeDef:
         """
         Returns information about all of the operations that return an operation ID and
         that have ever been performed on domains that were registered by the current
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.list_operations)
@@ -383,15 +383,15 @@
         AdminContact: ContactDetailTypeDef,
         RegistrantContact: ContactDetailTypeDef,
         TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
-        PrivacyProtectTechContact: bool = ...
+        PrivacyProtectTechContact: bool = ...,
     ) -> RegisterDomainResponseTypeDef:
         """
         This operation registers a domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.register_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#register_domain)
         """
@@ -461,15 +461,15 @@
         TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         Nameservers: Sequence[NameserverTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
-        PrivacyProtectTechContact: bool = ...
+        PrivacyProtectTechContact: bool = ...,
     ) -> TransferDomainResponseTypeDef:
         """
         Transfers a domain from another registrar to Amazon Route 53.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain)
         """
@@ -489,30 +489,30 @@
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
         AdminContact: ContactDetailTypeDef = ...,
         RegistrantContact: ContactDetailTypeDef = ...,
         TechContact: ContactDetailTypeDef = ...,
-        Consent: ConsentTypeDef = ...
+        Consent: ConsentTypeDef = ...,
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
         """
 
     async def update_domain_contact_privacy(
         self,
         *,
         DomainName: str,
         AdminPrivacy: bool = ...,
         RegistrantPrivacy: bool = ...,
-        TechPrivacy: bool = ...
+        TechPrivacy: bool = ...,
     ) -> UpdateDomainContactPrivacyResponseTypeDef:
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
@@ -541,15 +541,15 @@
 
     async def view_billing(
         self,
         *,
         Start: TimestampTypeDef = ...,
         End: TimestampTypeDef = ...,
         Marker: str = ...,
-        MaxItems: int = ...
+        MaxItems: int = ...,
     ) -> ViewBillingResponseTypeDef:
         """
         Returns all the domain-related billing records for the current Amazon Web
         Services account for a specified period See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/route53domains-2014-05-15/ViewBilling).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.view_billing)
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/literals.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/literals.py`

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
     "ContactTypeType",
     "CountryCodeType",
     "DomainAvailabilityType",
     "ExtraParamNameType",
     "ListDomainsAttributeNameType",
     "ListDomainsPaginatorName",
@@ -41,15 +40,14 @@
     "Route53DomainsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContactTypeType = Literal["ASSOCIATION", "COMPANY", "PERSON", "PUBLIC_BODY", "RESELLER"]
 CountryCodeType = Literal[
     "AC",
     "AD",
     "AE",
     "AF",
     "AG",
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/literals.pyi` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/paginator.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,23 +46,21 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDomainsPaginator",
     "ListOperationsPaginator",
     "ListPricesPaginator",
     "ViewBillingPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -76,15 +74,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
         """
 
 
@@ -98,15 +96,15 @@
         self,
         *,
         SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
         """
 
 
@@ -132,13 +130,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: TimestampTypeDef = ...,
         End: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/paginator.pyi` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     """
 
     def paginate(
         self,
         *,
         FilterConditions: Sequence[FilterConditionTypeDef] = ...,
         SortCondition: SortConditionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDomainsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listdomainspaginator)
         """
 
 class ListOperationsPaginator(AioPaginator):
@@ -93,15 +93,15 @@
         self,
         *,
         SubmittedSince: TimestampTypeDef = ...,
         Status: Sequence[OperationStatusType] = ...,
         Type: Sequence[OperationTypeType] = ...,
         SortBy: Literal["SubmittedDate"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListOperationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ListOperations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#listoperationspaginator)
         """
 
 class ListPricesPaginator(AioPaginator):
@@ -125,13 +125,13 @@
     """
 
     def paginate(
         self,
         *,
         Start: TimestampTypeDef = ...,
         End: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ViewBillingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Paginator.ViewBilling.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/paginators/#viewbillingpaginator)
         """
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/type_defs.py` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DnssecSigningAttributesTypeDef",
     "BillingRecordTypeDef",
     "CancelDomainTransferToAnotherAwsAccountRequestRequestTypeDef",
     "CheckDomainAvailabilityRequestRequestTypeDef",
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains/type_defs.pyi` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/PKG-INFO` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53domains
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53Domains 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53Domains 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/
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
 
 <a id="types-aiobotocore-route53domains"></a>
 
 # types-aiobotocore-route53domains
 
 [![PyPI - types-aiobotocore-route53domains](https://img.shields.io/pypi/v/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53domains.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53domains)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53domains)](https://pepy.tech/project/types-aiobotocore-route53domains)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53Domains 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
+[aiobotocore.Route53Domains 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains)
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
 [types-aiobotocore-route53domains docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53domains-2.9.0/types_aiobotocore_route53domains.egg-info/SOURCES.txt` & `types-aiobotocore-route53domains-2.9.1/types_aiobotocore_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

