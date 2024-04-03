# Comparing `tmp/types-aiobotocore-cloudcontrol-2.9.0.tar.gz` & `tmp/types-aiobotocore-cloudcontrol-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudcontrol-2.9.0.tar", last modified: Wed Dec 13 19:58:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudcontrol-2.9.1.tar", last modified: Thu Jan 18 01:20:14 2024, max compression
```

## Comparing `types-aiobotocore-cloudcontrol-2.9.0.tar` & `types-aiobotocore-cloudcontrol-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.081984 types-aiobotocore-cloudcontrol-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14250 2023-12-13 19:58:48.081984 types-aiobotocore-cloudcontrol-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12664 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:48.081984 types-aiobotocore-cloudcontrol-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.081984 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12081 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9803 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-12-13 19:42:14.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:48.081984 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14250 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:58:48.000000 types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.961468 types-aiobotocore-cloudcontrol-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-01-18 01:20:14.961468 types-aiobotocore-cloudcontrol-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12664 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:14.961468 types-aiobotocore-cloudcontrol-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.957468 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12086 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9803 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-01-18 01:04:10.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:14.961468 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14270 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:14.000000 types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/LICENSE` & `types-aiobotocore-cloudcontrol-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudControlApi 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudControlApi 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
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
 
 <a id="types-aiobotocore-cloudcontrol"></a>
 
 # types-aiobotocore-cloudcontrol
 
 [![PyPI - types-aiobotocore-cloudcontrol](https://img.shields.io/pypi/v/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/README.md` & `types-aiobotocore-cloudcontrol-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/setup.py` & `types-aiobotocore-cloudcontrol-2.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudcontrol",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CloudControlApi 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CloudControlApi 2.9.1 service generated with"
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
     keywords="aiobotocore cloudcontrol type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudcontrol": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__init__.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 
 from .client import CloudControlApiClient
 from .paginator import ListResourceRequestsPaginator, ListResourcesPaginator
 from .waiter import ResourceRequestSuccessWaiter
 
 Client = CloudControlApiClient
 
-
 __all__ = (
     "Client",
     "CloudControlApiClient",
     "ListResourceRequestsPaginator",
     "ListResourcesPaginator",
     "ResourceRequestSuccessWaiter",
 )
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__init__.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/__main__.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudControlApi 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CloudControlApi 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/client.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from .waiter import ResourceRequestSuccessWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CloudControlApiClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -123,15 +122,15 @@
     async def create_resource(
         self,
         *,
         TypeName: str,
         DesiredState: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateResourceOutputTypeDef:
         """
         Creates the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.create_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#create_resource)
         """
@@ -139,15 +138,15 @@
     async def delete_resource(
         self,
         *,
         TypeName: str,
         Identifier: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> DeleteResourceOutputTypeDef:
         """
         Deletes the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.delete_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#delete_resource)
         """
@@ -187,15 +186,15 @@
         """
 
     async def list_resource_requests(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...
+        ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
     ) -> ListResourceRequestsOutputTypeDef:
         """
         Returns existing resource operation requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resource_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#list_resource_requests)
         """
@@ -204,15 +203,15 @@
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceModel: str = ...
+        ResourceModel: str = ...,
     ) -> ListResourcesOutputTypeDef:
         """
         Returns information about the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#list_resources)
         """
@@ -221,15 +220,15 @@
         self,
         *,
         TypeName: str,
         Identifier: str,
         PatchDocument: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdateResourceOutputTypeDef:
         """
         Updates the specified property values in the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#update_resource)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/client.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     async def create_resource(
         self,
         *,
         TypeName: str,
         DesiredState: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> CreateResourceOutputTypeDef:
         """
         Creates the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.create_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#create_resource)
         """
@@ -135,15 +135,15 @@
     async def delete_resource(
         self,
         *,
         TypeName: str,
         Identifier: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> DeleteResourceOutputTypeDef:
         """
         Deletes the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.delete_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#delete_resource)
         """
@@ -183,15 +183,15 @@
         """
 
     async def list_resource_requests(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
-        ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...
+        ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
     ) -> ListResourceRequestsOutputTypeDef:
         """
         Returns existing resource operation requests.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resource_requests)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#list_resource_requests)
         """
@@ -200,15 +200,15 @@
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ResourceModel: str = ...
+        ResourceModel: str = ...,
     ) -> ListResourcesOutputTypeDef:
         """
         Returns information about the specified resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.list_resources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#list_resources)
         """
@@ -217,15 +217,15 @@
         self,
         *,
         TypeName: str,
         Identifier: str,
         PatchDocument: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
-        ClientToken: str = ...
+        ClientToken: str = ...,
     ) -> UpdateResourceOutputTypeDef:
         """
         Updates the specified property values in the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Client.update_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/client/#update_resource)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/literals.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/literals.py`

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
     "HandlerErrorCodeType",
     "ListResourceRequestsPaginatorName",
     "ListResourcesPaginatorName",
     "OperationStatusType",
     "OperationType",
     "ResourceRequestSuccessWaiterName",
@@ -31,15 +30,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 HandlerErrorCodeType = Literal[
     "AccessDenied",
     "AlreadyExists",
     "GeneralServiceException",
     "InternalFailure",
     "InvalidCredentials",
     "InvalidRequest",
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/literals.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/paginator.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListResourcesOutputTypeDef,
     PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
 )
 
 __all__ = ("ListResourceRequestsPaginator", "ListResourcesPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -54,15 +53,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 
@@ -75,13 +74,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/paginator.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 class ListResourcesPaginator(AioPaginator):
@@ -71,13 +71,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/type_defs.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/type_defs.py`

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
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
     "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/type_defs.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/waiter.py` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol/waiter.pyi` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CloudControlApi 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CloudControlApi 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
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
 
 <a id="types-aiobotocore-cloudcontrol"></a>
 
 # types-aiobotocore-cloudcontrol
 
 [![PyPI - types-aiobotocore-cloudcontrol](https://img.shields.io/pypi/v/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CloudControlApi 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[aiobotocore.CloudControlApi 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cloudcontrol-2.9.0/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt` & `types-aiobotocore-cloudcontrol-2.9.1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

