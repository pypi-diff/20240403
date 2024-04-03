# Comparing `tmp/types-aiobotocore-glacier-2.9.0.tar.gz` & `tmp/types-aiobotocore-glacier-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glacier-2.9.0.tar", last modified: Wed Dec 13 19:59:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-glacier-2.9.1.tar", last modified: Thu Jan 18 01:20:46 2024, max compression
```

## Comparing `types-aiobotocore-glacier-2.9.0.tar` & `types-aiobotocore-glacier-2.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.773733 types-aiobotocore-glacier-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2023-12-13 19:59:22.769734 types-aiobotocore-glacier-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14906 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:22.773733 types-aiobotocore-glacier-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.769734 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      932 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28495 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28491 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10215 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10213 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    42797 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    42771 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    28992 2023-12-13 19:46:41.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    28991 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:46:38.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2023-12-13 19:46:40.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:22.769734 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-13 19:59:22.000000 types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.953313 types-aiobotocore-glacier-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-01-18 01:20:46.953313 types-aiobotocore-glacier-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14906 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:46.957313 types-aiobotocore-glacier-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-01-18 01:08:32.000000 types-aiobotocore-glacier-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.953313 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28501 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28498 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10213 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5307 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    43100 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43077 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    28991 2024-01-18 01:08:34.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28991 2024-01-18 01:08:34.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-01-18 01:08:33.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:46.953313 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16489 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-18 01:20:46.000000 types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glacier-2.9.0/LICENSE` & `types-aiobotocore-glacier-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-glacier-2.9.0/PKG-INFO` & `types-aiobotocore-glacier-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Glacier 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Glacier 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
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
 
 <a id="types-aiobotocore-glacier"></a>
 
 # types-aiobotocore-glacier
 
 [![PyPI - types-aiobotocore-glacier](https://img.shields.io/pypi/v/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [types-aiobotocore-glacier docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glacier-2.9.0/README.md` & `types-aiobotocore-glacier-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [types-aiobotocore-glacier docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glacier-2.9.0/setup.py` & `types-aiobotocore-glacier-2.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glacier",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Glacier 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Glacier 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore glacier type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_glacier": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__init__.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,18 +42,16 @@
     ListVaultsPaginator,
 )
 from .service_resource import GlacierServiceResource
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 Client = GlacierClient
 
-
 ServiceResource = GlacierServiceResource
 
-
 __all__ = (
     "Client",
     "GlacierClient",
     "GlacierServiceResource",
     "ListJobsPaginator",
     "ListMultipartUploadsPaginator",
     "ListPartsPaginator",
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__init__.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/__main__.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glacier 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Glacier 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/client.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GlacierClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -155,15 +154,15 @@
     async def complete_multipart_upload(
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         archiveSize: str = ...,
-        checksum: str = ...
+        checksum: str = ...,
     ) -> ArchiveCreationOutputTypeDef:
         """
         You call this operation to inform Amazon S3 Glacier (Glacier) that all the
         archive parts have been uploaded and that Glacier can now assemble the archive
         from the uploaded
         parts.
 
@@ -347,15 +346,15 @@
 
     async def initiate_multipart_upload(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
-        partSize: str = ...
+        partSize: str = ...,
     ) -> InitiateMultipartUploadOutputTypeDef:
         """
         This operation initiates a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#initiate_multipart_upload)
         """
@@ -376,15 +375,15 @@
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         limit: str = ...,
         marker: str = ...,
         statuscode: str = ...,
-        completed: str = ...
+        completed: str = ...,
     ) -> ListJobsOutputTypeDef:
         """
         This operation lists jobs for a vault, including jobs that are in-progress and
         jobs that have recently
         finished.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_jobs)
@@ -404,15 +403,15 @@
     async def list_parts(
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         marker: str = ...,
-        limit: str = ...
+        limit: str = ...,
     ) -> ListPartsOutputTypeDef:
         """
         This operation lists the parts of an archive that have been uploaded in a
         specific multipart
         upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_parts)
@@ -496,15 +495,15 @@
         """
 
     async def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
+        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
@@ -514,15 +513,15 @@
     async def upload_archive(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
         checksum: str = ...,
-        body: BlobTypeDef = ...
+        body: BlobTypeDef = ...,
     ) -> ArchiveCreationOutputTypeDef:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#upload_archive)
         """
@@ -531,15 +530,15 @@
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         checksum: str = ...,
         range: str = ...,
-        body: BlobTypeDef = ...
+        body: BlobTypeDef = ...,
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_multipart_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#upload_multipart_part)
         """
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/client.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     async def complete_multipart_upload(
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         archiveSize: str = ...,
-        checksum: str = ...
+        checksum: str = ...,
     ) -> ArchiveCreationOutputTypeDef:
         """
         You call this operation to inform Amazon S3 Glacier (Glacier) that all the
         archive parts have been uploaded and that Glacier can now assemble the archive
         from the uploaded
         parts.
 
@@ -343,15 +343,15 @@
 
     async def initiate_multipart_upload(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
-        partSize: str = ...
+        partSize: str = ...,
     ) -> InitiateMultipartUploadOutputTypeDef:
         """
         This operation initiates a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#initiate_multipart_upload)
         """
@@ -372,15 +372,15 @@
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         limit: str = ...,
         marker: str = ...,
         statuscode: str = ...,
-        completed: str = ...
+        completed: str = ...,
     ) -> ListJobsOutputTypeDef:
         """
         This operation lists jobs for a vault, including jobs that are in-progress and
         jobs that have recently
         finished.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_jobs)
