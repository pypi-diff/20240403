# Comparing `tmp/types-aiobotocore-route53-2.9.0.tar.gz` & `tmp/types-aiobotocore-route53-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-2.9.0.tar", last modified: Wed Dec 13 20:00:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-2.9.1.tar", last modified: Thu Jan 18 01:21:39 2024, max compression
```

## Comparing `types-aiobotocore-route53-2.9.0.tar` & `types-aiobotocore-route53-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.989228 types-aiobotocore-route53-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2023-12-13 20:00:19.989228 types-aiobotocore-route53-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13321 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:19.989228 types-aiobotocore-route53-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.989228 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58549 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    58545 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    13719 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10464 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10453 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54920 2023-12-13 19:54:50.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    54919 2023-12-13 19:54:50.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:48.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-12-13 19:54:49.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:19.989228 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14884 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 20:00:19.000000 types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.361077 types-aiobotocore-route53-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-01-18 01:21:39.361077 types-aiobotocore-route53-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13321 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:39.361077 types-aiobotocore-route53-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.357077 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58562 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58559 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13719 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10456 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54919 2024-01-18 01:16:23.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54919 2024-01-18 01:16:23.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:21.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-18 01:16:22.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:39.361077 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14904 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:21:39.000000 types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-2.9.0/LICENSE` & `types-aiobotocore-route53-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-route53-2.9.0/PKG-INFO` & `types-aiobotocore-route53-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/
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
 
 <a id="types-aiobotocore-route53"></a>
 
 # types-aiobotocore-route53
 
 [![PyPI - types-aiobotocore-route53](https://img.shields.io/pypi/v/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[aiobotocore.Route53 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-2.9.0/README.md` & `types-aiobotocore-route53-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[aiobotocore.Route53 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-2.9.0/setup.py` & `types-aiobotocore-route53-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Route53 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Route53 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore route53 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__init__.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
     ListResourceRecordSetsPaginator,
     ListVPCAssociationAuthorizationsPaginator,
 )
 from .waiter import ResourceRecordSetsChangedWaiter
 
 Client = Route53Client
 
-
 __all__ = (
     "Client",
     "ListCidrBlocksPaginator",
     "ListCidrCollectionsPaginator",
     "ListCidrLocationsPaginator",
     "ListHealthChecksPaginator",
     "ListHostedZonesPaginator",
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__init__.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/__main__.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Route53 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/client.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,14 @@
 from .waiter import ResourceRecordSetsChangedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Route53Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -250,15 +249,15 @@
         """
 
     async def change_cidr_collection(
         self,
         *,
         Id: str,
         Changes: Sequence[CidrCollectionChangeTypeDef],
-        CollectionVersion: int = ...
+        CollectionVersion: int = ...,
     ) -> ChangeCidrCollectionResponseTypeDef:
         """
         Creates, changes, or deletes CIDR blocks within a collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#change_cidr_collection)
         """
@@ -277,15 +276,15 @@
 
     async def change_tags_for_resource(
         self,
         *,
         ResourceType: TagResourceTypeType,
         ResourceId: str,
         AddTags: Sequence[TagTypeDef] = ...,
-        RemoveTagKeys: Sequence[str] = ...
+        RemoveTagKeys: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Adds, edits, or deletes tags for a health check or a hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#change_tags_for_resource)
         """
@@ -321,15 +320,15 @@
     async def create_hosted_zone(
         self,
         *,
         Name: str,
         CallerReference: str,
         VPC: VPCTypeDef = ...,
         HostedZoneConfig: HostedZoneConfigTypeDef = ...,
-        DelegationSetId: str = ...
+        DelegationSetId: str = ...,
     ) -> CreateHostedZoneResponseTypeDef:
         """
         Creates a new public or private hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_hosted_zone)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_hosted_zone)
         """
@@ -337,15 +336,15 @@
     async def create_key_signing_key(
         self,
         *,
         CallerReference: str,
         HostedZoneId: str,
         KeyManagementServiceArn: str,
         Name: str,
-        Status: str
+        Status: str,
     ) -> CreateKeySigningKeyResponseTypeDef:
         """
         Creates a new key-signing key (KSK) associated with a hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_key_signing_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_key_signing_key)
         """
@@ -387,15 +386,15 @@
     async def create_traffic_policy_instance(
         self,
         *,
         HostedZoneId: str,
         Name: str,
         TTL: int,
         TrafficPolicyId: str,
-        TrafficPolicyVersion: int
+        TrafficPolicyVersion: int,
     ) -> CreateTrafficPolicyInstanceResponseTypeDef:
         """
         Creates resource record sets in a specified hosted zone based on the settings
         in a specified traffic policy
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_traffic_policy_instance)
@@ -748,15 +747,15 @@
 
     async def list_cidr_blocks(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
         NextToken: str = ...,
-        MaxResults: str = ...
+        MaxResults: str = ...,
     ) -> ListCidrBlocksResponseTypeDef:
         """
         Returns a paginated list of location objects and their CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_cidr_blocks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_cidr_blocks)
         """
@@ -787,15 +786,15 @@
 
     async def list_geo_locations(
         self,
         *,
         StartContinentCode: str = ...,
         StartCountryCode: str = ...,
         StartSubdivisionCode: str = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListGeoLocationsResponseTypeDef:
         """
         Retrieves a list of supported geographic locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_geo_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_geo_locations)
         """
@@ -814,15 +813,15 @@
 
     async def list_hosted_zones(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         DelegationSetId: str = ...,
-        HostedZoneType: Literal["PrivateHostedZone"] = ...
+        HostedZoneType: Literal["PrivateHostedZone"] = ...,
     ) -> ListHostedZonesResponseTypeDef:
         """
         Retrieves a list of the public and private hosted zones that are associated
         with the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_hosted_zones)
