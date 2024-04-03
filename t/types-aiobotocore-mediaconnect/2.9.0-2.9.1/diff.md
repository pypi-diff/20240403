# Comparing `tmp/types-aiobotocore-mediaconnect-2.9.0.tar.gz` & `tmp/types-aiobotocore-mediaconnect-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconnect-2.9.0.tar", last modified: Wed Dec 13 19:59:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconnect-2.9.1.tar", last modified: Thu Jan 18 01:21:14 2024, max compression
```

## Comparing `types-aiobotocore-mediaconnect-2.9.0.tar` & `types-aiobotocore-mediaconnect-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.301470 types-aiobotocore-mediaconnect-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-13 19:59:52.301470 types-aiobotocore-mediaconnect-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13375 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:52.301470 types-aiobotocore-mediaconnect-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.301470 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42824 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42820 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12447 2023-12-13 19:49:50.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12445 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8626 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    55444 2023-12-13 19:49:51.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55443 2023-12-13 19:49:50.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:47.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2023-12-13 19:49:48.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:52.301470 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14958 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:52.000000 types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.281190 types-aiobotocore-mediaconnect-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-01-18 01:21:14.281190 types-aiobotocore-mediaconnect-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13375 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:14.281190 types-aiobotocore-mediaconnect-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.281190 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42834 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42831 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12445 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8625 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    55443 2024-01-18 01:11:34.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55443 2024-01-18 01:11:34.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:32.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-01-18 01:11:33.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:14.281190 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14978 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:21:14.000000 types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/LICENSE` & `types-aiobotocore-mediaconnect-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-mediaconnect-2.9.0/PKG-INFO` & `types-aiobotocore-mediaconnect-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/
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
 
 <a id="types-aiobotocore-mediaconnect"></a>
 
 # types-aiobotocore-mediaconnect
 
 [![PyPI - types-aiobotocore-mediaconnect](https://img.shields.io/pypi/v/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [types-aiobotocore-mediaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/README.md` & `types-aiobotocore-mediaconnect-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [types-aiobotocore-mediaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/setup.py` & `types-aiobotocore-mediaconnect-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconnect",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_mediaconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MediaConnect 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MediaConnect 2.9.1 service generated with"
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
     keywords="aiobotocore mediaconnect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_mediaconnect": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__init__.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     ListOfferingsPaginator,
     ListReservationsPaginator,
 )
 from .waiter import FlowActiveWaiter, FlowDeletedWaiter, FlowStandbyWaiter
 
 Client = MediaConnectClient
 
-
 __all__ = (
     "Client",
     "FlowActiveWaiter",
     "FlowDeletedWaiter",
     "FlowStandbyWaiter",
     "ListBridgesPaginator",
     "ListEntitlementsPaginator",
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__init__.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/__main__.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConnect 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MediaConnect 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect\nOther"
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

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/client.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
 from .waiter import FlowActiveWaiter, FlowDeletedWaiter, FlowStandbyWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MediaConnectClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -248,15 +247,15 @@
         *,
         Name: str,
         PlacementArn: str,
         Sources: Sequence[AddBridgeSourceRequestTypeDef],
         EgressGatewayBridge: AddEgressGatewayBridgeRequestTypeDef = ...,
         IngressGatewayBridge: AddIngressGatewayBridgeRequestTypeDef = ...,
         Outputs: Sequence[AddBridgeOutputRequestTypeDef] = ...,
-        SourceFailoverConfig: FailoverConfigTypeDef = ...
+        SourceFailoverConfig: FailoverConfigTypeDef = ...,
     ) -> CreateBridgeResponseTypeDef:
         """
         Creates a new bridge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_bridge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_bridge)
         """
@@ -269,29 +268,29 @@
         Entitlements: Sequence[GrantEntitlementRequestTypeDef] = ...,
         MediaStreams: Sequence[AddMediaStreamRequestTypeDef] = ...,
         Outputs: Sequence[AddOutputRequestTypeDef] = ...,
         Source: SetSourceRequestTypeDef = ...,
         SourceFailoverConfig: FailoverConfigTypeDef = ...,
         Sources: Sequence[SetSourceRequestTypeDef] = ...,
         VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef] = ...,