@@ -400,15 +400,15 @@
     async def list_parts(
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         marker: str = ...,
-        limit: str = ...
+        limit: str = ...,
     ) -> ListPartsOutputTypeDef:
         """
         This operation lists the parts of an archive that have been uploaded in a
         specific multipart
         upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.list_parts)
@@ -492,15 +492,15 @@
         """
 
     async def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
+        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
@@ -510,15 +510,15 @@
     async def upload_archive(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
         archiveDescription: str = ...,
         checksum: str = ...,
-        body: BlobTypeDef = ...
+        body: BlobTypeDef = ...,
     ) -> ArchiveCreationOutputTypeDef:
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#upload_archive)
         """
@@ -527,15 +527,15 @@
         self,
         *,
         vaultName: str,
         uploadId: str,
         accountId: str = "-",
         checksum: str = ...,
         range: str = ...,
-        body: BlobTypeDef = ...
+        body: BlobTypeDef = ...,
     ) -> UploadMultipartPartOutputTypeDef:
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.upload_multipart_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#upload_multipart_part)
         """
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/literals.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/literals.py`

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
     "ActionCodeType",
     "CannedACLType",
     "EncryptionTypeType",
     "ExpressionTypeType",
     "FileHeaderInfoType",
     "ListJobsPaginatorName",
@@ -41,15 +40,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionCodeType = Literal["ArchiveRetrieval", "InventoryRetrieval", "Select"]
 CannedACLType = Literal[
     "authenticated-read",
     "aws-exec-read",
     "bucket-owner-full-control",
     "bucket-owner-read",
     "private",
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/literals.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/paginator.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 __all__ = (
     "ListJobsPaginator",
     "ListMultipartUploadsPaginator",
     "ListPartsPaginator",
     "ListVaultsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -67,15 +66,15 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/paginators/#listjobspaginator)
         """
 
 
@@ -102,15 +101,15 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/paginators/#listpartspaginator)
         """
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/paginator.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         statuscode: str = ...,
         completed: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/paginators/#listjobspaginator)
         """
 
 class ListMultipartUploadsPaginator(AioPaginator):
@@ -97,15 +97,15 @@
 
     def paginate(
         self,
         *,
         accountId: str,
         vaultName: str,
         uploadId: str,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPartsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Paginator.ListParts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/paginators/#listpartspaginator)
         """
 
 class ListVaultsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/service_resource.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 except ImportError:
     from builtins import object as AIOResourceCollection
 try:
     from boto3.resources.base import ResourceMeta
 except ImportError:
     from builtins import object as ResourceMeta
 
-
 __all__ = (
     "GlacierServiceResource",
     "Account",
     "Archive",
     "Job",
     "MultipartUpload",
     "Notification",
@@ -70,15 +69,14 @@
     "VaultJobsCollection",
     "VaultJobsInProgressCollection",
     "VaultMultipartUplaodsCollection",
     "VaultMultipartUploadsCollection",
     "VaultSucceededJobsCollection",
 )
 
-
 class ServiceResourceVaultsCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.vaults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#serviceresourcevaultscollection)
     """
 
     def all(self) -> "ServiceResourceVaultsCollection":
@@ -135,15 +133,14 @@
         """
         A generator which yields Vaults.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.vaults)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#serviceresourcevaultscollection)
         """
 
-
 class AccountVaultsCollection(AIOResourceCollection):
     def all(self) -> "AccountVaultsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -174,15 +171,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Vault"]:
         """
         A generator which yields Vaults.
         """
 
-
 class VaultCompletedJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultCompletedJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -213,15 +209,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
-
 class VaultFailedJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultFailedJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -252,15 +247,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
-
 class VaultJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -291,15 +285,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
-
 class VaultJobsInProgressCollection(AIOResourceCollection):
     def all(self) -> "VaultJobsInProgressCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -330,15 +323,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
-
 class VaultMultipartUplaodsCollection(AIOResourceCollection):
     def all(self) -> "VaultMultipartUplaodsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -369,15 +361,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
-
 class VaultMultipartUploadsCollection(AIOResourceCollection):
     def all(self) -> "VaultMultipartUploadsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -408,15 +399,14 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
-
 class VaultSucceededJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultSucceededJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -447,14 +437,49 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+class Account(AIOBoto3ServiceResource):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Account)
+    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#account)
+    """
+
+    id: str
+    vaults: AccountVaultsCollection
+    meta: Awaitable["GlacierResourceMeta"]
+
+    async def Vault(self, name: str) -> "_Vault":
+        """
+        Creates a Vault resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.Vault)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountvault-method)
+        """
+
+    async def create_vault(self, *, vaultName: str) -> "_Vault":
+        """
+        This operation creates a new vault with the specified name.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.create_vault)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountcreate_vault-method)
+        """
+
+    async def get_available_subresources(self) -> Sequence[str]:
+        """
+        Returns a list of all the available sub-resources for this Resource.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.get_available_subresources)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountget_available_subresources-method)
+        """
+
+_Account = Account
 
 class Job(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Job)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#job)
     """
 
@@ -478,14 +503,15 @@
     inventory_retrieval_parameters: Awaitable[InventoryRetrievalJobDescriptionResponseTypeDef]
     job_output_path: Awaitable[str]
     select_parameters: Awaitable[SelectParametersResponseTypeDef]
     output_location: Awaitable[OutputLocationResponseTypeDef]
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Job.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#jobvault-method)
@@ -523,32 +549,31 @@
         Job
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Job.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#jobreload-method)
         """
 
-
 _Job = Job
 
-
 class MultipartUpload(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.MultipartUpload)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartupload)
     """
 
     multipart_upload_id: Awaitable[str]
     vault_arn: Awaitable[str]
     archive_description: Awaitable[str]
     part_size_in_bytes: Awaitable[int]
     creation_date: Awaitable[str]
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartuploadvault-method)
@@ -599,28 +624,27 @@
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.upload_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartuploadupload_part-method)
         """
 
-
 _MultipartUpload = MultipartUpload
 
-
 class Notification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Notification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notification)
     """
 
     sns_topic: Awaitable[str]
     events: Awaitable[List[str]]
     account_id: str
     vault_name: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationvault-method)
@@ -670,64 +694,26 @@
         happen to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationset-method)
         """
 
-
 _Notification = Notification
 
-
-class Account(AIOBoto3ServiceResource):
-    """
-    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Account)
-    [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#account)
-    """
-
-    id: str
-    vaults: AccountVaultsCollection
-
-    async def Vault(self, name: str) -> "_Vault":
-        """
-        Creates a Vault resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.Vault)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountvault-method)
-        """
-
-    async def create_vault(self, *, vaultName: str) -> "_Vault":
-        """
-        This operation creates a new vault with the specified name.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.create_vault)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountcreate_vault-method)
-        """
-
-    async def get_available_subresources(self) -> Sequence[str]:
-        """
-        Returns a list of all the available sub-resources for this Resource.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.get_available_subresources)
-        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountget_available_subresources-method)
-        """
-
-
-_Account = Account
-
-
 class Archive(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Archive)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archive)
     """
 
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archivevault-method)
@@ -745,28 +731,26 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archiveget_available_subresources-method)
         """
 
-    async def initiate_archive_retrieval(self) -> _Job:
+    async def initiate_archive_retrieval(self) -> "_Job":
         """
         This operation initiates a job of the specified type, which can be a select, an
         archival retrieval, or a vault
         retrieval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.initiate_archive_retrieval)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archiveinitiate_archive_retrieval-method)
         """
 
-
 _Archive = Archive
 
-
 class Vault(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Vault)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vault)
     """
 
     vault_arn: Awaitable[str]
@@ -780,48 +764,49 @@
     completed_jobs: VaultCompletedJobsCollection
     failed_jobs: VaultFailedJobsCollection
     jobs: VaultJobsCollection
     jobs_in_progress: VaultJobsInProgressCollection
     multipart_uplaods: VaultMultipartUplaodsCollection
     multipart_uploads: VaultMultipartUploadsCollection
     succeeded_jobs: VaultSucceededJobsCollection
+    meta: Awaitable["GlacierResourceMeta"]
 
-    async def Account(self) -> _Account:
+    async def Account(self) -> "_Account":
         """
         Creates a Account resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultaccount-method)
         """
 
-    async def Archive(self, id: str) -> _Archive:
+    async def Archive(self, id: str) -> "_Archive":
         """
         Creates a Archive resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultarchive-method)
         """
 
-    async def Job(self, id: str) -> _Job:
+    async def Job(self, id: str) -> "_Job":
         """
         Creates a Job resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultjob-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultmultipartupload-method)
         """
 
-    async def Notification(self) -> _Notification:
+    async def Notification(self) -> "_Notification":
         """
         Creates a Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultnotification-method)
         """
 
@@ -845,27 +830,27 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultget_available_subresources-method)
         """
 
-    async def initiate_inventory_retrieval(self) -> _Job:
+    async def initiate_inventory_retrieval(self) -> "_Job":
         """
         This operation initiates a job of the specified type, which can be a select, an
         archival retrieval, or a vault
         retrieval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.initiate_inventory_retrieval)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultinitiate_inventory_retrieval-method)
         """
 
     async def initiate_multipart_upload(
         self, *, archiveDescription: str = ..., partSize: str = ...
-    ) -> _MultipartUpload:
+    ) -> "_MultipartUpload":
         """
         This operation initiates a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultinitiate_multipart_upload-method)
         """
 
@@ -887,88 +872,87 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultreload-method)
         """
 
     async def upload_archive(
         self, *, archiveDescription: str = ..., checksum: str = ..., body: BlobTypeDef = ...
-    ) -> _Archive:
+    ) -> "_Archive":
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.upload_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultupload_archive-method)
         """
 
-
 _Vault = Vault
 
-
 class GlacierResourceMeta(ResourceMeta):
     client: GlacierClient
 
-
 class GlacierServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/)
     """
 
     meta: "GlacierResourceMeta"
     vaults: ServiceResourceVaultsCollection
 
-    async def Account(self, id: str) -> _Account:
+    async def Account(self, id: str) -> "_Account":
         """
         Creates a Account resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourceaccount-method)
         """
 
-    async def Archive(self, account_id: str, vault_name: str, id: str) -> _Archive:
+    async def Archive(self, account_id: str, vault_name: str, id: str) -> "_Archive":
         """
         Creates a Archive resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcearchive-method)
         """
 
-    async def Job(self, account_id: str, vault_name: str, id: str) -> _Job:
+    async def Job(self, account_id: str, vault_name: str, id: str) -> "_Job":
         """
         Creates a Job resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcejob-method)
         """
 
-    async def MultipartUpload(self, account_id: str, vault_name: str, id: str) -> _MultipartUpload:
+    async def MultipartUpload(
+        self, account_id: str, vault_name: str, id: str
+    ) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcemultipartupload-method)
         """
 
-    async def Notification(self, account_id: str, vault_name: str) -> _Notification:
+    async def Notification(self, account_id: str, vault_name: str) -> "_Notification":
         """
         Creates a Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcenotification-method)
         """
 
-    async def Vault(self, account_id: str, name: str) -> _Vault:
+    async def Vault(self, account_id: str, name: str) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcevault-method)
         """
 
-    async def create_vault(self, *, vaultName: str, accountId: str = "-") -> _Vault:
+    async def create_vault(self, *, vaultName: str, accountId: str = "-") -> "_Vault":
         """
         This operation creates a new vault with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.create_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcecreate_vault-method)
         """
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/service_resource.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     "VaultJobsCollection",
     "VaultJobsInProgressCollection",
     "VaultMultipartUplaodsCollection",
     "VaultMultipartUploadsCollection",
     "VaultSucceededJobsCollection",
 )
 
+
 class ServiceResourceVaultsCollection(AIOResourceCollection):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.vaults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#serviceresourcevaultscollection)
     """
 
     def all(self) -> "ServiceResourceVaultsCollection":
@@ -133,14 +134,15 @@
         """
         A generator which yields Vaults.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.vaults)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#serviceresourcevaultscollection)
         """
 
+
 class AccountVaultsCollection(AIOResourceCollection):
     def all(self) -> "AccountVaultsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -171,14 +173,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Vault"]:
         """
         A generator which yields Vaults.
         """
 
+
 class VaultCompletedJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultCompletedJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -209,14 +212,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+
 class VaultFailedJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultFailedJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -247,14 +251,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+
 class VaultJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -285,14 +290,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+
 class VaultJobsInProgressCollection(AIOResourceCollection):
     def all(self) -> "VaultJobsInProgressCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -323,14 +329,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+
 class VaultMultipartUplaodsCollection(AIOResourceCollection):
     def all(self) -> "VaultMultipartUplaodsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -361,14 +368,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
+
 class VaultMultipartUploadsCollection(AIOResourceCollection):
     def all(self) -> "VaultMultipartUploadsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -399,14 +407,15 @@
         """
 
     def __aiter__(self) -> AsyncIterator["MultipartUpload"]:
         """
         A generator which yields MultipartUploads.
         """
 
+
 class VaultSucceededJobsCollection(AIOResourceCollection):
     def all(self) -> "VaultSucceededJobsCollection":
         """
         Get all items from the collection, optionally with a custom page size and item count limit.
         """
 
     def filter(  # type: ignore
@@ -437,32 +446,34 @@
         """
 
     def __aiter__(self) -> AsyncIterator["Job"]:
         """
         A generator which yields Jobs.
         """
 
+
 class Account(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Account)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#account)
     """
 
     id: str
     vaults: AccountVaultsCollection
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self, name: str) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountvault-method)
         """
 
-    async def create_vault(self, *, vaultName: str) -> _Vault:
+    async def create_vault(self, *, vaultName: str) -> "_Vault":
         """
         This operation creates a new vault with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.create_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountcreate_vault-method)
         """
 
@@ -470,16 +481,18 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Account.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#accountget_available_subresources-method)
         """
 
+
 _Account = Account
 
+
 class Job(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Job)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#job)
     """
 
     job_id: Awaitable[str]
@@ -502,14 +515,15 @@
     inventory_retrieval_parameters: Awaitable[InventoryRetrievalJobDescriptionResponseTypeDef]
     job_output_path: Awaitable[str]
     select_parameters: Awaitable[SelectParametersResponseTypeDef]
     output_location: Awaitable[OutputLocationResponseTypeDef]
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Job.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#jobvault-method)
@@ -547,30 +561,33 @@
         Job
         resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Job.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#jobreload-method)
         """
 
+
 _Job = Job
 
+
 class MultipartUpload(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.MultipartUpload)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartupload)
     """
 
     multipart_upload_id: Awaitable[str]
     vault_arn: Awaitable[str]
     archive_description: Awaitable[str]
     part_size_in_bytes: Awaitable[int]
     creation_date: Awaitable[str]
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartuploadvault-method)
@@ -621,26 +638,29 @@
         """
         This operation uploads a part of an archive.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.MultipartUpload.upload_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#multipartuploadupload_part-method)
         """
 
+
 _MultipartUpload = MultipartUpload
 
+
 class Notification(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Notification)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notification)
     """
 
     sns_topic: Awaitable[str]
     events: Awaitable[List[str]]
     account_id: str
     vault_name: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationvault-method)
@@ -690,25 +710,28 @@
         happen to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationset-method)
         """
 
+
 _Notification = Notification
 
+
 class Archive(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Archive)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archive)
     """
 
     account_id: str
     vault_name: str
     id: str
+    meta: Awaitable["GlacierResourceMeta"]
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archivevault-method)
@@ -726,26 +749,28 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archiveget_available_subresources-method)
         """
 
-    async def initiate_archive_retrieval(self) -> _Job:
+    async def initiate_archive_retrieval(self) -> "_Job":
         """
         This operation initiates a job of the specified type, which can be a select, an
         archival retrieval, or a vault
         retrieval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Archive.initiate_archive_retrieval)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#archiveinitiate_archive_retrieval-method)
         """
 
+
 _Archive = Archive
 
+
 class Vault(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Vault)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vault)
     """
 
     vault_arn: Awaitable[str]
@@ -759,48 +784,49 @@
     completed_jobs: VaultCompletedJobsCollection
     failed_jobs: VaultFailedJobsCollection
     jobs: VaultJobsCollection
     jobs_in_progress: VaultJobsInProgressCollection
     multipart_uplaods: VaultMultipartUplaodsCollection
     multipart_uploads: VaultMultipartUploadsCollection
     succeeded_jobs: VaultSucceededJobsCollection
+    meta: Awaitable["GlacierResourceMeta"]
 
-    async def Account(self) -> _Account:
+    async def Account(self) -> "_Account":
         """
         Creates a Account resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultaccount-method)
         """
 
-    async def Archive(self, id: str) -> _Archive:
+    async def Archive(self, id: str) -> "_Archive":
         """
         Creates a Archive resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultarchive-method)
         """
 
-    async def Job(self, id: str) -> _Job:
+    async def Job(self, id: str) -> "_Job":
         """
         Creates a Job resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultjob-method)
         """
 
-    async def MultipartUpload(self, id: str) -> _MultipartUpload:
+    async def MultipartUpload(self, id: str) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultmultipartupload-method)
         """
 
-    async def Notification(self) -> _Notification:
+    async def Notification(self) -> "_Notification":
         """
         Creates a Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultnotification-method)
         """
 
@@ -824,27 +850,27 @@
         """
         Returns a list of all the available sub-resources for this Resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultget_available_subresources-method)
         """
 
-    async def initiate_inventory_retrieval(self) -> _Job:
+    async def initiate_inventory_retrieval(self) -> "_Job":
         """
         This operation initiates a job of the specified type, which can be a select, an
         archival retrieval, or a vault
         retrieval.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.initiate_inventory_retrieval)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultinitiate_inventory_retrieval-method)
         """
 
     async def initiate_multipart_upload(
         self, *, archiveDescription: str = ..., partSize: str = ...
-    ) -> _MultipartUpload:
+    ) -> "_MultipartUpload":
         """
         This operation initiates a multipart upload.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.initiate_multipart_upload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultinitiate_multipart_upload-method)
         """
 
@@ -866,85 +892,90 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultreload-method)
         """
 
     async def upload_archive(
         self, *, archiveDescription: str = ..., checksum: str = ..., body: BlobTypeDef = ...
-    ) -> _Archive:
+    ) -> "_Archive":
         """
         This operation adds an archive to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Vault.upload_archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#vaultupload_archive-method)
         """
 
+
 _Vault = Vault
 
+
 class GlacierResourceMeta(ResourceMeta):
     client: GlacierClient
 
+
 class GlacierServiceResource(AIOBoto3ServiceResource):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/)
     """
 
     meta: "GlacierResourceMeta"
     vaults: ServiceResourceVaultsCollection
 
-    async def Account(self, id: str) -> _Account:
+    async def Account(self, id: str) -> "_Account":
         """
         Creates a Account resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourceaccount-method)
         """
 
-    async def Archive(self, account_id: str, vault_name: str, id: str) -> _Archive:
+    async def Archive(self, account_id: str, vault_name: str, id: str) -> "_Archive":
         """
         Creates a Archive resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Archive)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcearchive-method)
         """
 
-    async def Job(self, account_id: str, vault_name: str, id: str) -> _Job:
+    async def Job(self, account_id: str, vault_name: str, id: str) -> "_Job":
         """
         Creates a Job resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcejob-method)
         """
 
-    async def MultipartUpload(self, account_id: str, vault_name: str, id: str) -> _MultipartUpload:
+    async def MultipartUpload(
+        self, account_id: str, vault_name: str, id: str
+    ) -> "_MultipartUpload":
         """
         Creates a MultipartUpload resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.MultipartUpload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcemultipartupload-method)
         """
 
-    async def Notification(self, account_id: str, vault_name: str) -> _Notification:
+    async def Notification(self, account_id: str, vault_name: str) -> "_Notification":
         """
         Creates a Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Notification)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcenotification-method)
         """
 
-    async def Vault(self, account_id: str, name: str) -> _Vault:
+    async def Vault(self, account_id: str, name: str) -> "_Vault":
         """
         Creates a Vault resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.Vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcevault-method)
         """
 
-    async def create_vault(self, *, vaultName: str, accountId: str = "-") -> _Vault:
+    async def create_vault(self, *, vaultName: str, accountId: str = "-") -> "_Vault":
         """
         This operation creates a new vault with the specified name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.ServiceResource.create_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#glacierserviceresourcecreate_vault-method)
         """
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/type_defs.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AbortMultipartUploadInputRequestTypeDef",
     "AbortVaultLockInputRequestTypeDef",
     "AddTagsToVaultInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BlobTypeDef",
     "CSVInputTypeDef",
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/type_defs.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/waiter.py` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier/waiter.pyi` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/PKG-INFO` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-glacier
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Glacier 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Glacier 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/
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
 
 <a id="types-aiobotocore-glacier"></a>
 
 # types-aiobotocore-glacier
 
 [![PyPI - types-aiobotocore-glacier](https://img.shields.io/pypi/v/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-glacier.svg?color=blue)](https://pypi.org/project/types-aiobotocore-glacier)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-glacier)](https://pepy.tech/project/types-aiobotocore-glacier)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Glacier 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
+[aiobotocore.Glacier 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
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
 [types-aiobotocore-glacier docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-glacier-2.9.0/types_aiobotocore_glacier.egg-info/SOURCES.txt` & `types-aiobotocore-glacier-2.9.1/types_aiobotocore_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