@@ -868,15 +867,15 @@
     async def list_resource_record_sets(
         self,
         *,
         HostedZoneId: str,
         StartRecordName: str = ...,
         StartRecordType: RRTypeType = ...,
         StartRecordIdentifier: str = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListResourceRecordSetsResponseTypeDef:
         """
         Lists the resource record sets in a specified hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_resource_record_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_resource_record_sets)
         """
@@ -927,15 +926,15 @@
 
     async def list_traffic_policy_instances(
         self,
         *,
         HostedZoneIdMarker: str = ...,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created by using
         the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances)
@@ -944,15 +943,15 @@
 
     async def list_traffic_policy_instances_by_hosted_zone(
         self,
         *,
         HostedZoneId: str,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesByHostedZoneResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created in a
         specified hosted
         zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_hosted_zone)
@@ -963,15 +962,15 @@
         self,
         *,
         TrafficPolicyId: str,
         TrafficPolicyVersion: int,
         HostedZoneIdMarker: str = ...,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesByPolicyResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created by using a
         specify traffic policy
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_policy)
@@ -1005,15 +1004,15 @@
         self,
         *,
         HostedZoneId: str,
         RecordName: str,
         RecordType: RRTypeType,
         ResolverIP: str = ...,
         EDNS0ClientSubnetIP: str = ...,
-        EDNS0ClientSubnetMask: str = ...
+        EDNS0ClientSubnetMask: str = ...,
     ) -> TestDNSAnswerResponseTypeDef:
         """
         Gets the value that Amazon Route 53 returns in response to a DNS request for a
         specified record name and
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.test_dns_answer)
@@ -1035,15 +1034,15 @@
         Disabled: bool = ...,
         HealthThreshold: int = ...,
         ChildHealthChecks: Sequence[str] = ...,
         EnableSNI: bool = ...,
         Regions: Sequence[HealthCheckRegionType] = ...,
         AlarmIdentifier: AlarmIdentifierTypeDef = ...,
         InsufficientDataHealthStatus: InsufficientDataHealthStatusType = ...,
-        ResetElements: Sequence[ResettableElementNameType] = ...
+        ResetElements: Sequence[ResettableElementNameType] = ...,
     ) -> UpdateHealthCheckResponseTypeDef:
         """
         Updates an existing health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#update_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/client.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         """
 
     async def change_cidr_collection(
         self,
         *,
         Id: str,
         Changes: Sequence[CidrCollectionChangeTypeDef],
-        CollectionVersion: int = ...
+        CollectionVersion: int = ...,
     ) -> ChangeCidrCollectionResponseTypeDef:
         """
         Creates, changes, or deletes CIDR blocks within a collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#change_cidr_collection)
         """