-        Maintenance: AddMaintenanceTypeDef = ...
+        Maintenance: AddMaintenanceTypeDef = ...,
     ) -> CreateFlowResponseTypeDef:
         """
         Creates a new flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_flow)
         """
 
     async def create_gateway(
         self,
         *,
         EgressCidrBlocks: Sequence[str],
         Name: str,
-        Networks: Sequence[GatewayNetworkTypeDef]
+        Networks: Sequence[GatewayNetworkTypeDef],
     ) -> CreateGatewayResponseTypeDef:
         """
         Creates a new gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_gateway)
         """
@@ -611,45 +610,45 @@
 
     async def update_bridge(
         self,
         *,
         BridgeArn: str,
         EgressGatewayBridge: UpdateEgressGatewayBridgeRequestTypeDef = ...,
         IngressGatewayBridge: UpdateIngressGatewayBridgeRequestTypeDef = ...,
-        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...
+        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
     ) -> UpdateBridgeResponseTypeDef:
         """
         Updates the bridge See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridge).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge)
         """
 
     async def update_bridge_output(
         self,
         *,
         BridgeArn: str,
         OutputName: str,
-        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...
+        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...,
     ) -> UpdateBridgeOutputResponseTypeDef:
         """
         Updates an existing bridge output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_output)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge_output)
         """
 
     async def update_bridge_source(
         self,
         *,
         BridgeArn: str,
         SourceName: str,
         FlowSource: UpdateBridgeFlowSourceRequestTypeDef = ...,
-        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...
+        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...,
     ) -> UpdateBridgeSourceResponseTypeDef:
         """
         Updates an existing bridge source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge_source)
         """
