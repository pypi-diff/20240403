# Comparing `tmp/types-aiobotocore-marketplace-entitlement-2.9.0.tar.gz` & `tmp/types-aiobotocore-marketplace-entitlement-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-entitlement-2.9.0.tar", last modified: Wed Dec 13 19:59:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-entitlement-2.9.1.tar", last modified: Thu Jan 18 01:21:13 2024, max compression
```

## Comparing `types-aiobotocore-marketplace-entitlement-2.9.0.tar` & `types-aiobotocore-marketplace-entitlement-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.573477 types-aiobotocore-marketplace-entitlement-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2023-12-13 19:59:51.573477 types-aiobotocore-marketplace-entitlement-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12345 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:51.573477 types-aiobotocore-marketplace-entitlement-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.573477 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5996 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8551 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:46.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:51.573477 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13978 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-13 19:59:51.000000 types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.601193 types-aiobotocore-marketplace-entitlement-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-01-18 01:21:13.601193 types-aiobotocore-marketplace-entitlement-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12345 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:13.601193 types-aiobotocore-marketplace-entitlement-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.597193 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5997 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:31.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:13.601193 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13998 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-18 01:21:13.000000 types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/LICENSE` & `types-aiobotocore-marketplace-entitlement-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/PKG-INFO` & `types-aiobotocore-marketplace-entitlement-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-entitlement
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/
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
 
 <a id="types-aiobotocore-marketplace-entitlement"></a>
 
 # types-aiobotocore-marketplace-entitlement
 
 [![PyPI - types-aiobotocore-marketplace-entitlement](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [types-aiobotocore-marketplace-entitlement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/README.md` & `types-aiobotocore-marketplace-entitlement-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [types-aiobotocore-marketplace-entitlement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/setup.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-entitlement",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_marketplace_entitlement"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.0 service generated"
-        " with mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.1 service generated"
+        " with mypy-boto3-builder 7.23.1"
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
         "aiobotocore marketplace-entitlement type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_marketplace_entitlement": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__init__.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import MarketplaceEntitlementServiceClient
 from .paginator import GetEntitlementsPaginator
 
 Client = MarketplaceEntitlementServiceClient
 
-
 __all__ = ("Client", "GetEntitlementsPaginator", "MarketplaceEntitlementServiceClient")
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__init__.pyi` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/__main__.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService\nOther"
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

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/client.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from .type_defs import GetEntitlementsResultTypeDef
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MarketplaceEntitlementServiceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -98,15 +97,15 @@
 
     async def get_entitlements(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEntitlementsResultTypeDef:
         """
         GetEntitlements retrieves entitlement values for a given product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/client/#get_entitlements)
         """
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/client.pyi` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
     async def get_entitlements(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> GetEntitlementsResultTypeDef:
         """
         GetEntitlements retrieves entitlement values for a given product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/client/#get_entitlements)
         """
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/literals.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "GetEntitlementFilterNameType",
     "GetEntitlementsPaginatorName",
     "MarketplaceEntitlementServiceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 GetEntitlementFilterNameType = Literal["CUSTOMER_IDENTIFIER", "DIMENSION"]
 GetEntitlementsPaginatorName = Literal["get_entitlements"]
 MarketplaceEntitlementServiceServiceName = Literal["marketplace-entitlement"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/literals.pyi` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/paginator.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from botocore.paginate import PageIterator
 
 from .literals import GetEntitlementFilterNameType
 from .type_defs import GetEntitlementsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("GetEntitlementsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -49,13 +48,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/paginator.pyi` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,13 +46,13 @@
     """
 
     def paginate(
         self,
         *,
         ProductCode: str,
         Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEntitlementsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/paginators/#getentitlementspaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/type_defs.py` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EntitlementValueTypeDef",
     "PaginatorConfigTypeDef",
     "GetEntitlementsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EntitlementTypeDef",
     "GetEntitlementsRequestGetEntitlementsPaginateTypeDef",
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement/type_defs.pyi` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-entitlement
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MarketplaceEntitlementService 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/
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
 
 <a id="types-aiobotocore-marketplace-entitlement"></a>
 
 # types-aiobotocore-marketplace-entitlement
 
 [![PyPI - types-aiobotocore-marketplace-entitlement](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-entitlement.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-entitlement)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-entitlement)](https://pepy.tech/project/types-aiobotocore-marketplace-entitlement)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MarketplaceEntitlementService 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
+[aiobotocore.MarketplaceEntitlementService 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
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
 [types-aiobotocore-marketplace-entitlement docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_entitlement/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-marketplace-entitlement-2.9.0/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-entitlement-2.9.1/types_aiobotocore_marketplace_entitlement.egg-info/SOURCES.txt`

 * *Files identical despite different names*