@@ -273,15 +273,15 @@
 
     async def change_tags_for_resource(
         self,
         *,
         ResourceType: TagResourceTypeType,
         ResourceId: str,
         AddTags: Sequence[TagTypeDef] = ...,
-        RemoveTagKeys: Sequence[str] = ...
+        RemoveTagKeys: Sequence[str] = ...,
     ) -> Dict[str, Any]:
         """
         Adds, edits, or deletes tags for a health check or a hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.change_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#change_tags_for_resource)
         """
@@ -317,15 +317,15 @@
     async def create_hosted_zone(
         self,
         *,
         Name: str,
         CallerReference: str,
         VPC: VPCTypeDef = ...,
         HostedZoneConfig: HostedZoneConfigTypeDef = ...,
-        DelegationSetId: str = ...
+        DelegationSetId: str = ...,
     ) -> CreateHostedZoneResponseTypeDef:
         """
         Creates a new public or private hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_hosted_zone)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_hosted_zone)
         """
@@ -333,15 +333,15 @@
     async def create_key_signing_key(
         self,
         *,
         CallerReference: str,
         HostedZoneId: str,
         KeyManagementServiceArn: str,
         Name: str,
-        Status: str
+        Status: str,
     ) -> CreateKeySigningKeyResponseTypeDef:
         """
         Creates a new key-signing key (KSK) associated with a hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_key_signing_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_key_signing_key)
         """
@@ -383,15 +383,15 @@
     async def create_traffic_policy_instance(
         self,
         *,
         HostedZoneId: str,
         Name: str,
         TTL: int,
         TrafficPolicyId: str,
-        TrafficPolicyVersion: int
+        TrafficPolicyVersion: int,
     ) -> CreateTrafficPolicyInstanceResponseTypeDef:
         """
         Creates resource record sets in a specified hosted zone based on the settings
         in a specified traffic policy
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_traffic_policy_instance)
@@ -744,15 +744,15 @@
 
     async def list_cidr_blocks(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
         NextToken: str = ...,
-        MaxResults: str = ...
+        MaxResults: str = ...,
     ) -> ListCidrBlocksResponseTypeDef:
         """
         Returns a paginated list of location objects and their CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_cidr_blocks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_cidr_blocks)
         """
@@ -783,15 +783,15 @@
 
     async def list_geo_locations(
         self,
         *,
         StartContinentCode: str = ...,
         StartCountryCode: str = ...,
         StartSubdivisionCode: str = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListGeoLocationsResponseTypeDef:
         """
         Retrieves a list of supported geographic locations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_geo_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_geo_locations)
         """
@@ -810,15 +810,15 @@
 
     async def list_hosted_zones(
         self,
         *,
         Marker: str = ...,
         MaxItems: str = ...,
         DelegationSetId: str = ...,
-        HostedZoneType: Literal["PrivateHostedZone"] = ...
+        HostedZoneType: Literal["PrivateHostedZone"] = ...,
     ) -> ListHostedZonesResponseTypeDef:
         """
         Retrieves a list of the public and private hosted zones that are associated
         with the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_hosted_zones)
@@ -864,15 +864,15 @@
     async def list_resource_record_sets(
         self,
         *,
         HostedZoneId: str,
         StartRecordName: str = ...,
         StartRecordType: RRTypeType = ...,
         StartRecordIdentifier: str = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListResourceRecordSetsResponseTypeDef:
         """
         Lists the resource record sets in a specified hosted zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_resource_record_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#list_resource_record_sets)
         """
@@ -923,15 +923,15 @@
 
     async def list_traffic_policy_instances(
         self,
         *,
         HostedZoneIdMarker: str = ...,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created by using
         the current Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances)
@@ -940,15 +940,15 @@
 
     async def list_traffic_policy_instances_by_hosted_zone(
         self,
         *,
         HostedZoneId: str,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesByHostedZoneResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created in a
         specified hosted
         zone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_hosted_zone)
@@ -959,15 +959,15 @@
         self,
         *,
         TrafficPolicyId: str,
         TrafficPolicyVersion: int,
         HostedZoneIdMarker: str = ...,
         TrafficPolicyInstanceNameMarker: str = ...,
         TrafficPolicyInstanceTypeMarker: RRTypeType = ...,
-        MaxItems: str = ...
+        MaxItems: str = ...,
     ) -> ListTrafficPolicyInstancesByPolicyResponseTypeDef:
         """
         Gets information about the traffic policy instances that you created by using a
         specify traffic policy
         version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.list_traffic_policy_instances_by_policy)
@@ -1001,15 +1001,15 @@
         self,
         *,
         HostedZoneId: str,
         RecordName: str,
         RecordType: RRTypeType,
         ResolverIP: str = ...,
         EDNS0ClientSubnetIP: str = ...,
-        EDNS0ClientSubnetMask: str = ...
+        EDNS0ClientSubnetMask: str = ...,
     ) -> TestDNSAnswerResponseTypeDef:
         """
         Gets the value that Amazon Route 53 returns in response to a DNS request for a
         specified record name and
         type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.test_dns_answer)