@@ -666,15 +665,15 @@
         """
 
     async def update_flow(
         self,
         *,
         FlowArn: str,
         SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
-        Maintenance: UpdateMaintenanceTypeDef = ...
+        Maintenance: UpdateMaintenanceTypeDef = ...,
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates flow See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateFlow).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow)
@@ -684,15 +683,15 @@
         self,
         *,
         EntitlementArn: str,
         FlowArn: str,
         Description: str = ...,
         Encryption: UpdateEncryptionTypeDef = ...,
         EntitlementStatus: EntitlementStatusType = ...,
-        Subscribers: Sequence[str] = ...
+        Subscribers: Sequence[str] = ...,
     ) -> UpdateFlowEntitlementResponseTypeDef:
         """
         You can change an entitlement's description, subscribers, and encryption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_entitlement)
         """
@@ -702,15 +701,15 @@
         *,
         FlowArn: str,
         MediaStreamName: str,
         Attributes: MediaStreamAttributesRequestTypeDef = ...,
         ClockRate: int = ...,
         Description: str = ...,
         MediaStreamType: MediaStreamTypeType = ...,
-        VideoFormat: str = ...
+        VideoFormat: str = ...,
     ) -> UpdateFlowMediaStreamResponseTypeDef:
         """
         Updates an existing media stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_media_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_media_stream)
         """
@@ -732,15 +731,15 @@
         Port: int = ...,
         Protocol: ProtocolType = ...,
         RemoteId: str = ...,
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SmoothingLatency: int = ...,
         StreamId: str = ...,
-        VpcInterfaceAttachment: VpcInterfaceAttachmentTypeDef = ...
+        VpcInterfaceAttachment: VpcInterfaceAttachmentTypeDef = ...,
     ) -> UpdateFlowOutputResponseTypeDef:
         """
         Updates an existing flow output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_output)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_output)
         """
@@ -765,15 +764,15 @@
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SourceListenerAddress: str = ...,
         SourceListenerPort: int = ...,
         StreamId: str = ...,
         VpcInterfaceName: str = ...,
         WhitelistCidr: str = ...,
-        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...
+        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...,
     ) -> UpdateFlowSourceResponseTypeDef:
         """
         Updates the source of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_source)
         """
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/client.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -244,15 +244,15 @@
         *,
         Name: str,
         PlacementArn: str,
         Sources: Sequence[AddBridgeSourceRequestTypeDef],
         EgressGatewayBridge: AddEgressGatewayBridgeRequestTypeDef = ...,
         IngressGatewayBridge: AddIngressGatewayBridgeRequestTypeDef = ...,
         Outputs: Sequence[AddBridgeOutputRequestTypeDef] = ...,
-        SourceFailoverConfig: FailoverConfigTypeDef = ...
+        SourceFailoverConfig: FailoverConfigTypeDef = ...,
     ) -> CreateBridgeResponseTypeDef:
         """
         Creates a new bridge.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_bridge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_bridge)
         """
@@ -265,29 +265,29 @@
         Entitlements: Sequence[GrantEntitlementRequestTypeDef] = ...,
         MediaStreams: Sequence[AddMediaStreamRequestTypeDef] = ...,
         Outputs: Sequence[AddOutputRequestTypeDef] = ...,
         Source: SetSourceRequestTypeDef = ...,
         SourceFailoverConfig: FailoverConfigTypeDef = ...,
         Sources: Sequence[SetSourceRequestTypeDef] = ...,
         VpcInterfaces: Sequence[VpcInterfaceRequestTypeDef] = ...,
-        Maintenance: AddMaintenanceTypeDef = ...
+        Maintenance: AddMaintenanceTypeDef = ...,
     ) -> CreateFlowResponseTypeDef:
         """
         Creates a new flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_flow)
         """
 
     async def create_gateway(
         self,
         *,
         EgressCidrBlocks: Sequence[str],
         Name: str,
-        Networks: Sequence[GatewayNetworkTypeDef]
+        Networks: Sequence[GatewayNetworkTypeDef],
     ) -> CreateGatewayResponseTypeDef:
         """
         Creates a new gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.create_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#create_gateway)
         """
@@ -607,45 +607,45 @@
 
     async def update_bridge(
         self,
         *,
         BridgeArn: str,
         EgressGatewayBridge: UpdateEgressGatewayBridgeRequestTypeDef = ...,
         IngressGatewayBridge: UpdateIngressGatewayBridgeRequestTypeDef = ...,
-        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...
+        SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
     ) -> UpdateBridgeResponseTypeDef:
         """
         Updates the bridge See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateBridge).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge)
         """
 
     async def update_bridge_output(
         self,
         *,
         BridgeArn: str,
         OutputName: str,
-        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...
+        NetworkOutput: UpdateBridgeNetworkOutputRequestTypeDef = ...,
     ) -> UpdateBridgeOutputResponseTypeDef:
         """
         Updates an existing bridge output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_output)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge_output)
         """
 
     async def update_bridge_source(
         self,
         *,
         BridgeArn: str,
         SourceName: str,
         FlowSource: UpdateBridgeFlowSourceRequestTypeDef = ...,
-        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...
+        NetworkSource: UpdateBridgeNetworkSourceRequestTypeDef = ...,
     ) -> UpdateBridgeSourceResponseTypeDef:
         """
         Updates an existing bridge source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_bridge_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_bridge_source)
         """
@@ -662,15 +662,15 @@
         """
 
     async def update_flow(
         self,
         *,
         FlowArn: str,
         SourceFailoverConfig: UpdateFailoverConfigTypeDef = ...,
-        Maintenance: UpdateMaintenanceTypeDef = ...
+        Maintenance: UpdateMaintenanceTypeDef = ...,
     ) -> UpdateFlowResponseTypeDef:
         """
         Updates flow See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/mediaconnect-2018-11-14/UpdateFlow).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow)
@@ -680,15 +680,15 @@
         self,
         *,
         EntitlementArn: str,
         FlowArn: str,
         Description: str = ...,
         Encryption: UpdateEncryptionTypeDef = ...,
         EntitlementStatus: EntitlementStatusType = ...,
-        Subscribers: Sequence[str] = ...
+        Subscribers: Sequence[str] = ...,
     ) -> UpdateFlowEntitlementResponseTypeDef:
         """
         You can change an entitlement's description, subscribers, and encryption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_entitlement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_entitlement)
         """
@@ -698,15 +698,15 @@
         *,
         FlowArn: str,
         MediaStreamName: str,
         Attributes: MediaStreamAttributesRequestTypeDef = ...,
         ClockRate: int = ...,
         Description: str = ...,
         MediaStreamType: MediaStreamTypeType = ...,
-        VideoFormat: str = ...
+        VideoFormat: str = ...,
     ) -> UpdateFlowMediaStreamResponseTypeDef:
         """
         Updates an existing media stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_media_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_media_stream)
         """
@@ -728,15 +728,15 @@
         Port: int = ...,
         Protocol: ProtocolType = ...,
         RemoteId: str = ...,
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SmoothingLatency: int = ...,
         StreamId: str = ...,
-        VpcInterfaceAttachment: VpcInterfaceAttachmentTypeDef = ...
+        VpcInterfaceAttachment: VpcInterfaceAttachmentTypeDef = ...,
     ) -> UpdateFlowOutputResponseTypeDef:
         """
         Updates an existing flow output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_output)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_output)
         """
@@ -761,15 +761,15 @@
         SenderControlPort: int = ...,
         SenderIpAddress: str = ...,
         SourceListenerAddress: str = ...,
         SourceListenerPort: int = ...,
         StreamId: str = ...,
         VpcInterfaceName: str = ...,
         WhitelistCidr: str = ...,
-        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...
+        GatewayBridgeSource: UpdateGatewayBridgeSourceRequestTypeDef = ...,
     ) -> UpdateFlowSourceResponseTypeDef:
         """
         Updates the source of a flow.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect.Client.update_flow_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/client/#update_flow_source)
         """
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/literals.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/literals.py`

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
     "AlgorithmType",
     "BridgePlacementType",
     "BridgeStateType",
     "ColorimetryType",
     "ConnectionStatusType",
     "DesiredStateType",
@@ -62,15 +61,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlgorithmType = Literal["aes128", "aes192", "aes256"]
 BridgePlacementType = Literal["AVAILABLE", "LOCKED"]
 BridgeStateType = Literal[
     "ACTIVE",
     "CREATING",
     "DELETED",
     "DELETING",
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/literals.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/paginator.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     "ListFlowsPaginator",
     "ListGatewayInstancesPaginator",
     "ListGatewaysPaginator",
     "ListOfferingsPaginator",
     "ListReservationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/paginator.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/type_defs.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "VpcInterfaceAttachmentTypeDef",
     "AddBridgeNetworkOutputRequestTypeDef",
     "AddBridgeNetworkSourceRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AddEgressGatewayBridgeRequestTypeDef",
     "VpcInterfaceRequestTypeDef",
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/type_defs.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/waiter.py` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect/waiter.pyi` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/PKG-INFO` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-mediaconnect
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MediaConnect 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MediaConnect 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/
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
 
 <a id="types-aiobotocore-mediaconnect"></a>
 
 # types-aiobotocore-mediaconnect
 
 [![PyPI - types-aiobotocore-mediaconnect](https://img.shields.io/pypi/v/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-mediaconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-mediaconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-mediaconnect)](https://pepy.tech/project/types-aiobotocore-mediaconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MediaConnect 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
+[aiobotocore.MediaConnect 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#MediaConnect)
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
 [types-aiobotocore-mediaconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconnect/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-mediaconnect-2.9.0/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconnect-2.9.1/types_aiobotocore_mediaconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

