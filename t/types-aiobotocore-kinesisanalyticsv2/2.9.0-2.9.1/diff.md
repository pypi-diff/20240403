# Comparing `tmp/types-aiobotocore-kinesisanalyticsv2-2.9.0.tar.gz` & `tmp/types-aiobotocore-kinesisanalyticsv2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.9.0.tar", last modified: Wed Dec 13 19:59:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalyticsv2-2.9.1.tar", last modified: Thu Jan 18 01:21:04 2024, max compression
```

## Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0.tar` & `types-aiobotocore-kinesisanalyticsv2-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.461560 types-aiobotocore-kinesisanalyticsv2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13822 2023-12-13 19:59:41.461560 types-aiobotocore-kinesisanalyticsv2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12215 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:41.461560 types-aiobotocore-kinesisanalyticsv2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2023-12-13 19:48:37.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.457560 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      976 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29397 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    29393 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10596 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10594 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56255 2023-12-13 19:48:39.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    56254 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:48:38.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:41.461560 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13822 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-12-13 19:59:41.000000 types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.205235 types-aiobotocore-kinesisanalyticsv2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-01-18 01:21:04.205235 types-aiobotocore-kinesisanalyticsv2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12215 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:04.205235 types-aiobotocore-kinesisanalyticsv2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.205235 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29408 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29405 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-01-18 01:10:25.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10594 2024-01-18 01:10:25.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    56254 2024-01-18 01:10:25.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56254 2024-01-18 01:10:25.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:10:24.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:04.205235 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-01-18 01:21:04.000000 types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/LICENSE` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
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
 
 <a id="types-aiobotocore-kinesisanalyticsv2"></a>
 
 # types-aiobotocore-kinesisanalyticsv2
 
 [![PyPI - types-aiobotocore-kinesisanalyticsv2](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/README.md` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/setup.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalyticsv2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_kinesisanalyticsv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.1 service generated with"
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
     keywords="aiobotocore kinesisanalyticsv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisanalyticsv2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__init__.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,13 @@
 """
 
 from .client import KinesisAnalyticsV2Client
 from .paginator import ListApplicationSnapshotsPaginator, ListApplicationsPaginator
 
 Client = KinesisAnalyticsV2Client
 
-
 __all__ = (
     "Client",
     "KinesisAnalyticsV2Client",
     "ListApplicationSnapshotsPaginator",
     "ListApplicationsPaginator",
 )
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__init__.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/__main__.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2\nOther"
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

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/client.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KinesisAnalyticsV2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -119,15 +118,15 @@
 
     async def add_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> AddApplicationCloudWatchLoggingOptionResponseTypeDef:
         """
         Adds an Amazon CloudWatch log stream to monitor application configuration
         errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_cloud_watch_logging_option)
@@ -145,15 +144,15 @@
 
     async def add_application_input_processing_configuration(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
         InputId: str,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef,
     ) -> AddApplicationInputProcessingConfigurationResponseTypeDef:
         """
         Adds an  InputProcessingConfiguration to a SQL-based Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_input_processing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_input_processing_configuration)
@@ -171,15 +170,15 @@
         """
 
     async def add_application_reference_data_source(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ReferenceDataSource: ReferenceDataSourceTypeDef
+        ReferenceDataSource: ReferenceDataSourceTypeDef,
     ) -> AddApplicationReferenceDataSourceResponseTypeDef:
         """
         Adds a reference data source to an existing SQL-based Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_reference_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_reference_data_source)
@@ -187,15 +186,15 @@
 
     async def add_application_vpc_configuration(
         self,
         *,
         ApplicationName: str,
         VpcConfiguration: VpcConfigurationTypeDef,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> AddApplicationVpcConfigurationResponseTypeDef:
         """
         Adds a Virtual Private Cloud (VPC) configuration to the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_vpc_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_vpc_configuration)
         """
@@ -222,29 +221,29 @@
         ApplicationName: str,
         RuntimeEnvironment: RuntimeEnvironmentType,
         ServiceExecutionRole: str,
         ApplicationDescription: str = ...,
         ApplicationConfiguration: ApplicationConfigurationTypeDef = ...,
         CloudWatchLoggingOptions: Sequence[CloudWatchLoggingOptionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ApplicationMode: ApplicationModeType = ...
+        ApplicationMode: ApplicationModeType = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application)
         """
 
     async def create_application_presigned_url(
         self,
         *,
         ApplicationName: str,
         UrlType: UrlTypeType,
-        SessionExpirationDurationInSeconds: int = ...
+        SessionExpirationDurationInSeconds: int = ...,
     ) -> CreateApplicationPresignedUrlResponseTypeDef:
         """
         Creates and returns a URL that you can use to connect to an application's
         extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application_presigned_url)
@@ -272,15 +271,15 @@
 
     async def delete_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CloudWatchLoggingOptionId: str,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> DeleteApplicationCloudWatchLoggingOptionResponseTypeDef:
         """
         Deletes an Amazon CloudWatch log stream from an Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_cloud_watch_logging_option)
@@ -321,30 +320,30 @@
         """
 
     async def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: TimestampTypeDef
+        SnapshotCreationTimestamp: TimestampTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
 
     async def delete_application_vpc_configuration(
         self,
         *,
         ApplicationName: str,
         VpcConfigurationId: str,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> DeleteApplicationVpcConfigurationResponseTypeDef:
         """
         Removes a VPC configuration from a Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_vpc_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_vpc_configuration)
         """
@@ -382,15 +381,15 @@
     async def discover_input_schema(
         self,
         *,
         ServiceExecutionRole: str,
         ResourceARN: str = ...,
         InputStartingPositionConfiguration: InputStartingPositionConfigurationTypeDef = ...,
         S3Configuration: S3ConfigurationTypeDef = ...,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...,
     ) -> DiscoverInputSchemaResponseTypeDef:
         """
         Infers a schema for a SQL-based Kinesis Data Analytics application by
         evaluating sample records on the specified streaming source (Kinesis data
         stream or Kinesis Data Firehose delivery stream) or Amazon S3
         object.
 
@@ -503,28 +502,28 @@
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int = ...,
         ApplicationConfigurationUpdate: ApplicationConfigurationUpdateTypeDef = ...,
         ServiceExecutionRoleUpdate: str = ...,
         RunConfigurationUpdate: RunConfigurationUpdateTypeDef = ...,
         CloudWatchLoggingOptionUpdates: Sequence[CloudWatchLoggingOptionUpdateTypeDef] = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an existing Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#update_application)
         """
 
     async def update_application_maintenance_configuration(
         self,
         *,
         ApplicationName: str,
-        ApplicationMaintenanceConfigurationUpdate: ApplicationMaintenanceConfigurationUpdateTypeDef
+        ApplicationMaintenanceConfigurationUpdate: ApplicationMaintenanceConfigurationUpdateTypeDef,
     ) -> UpdateApplicationMaintenanceConfigurationResponseTypeDef:
         """
         Updates the maintenance configuration of the Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.update_application_maintenance_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#update_application_maintenance_configuration)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/client.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 
     async def add_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CloudWatchLoggingOption: CloudWatchLoggingOptionTypeDef,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> AddApplicationCloudWatchLoggingOptionResponseTypeDef:
         """
         Adds an Amazon CloudWatch log stream to monitor application configuration
         errors.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_cloud_watch_logging_option)
@@ -141,15 +141,15 @@
 
     async def add_application_input_processing_configuration(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
         InputId: str,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef,
     ) -> AddApplicationInputProcessingConfigurationResponseTypeDef:
         """
         Adds an  InputProcessingConfiguration to a SQL-based Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_input_processing_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_input_processing_configuration)
@@ -167,15 +167,15 @@
         """
 
     async def add_application_reference_data_source(
         self,
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int,
-        ReferenceDataSource: ReferenceDataSourceTypeDef
+        ReferenceDataSource: ReferenceDataSourceTypeDef,
     ) -> AddApplicationReferenceDataSourceResponseTypeDef:
         """
         Adds a reference data source to an existing SQL-based Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_reference_data_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_reference_data_source)
@@ -183,15 +183,15 @@
 
     async def add_application_vpc_configuration(
         self,
         *,
         ApplicationName: str,
         VpcConfiguration: VpcConfigurationTypeDef,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> AddApplicationVpcConfigurationResponseTypeDef:
         """
         Adds a Virtual Private Cloud (VPC) configuration to the application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.add_application_vpc_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#add_application_vpc_configuration)
         """
@@ -218,29 +218,29 @@
         ApplicationName: str,
         RuntimeEnvironment: RuntimeEnvironmentType,
         ServiceExecutionRole: str,
         ApplicationDescription: str = ...,
         ApplicationConfiguration: ApplicationConfigurationTypeDef = ...,
         CloudWatchLoggingOptions: Sequence[CloudWatchLoggingOptionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ApplicationMode: ApplicationModeType = ...
+        ApplicationMode: ApplicationModeType = ...,
     ) -> CreateApplicationResponseTypeDef:
         """
         Creates a Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application)
         """
 
     async def create_application_presigned_url(
         self,
         *,
         ApplicationName: str,
         UrlType: UrlTypeType,
-        SessionExpirationDurationInSeconds: int = ...
+        SessionExpirationDurationInSeconds: int = ...,
     ) -> CreateApplicationPresignedUrlResponseTypeDef:
         """
         Creates and returns a URL that you can use to connect to an application's
         extension.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.create_application_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#create_application_presigned_url)
@@ -268,15 +268,15 @@
 
     async def delete_application_cloud_watch_logging_option(
         self,
         *,
         ApplicationName: str,
         CloudWatchLoggingOptionId: str,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> DeleteApplicationCloudWatchLoggingOptionResponseTypeDef:
         """
         Deletes an Amazon CloudWatch log stream from an Kinesis Data Analytics
         application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_cloud_watch_logging_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_cloud_watch_logging_option)
@@ -317,30 +317,30 @@
         """
 
     async def delete_application_snapshot(
         self,
         *,
         ApplicationName: str,
         SnapshotName: str,
-        SnapshotCreationTimestamp: TimestampTypeDef
+        SnapshotCreationTimestamp: TimestampTypeDef,
     ) -> Dict[str, Any]:
         """
         Deletes a snapshot of application state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_snapshot)
         """
 
     async def delete_application_vpc_configuration(
         self,
         *,
         ApplicationName: str,
         VpcConfigurationId: str,
         CurrentApplicationVersionId: int = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> DeleteApplicationVpcConfigurationResponseTypeDef:
         """
         Removes a VPC configuration from a Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.delete_application_vpc_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#delete_application_vpc_configuration)
         """
@@ -378,15 +378,15 @@
     async def discover_input_schema(
         self,
         *,
         ServiceExecutionRole: str,
         ResourceARN: str = ...,
         InputStartingPositionConfiguration: InputStartingPositionConfigurationTypeDef = ...,
         S3Configuration: S3ConfigurationTypeDef = ...,
-        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...
+        InputProcessingConfiguration: InputProcessingConfigurationTypeDef = ...,
     ) -> DiscoverInputSchemaResponseTypeDef:
         """
         Infers a schema for a SQL-based Kinesis Data Analytics application by
         evaluating sample records on the specified streaming source (Kinesis data
         stream or Kinesis Data Firehose delivery stream) or Amazon S3
         object.
 
@@ -499,28 +499,28 @@
         *,
         ApplicationName: str,
         CurrentApplicationVersionId: int = ...,
         ApplicationConfigurationUpdate: ApplicationConfigurationUpdateTypeDef = ...,
         ServiceExecutionRoleUpdate: str = ...,
         RunConfigurationUpdate: RunConfigurationUpdateTypeDef = ...,
         CloudWatchLoggingOptionUpdates: Sequence[CloudWatchLoggingOptionUpdateTypeDef] = ...,
-        ConditionalToken: str = ...
+        ConditionalToken: str = ...,
     ) -> UpdateApplicationResponseTypeDef:
         """
         Updates an existing Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.update_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#update_application)
         """
 
     async def update_application_maintenance_configuration(
         self,
         *,
         ApplicationName: str,
-        ApplicationMaintenanceConfigurationUpdate: ApplicationMaintenanceConfigurationUpdateTypeDef
+        ApplicationMaintenanceConfigurationUpdate: ApplicationMaintenanceConfigurationUpdateTypeDef,
     ) -> UpdateApplicationMaintenanceConfigurationResponseTypeDef:
         """
         Updates the maintenance configuration of the Kinesis Data Analytics application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2.Client.update_application_maintenance_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/client/#update_application_maintenance_configuration)
         """
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/literals.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/literals.py`

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
     "ApplicationModeType",
     "ApplicationRestoreTypeType",
     "ApplicationStatusType",
     "ArtifactTypeType",
     "CodeContentTypeType",
     "ConfigurationTypeType",
@@ -39,15 +38,14 @@
     "KinesisAnalyticsV2ServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ApplicationModeType = Literal["INTERACTIVE", "STREAMING"]
 ApplicationRestoreTypeType = Literal[
     "RESTORE_FROM_CUSTOM_SNAPSHOT", "RESTORE_FROM_LATEST_SNAPSHOT", "SKIP_RESTORE_FROM_SNAPSHOT"
 ]
 ApplicationStatusType = Literal[
     "AUTOSCALING",
     "DELETING",
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/literals.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/paginator.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     ListApplicationSnapshotsResponseTypeDef,
     ListApplicationsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListApplicationSnapshotsPaginator", "ListApplicationsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/paginator.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/type_defs.py` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "VpcConfigurationDescriptionTypeDef",
     "ApplicationSnapshotConfigurationDescriptionTypeDef",
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalyticsv2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.KinesisAnalyticsV2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/
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
 
 <a id="types-aiobotocore-kinesisanalyticsv2"></a>
 
 # types-aiobotocore-kinesisanalyticsv2
 
 [![PyPI - types-aiobotocore-kinesisanalyticsv2](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalyticsv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalyticsv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalyticsv2)](https://pepy.tech/project/types-aiobotocore-kinesisanalyticsv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.KinesisAnalyticsV2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
+[aiobotocore.KinesisAnalyticsV2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#KinesisAnalyticsV2)
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
 [types-aiobotocore-kinesisanalyticsv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalyticsv2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-kinesisanalyticsv2-2.9.0/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalyticsv2-2.9.1/types_aiobotocore_kinesisanalyticsv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

