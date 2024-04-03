# Comparing `tmp/types-aiobotocore-cloudsearchdomain-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudsearchdomain-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.9.0.tar", last modified: Wed Dec 13 19:58:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudsearchdomain-2.9.1.tar", last modified: Thu Jan 18 01:20:17 2024, max compression
```

## Comparing `types-aiobotocore-cloudsearchdomain-2.9.0.tar` & `types-aiobotocore-cloudsearchdomain-2.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.085961 types-aiobotocore-cloudsearchdomain-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2023-12-13 19:58:51.085961 types-aiobotocore-cloudsearchdomain-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11130 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:51.085961 types-aiobotocore-cloudsearchdomain-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.085961 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/
--rw-r--r--   0 runner    (1001) docker     (127)      523 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6366 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8332 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:33.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:51.085961 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12733 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:51.000000 types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.729455 types-aiobotocore-cloudsearchdomain-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-01-18 01:20:17.729455 types-aiobotocore-cloudsearchdomain-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:17.729455 types-aiobotocore-cloudsearchdomain-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.725455 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:29.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:17.729455 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:17.000000 types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/LICENSE` & `types-aiobotocore-cloudsearchdomain-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
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
 
 <a id="types-aiobotocore-cloudsearchdomain"></a>
 
 # types-aiobotocore-cloudsearchdomain
 
 [![PyPI - types-aiobotocore-cloudsearchdomain](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/README.md` & `types-aiobotocore-cloudsearchdomain-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/setup.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudsearchdomain",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudsearchdomain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudSearchDomain 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudSearchDomain 2.9.1 service generated with"
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
     keywords="aiobotocore cloudsearchdomain type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudsearchdomain": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__init__.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,9 +18,8 @@
     ```
 """
 
 from .client import CloudSearchDomainClient
 
 Client = CloudSearchDomainClient
 
-
 __all__ = ("Client", "CloudSearchDomainClient")
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__init__.pyi` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/__main__.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudSearchDomain 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudSearchDomain 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain\nOther"
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

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/client.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         partial: bool = ...,
         queryOptions: str = ...,
         queryParser: QueryParserType = ...,
         returnFields: str = ...,
         size: int = ...,
         sort: str = ...,
         start: int = ...,
-        stats: str = ...
+        stats: str = ...,
     ) -> SearchResponseTypeDef:
         """
         Retrieves a list of documents that match the specified search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#search)
         """
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/client.pyi` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         partial: bool = ...,
         queryOptions: str = ...,
         queryParser: QueryParserType = ...,
         returnFields: str = ...,
         size: int = ...,
         sort: str = ...,
         start: int = ...,
-        stats: str = ...
+        stats: str = ...,
     ) -> SearchResponseTypeDef:
         """
         Retrieves a list of documents that match the specified search criteria.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/client/#search)
         """
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/literals.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContentTypeType",
     "QueryParserType",
     "CloudSearchDomainServiceName",
     "ServiceName",
     "ResourceServiceName",
 )
 
-
 ContentTypeType = Literal["application/json", "application/xml"]
 QueryParserType = Literal["dismax", "lucene", "simple", "structured"]
 CloudSearchDomainServiceName = Literal["cloudsearchdomain"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/literals.pyi` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/type_defs.py` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlobTypeDef",
     "BucketTypeDef",
     "DocumentServiceWarningTypeDef",
     "FieldStatsTypeDef",
     "HitTypeDef",
     "ResponseMetadataTypeDef",
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain/type_defs.pyi` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudsearchdomain
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudSearchDomain 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudSearchDomain 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/
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
 
 <a id="types-aiobotocore-cloudsearchdomain"></a>
 
 # types-aiobotocore-cloudsearchdomain
 
 [![PyPI - types-aiobotocore-cloudsearchdomain](https://img.shields.io/pypi/v/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudsearchdomain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudsearchdomain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudsearchdomain)](https://pepy.tech/project/types-aiobotocore-cloudsearchdomain)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudSearchDomain 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
+[aiobotocore.CloudSearchDomain 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
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
 [types-aiobotocore-cloudsearchdomain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudsearchdomain/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudsearchdomain-2.9.0/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt` & `types-aiobotocore-cloudsearchdomain-2.9.1/types_aiobotocore_cloudsearchdomain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

