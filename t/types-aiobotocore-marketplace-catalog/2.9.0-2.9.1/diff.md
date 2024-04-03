# Comparing `tmp/types-aiobotocore-marketplace-catalog-2.9.0.tar.gz` & `tmp/types-aiobotocore-marketplace-catalog-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.9.0.tar", last modified: Wed Dec 13 19:59:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.9.1.tar", last modified: Thu Jan 18 01:21:12 2024, max compression
```

## Comparing `types-aiobotocore-marketplace-catalog-2.9.0.tar` & `types-aiobotocore-marketplace-catalog-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.837484 types-aiobotocore-marketplace-catalog-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2023-12-13 19:59:50.837484 types-aiobotocore-marketplace-catalog-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:50.837484 types-aiobotocore-marketplace-catalog-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2023-12-13 19:49:44.000000 types-aiobotocore-marketplace-catalog-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.837484 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      978 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14138 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14134 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10751 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10749 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30647 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30646 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:45.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:50.837484 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13790 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:50.000000 types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.925196 types-aiobotocore-marketplace-catalog-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-01-18 01:21:12.925196 types-aiobotocore-marketplace-catalog-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:12.925196 types-aiobotocore-marketplace-catalog-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.925196 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14140 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10749 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30646 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30646 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:30.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:12.925196 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:12.000000 types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/LICENSE` & `types-aiobotocore-marketplace-catalog-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
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
 
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/README.md` & `types-aiobotocore-marketplace-catalog-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/setup.py` & `types-aiobotocore-marketplace-catalog-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-catalog",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MarketplaceCatalog 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MarketplaceCatalog 2.9.1 service generated with"
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
     keywords="aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_marketplace_catalog": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__init__.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,8 @@
 """
 
 from .client import MarketplaceCatalogClient
 from .paginator import ListChangeSetsPaginator, ListEntitiesPaginator
 
 Client = MarketplaceCatalogClient
 
-
 __all__ = ("Client", "ListChangeSetsPaginator", "ListEntitiesPaginator", "MarketplaceCatalogClient")
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__init__.pyi` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/__main__.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceCatalog 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceCatalog 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
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

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/client.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MarketplaceCatalogClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -167,15 +166,15 @@
     async def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChangeSetsResponseTypeDef:
         """
         Returns the list of change sets owned by the account being used to make the
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_change_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#list_change_sets)
@@ -188,15 +187,15 @@
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         OwnershipType: OwnershipTypeType = ...,
         EntityTypeFilters: EntityTypeFiltersTypeDef = ...,
-        EntityTypeSort: EntityTypeSortTypeDef = ...
+        EntityTypeSort: EntityTypeSortTypeDef = ...,
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#list_entities)
         """
@@ -225,15 +224,15 @@
     async def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
-        ChangeSetTags: Sequence[TagTypeDef] = ...
+        ChangeSetTags: Sequence[TagTypeDef] = ...,
     ) -> StartChangeSetResponseTypeDef:
         """
         Allows you to request changes for your entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.start_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#start_change_set)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/client.pyi` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     async def list_change_sets(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListChangeSetsResponseTypeDef:
         """
         Returns the list of change sets owned by the account being used to make the
         call.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_change_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#list_change_sets)
@@ -184,15 +184,15 @@
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         OwnershipType: OwnershipTypeType = ...,
         EntityTypeFilters: EntityTypeFiltersTypeDef = ...,
-        EntityTypeSort: EntityTypeSortTypeDef = ...
+        EntityTypeSort: EntityTypeSortTypeDef = ...,
     ) -> ListEntitiesResponseTypeDef:
         """
         Provides the list of entities of a given type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#list_entities)
         """
@@ -221,15 +221,15 @@
     async def start_change_set(
         self,
         *,
         Catalog: str,
         ChangeSet: Sequence[ChangeTypeDef],
         ChangeSetName: str = ...,
         ClientRequestToken: str = ...,
-        ChangeSetTags: Sequence[TagTypeDef] = ...
+        ChangeSetTags: Sequence[TagTypeDef] = ...,
     ) -> StartChangeSetResponseTypeDef:
         """
         Allows you to request changes for your entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.start_change_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/client/#start_change_set)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/literals.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/literals.py`

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
     "AmiProductSortByType",
     "AmiProductVisibilityStringType",
     "ChangeStatusType",
     "ContainerProductSortByType",
     "ContainerProductVisibilityStringType",
     "DataProductSortByType",
@@ -43,15 +42,14 @@
     "MarketplaceCatalogServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AmiProductSortByType = Literal["EntityId", "LastModifiedDate", "ProductTitle", "Visibility"]
 AmiProductVisibilityStringType = Literal["Draft", "Limited", "Public", "Restricted"]
 ChangeStatusType = Literal["APPLYING", "CANCELLED", "FAILED", "PREPARING", "SUCCEEDED"]
 ContainerProductSortByType = Literal["EntityId", "LastModifiedDate", "ProductTitle", "Visibility"]
 ContainerProductVisibilityStringType = Literal["Draft", "Limited", "Public", "Restricted"]
 DataProductSortByType = Literal["EntityId", "LastModifiedDate", "ProductTitle", "Visibility"]
 DataProductVisibilityStringType = Literal["Draft", "Limited", "Public", "Restricted", "Unavailable"]
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/literals.pyi` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/paginator.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
     ListEntitiesResponseTypeDef,
     PaginatorConfigTypeDef,
     SortTypeDef,
 )
 
 __all__ = ("ListChangeSetsPaginator", "ListEntitiesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -60,15 +59,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 
@@ -84,13 +83,13 @@
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
         EntityTypeFilters: EntityTypeFiltersTypeDef = ...,
         EntityTypeSort: EntityTypeSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/paginator.pyi` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 class ListEntitiesPaginator(AioPaginator):
@@ -80,13 +80,13 @@
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
         EntityTypeFilters: EntityTypeFiltersTypeDef = ...,
         EntityTypeSort: EntityTypeSortTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/type_defs.py` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/type_defs.py`

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
     "AmiProductEntityIdFilterTypeDef",
     "AmiProductTitleFilterTypeDef",
     "AmiProductVisibilityFilterTypeDef",
     "AmiProductLastModifiedDateFilterDateRangeTypeDef",
     "AmiProductSortTypeDef",
     "AmiProductSummaryTypeDef",
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog/type_defs.pyi` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
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
 
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceCatalog 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
+[aiobotocore.MarketplaceCatalog 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-catalog-2.9.0/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-catalog-2.9.1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