@@ -1031,15 +1031,15 @@
         Disabled: bool = ...,
         HealthThreshold: int = ...,
         ChildHealthChecks: Sequence[str] = ...,
         EnableSNI: bool = ...,
         Regions: Sequence[HealthCheckRegionType] = ...,
         AlarmIdentifier: AlarmIdentifierTypeDef = ...,
         InsufficientDataHealthStatus: InsufficientDataHealthStatusType = ...,
-        ResetElements: Sequence[ResettableElementNameType] = ...
+        ResetElements: Sequence[ResettableElementNameType] = ...,
     ) -> UpdateHealthCheckResponseTypeDef:
         """
         Updates an existing health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.update_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#update_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/literals.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/literals.py`

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
     "AccountLimitTypeType",
     "ChangeActionType",
     "ChangeStatusType",
     "CidrCollectionChangeActionType",
     "CloudWatchRegionType",
     "ComparisonOperatorType",
@@ -52,15 +51,14 @@
     "Route53ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
 )
 
-
 AccountLimitTypeType = Literal[
     "MAX_HEALTH_CHECKS_BY_OWNER",
     "MAX_HOSTED_ZONES_BY_OWNER",
     "MAX_REUSABLE_DELEGATION_SETS_BY_OWNER",
     "MAX_TRAFFIC_POLICIES_BY_OWNER",
     "MAX_TRAFFIC_POLICY_INSTANCES_BY_OWNER",
 ]
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/literals.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/paginator.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,25 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListCidrBlocksPaginator",
     "ListCidrCollectionsPaginator",
     "ListCidrLocationsPaginator",
     "ListHealthChecksPaginator",
     "ListHostedZonesPaginator",
     "ListQueryLoggingConfigsPaginator",
     "ListResourceRecordSetsPaginator",
     "ListVPCAssociationAuthorizationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -88,15 +86,15 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrblockspaginator)
         """
 
 
@@ -152,15 +150,15 @@
     """
 
     def paginate(
         self,
         *,
         DelegationSetId: str = ...,
         HostedZoneType: Literal["PrivateHostedZone"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
         """
 
 
@@ -201,13 +199,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/paginator.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrblockspaginator)
         """
 
 class ListCidrCollectionsPaginator(AioPaginator):
@@ -144,15 +144,15 @@
     """
 
     def paginate(
         self,
         *,
         DelegationSetId: str = ...,
         HostedZoneType: Literal["PrivateHostedZone"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
         """
 
 class ListQueryLoggingConfigsPaginator(AioPaginator):
@@ -190,13 +190,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/type_defs.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/type_defs.py`

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
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
     "ResponseMetadataTypeDef",
     "AlarmIdentifierTypeDef",
     "AliasTargetTypeDef",
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/type_defs.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/waiter.py` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53/waiter.pyi` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/PKG-INFO` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Route53 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Route53 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/
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
 
 <a id="types-aiobotocore-route53"></a>
 
 # types-aiobotocore-route53
 
 [![PyPI - types-aiobotocore-route53](https://img.shields.io/pypi/v/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Route53 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[aiobotocore.Route53 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-route53-2.9.0/types_aiobotocore_route53.egg-info/SOURCES.txt` & `types-aiobotocore-route53-2.9.1/types_aiobotocore_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

