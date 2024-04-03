# Comparing `tmp/types-aiobotocore-macie2-2.9.0.tar.gz` & `tmp/types-aiobotocore-macie2-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie2-2.9.0.tar", last modified: Wed Dec 13 19:59:49 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie2-2.9.1.tar", last modified: Thu Jan 18 01:21:11 2024, max compression
```

## Comparing `types-aiobotocore-macie2-2.9.0.tar` & `types-aiobotocore-macie2-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.341497 types-aiobotocore-macie2-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-12-13 19:59:49.341497 types-aiobotocore-macie2-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14564 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:49.341497 types-aiobotocore-macie2-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.341497 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63431 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    63427 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18217 2023-12-13 19:49:39.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18215 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    20372 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    86948 2023-12-13 19:49:40.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    86947 2023-12-13 19:49:39.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:36.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2023-12-13 19:49:38.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:49.341497 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16123 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-12-13 19:59:49.000000 types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.545203 types-aiobotocore-macie2-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-01-18 01:21:11.545203 types-aiobotocore-macie2-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14564 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:11.545203 types-aiobotocore-macie2-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.541203 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63448 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63445 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-01-18 01:11:24.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18215 2024-01-18 01:11:24.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20359 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    86947 2024-01-18 01:11:25.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86947 2024-01-18 01:11:25.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-18 01:11:23.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.545203 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-01-18 01:21:11.000000 types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie2-2.9.0/LICENSE` & `types-aiobotocore-macie2-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-macie2-2.9.0/PKG-INFO` & `types-aiobotocore-macie2-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Macie2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Macie2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
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
 
 <a id="types-aiobotocore-macie2"></a>
 
 # types-aiobotocore-macie2
 
 [![PyPI - types-aiobotocore-macie2](https://img.shields.io/pypi/v/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-macie2-2.9.0/README.md` & `types-aiobotocore-macie2-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-macie2-2.9.0/setup.py` & `types-aiobotocore-macie2-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie2",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Macie2 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.Macie2 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore macie2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_macie2": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__init__.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     ListSensitivityInspectionTemplatesPaginator,
     SearchResourcesPaginator,
 )
 from .waiter import FindingRevealedWaiter
 
 Client = Macie2Client
 
-
 __all__ = (
     "Client",
     "DescribeBucketsPaginator",
     "FindingRevealedWaiter",
     "GetUsageStatisticsPaginator",
     "ListAllowListsPaginator",
     "ListClassificationJobsPaginator",
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__init__.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/__main__.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie2 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Macie2 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/client.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 from .waiter import FindingRevealedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("Macie2Client",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -219,15 +218,15 @@
     async def create_allow_list(
         self,
         *,
         clientToken: str,
         criteria: AllowListCriteriaTypeDef,
         name: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAllowListResponseTypeDef:
         """
         Creates and defines the settings for an allow list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_allow_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_allow_list)
         """
@@ -243,15 +242,15 @@
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
         scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
         """
@@ -263,15 +262,15 @@
         regex: str,
         clientToken: str = ...,
         description: str = ...,
         ignoreWords: Sequence[str] = ...,
         keywords: Sequence[str] = ...,
         maximumMatchDistance: int = ...,
         severityLevels: Sequence[SeverityLevelTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateCustomDataIdentifierResponseTypeDef:
         """
         Creates and defines the criteria and other settings for a custom data
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
@@ -282,15 +281,15 @@
         *,
         action: FindingsFilterActionType,
         findingCriteria: FindingCriteriaTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFindingsFilterResponseTypeDef:
         """
         Creates and defines the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_findings_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_findings_filter)
         """
@@ -382,15 +381,15 @@
 
     async def describe_buckets(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: BucketSortCriteriaTypeDef = ...
+        sortCriteria: BucketSortCriteriaTypeDef = ...,
     ) -> DescribeBucketsResponseTypeDef:
         """
         Retrieves (queries) statistical data and other information about one or more S3
         buckets that Amazon Macie monitors and analyzes for an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.describe_buckets)
@@ -463,15 +462,15 @@
         """
 
     async def enable_macie(
         self,
         *,
         clientToken: str = ...,
         findingPublishingFrequency: FindingPublishingFrequencyType = ...,
-        status: MacieStatusType = ...
+        status: MacieStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Enables Amazon Macie and specifies the configuration settings for a Macie
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.enable_macie)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#enable_macie)
@@ -574,15 +573,15 @@
 
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
         findingCriteria: FindingCriteriaTypeDef = ...,
         size: int = ...,
-        sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
+        sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...,
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_finding_statistics)
         """
@@ -706,15 +705,15 @@
     async def get_usage_statistics(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
-        timeRange: TimeRangeType = ...
+        timeRange: TimeRangeType = ...,
     ) -> GetUsageStatisticsResponseTypeDef:
         """
         Retrieves (queries) quotas and aggregated usage data for one or more accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_usage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_usage_statistics)
         """
@@ -739,15 +738,15 @@
 
     async def list_classification_jobs(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: ListJobsSortCriteriaTypeDef = ...
+        sortCriteria: ListJobsSortCriteriaTypeDef = ...,
     ) -> ListClassificationJobsResponseTypeDef:
         """
         Retrieves a subset of information about one or more classification jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_classification_jobs)
         """
@@ -775,15 +774,15 @@
 
     async def list_findings(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SortCriteriaTypeDef = ...
+        sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_findings)
         """
@@ -904,30 +903,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#put_classification_export_configuration)
         """
 
     async def put_findings_publication_configuration(
         self,
         *,
         clientToken: str = ...,
-        securityHubConfiguration: SecurityHubConfigurationTypeDef = ...
+        securityHubConfiguration: SecurityHubConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration settings for publishing findings to Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.put_findings_publication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#put_findings_publication_configuration)
         """
 
     async def search_resources(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SearchResourcesSortCriteriaTypeDef = ...
+        sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
     ) -> SearchResourcesResponseTypeDef:
         """
         Retrieves (queries) statistical data and other information about Amazon Web
         Services resources that Amazon Macie monitors and
         analyzes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.search_resources)
@@ -947,15 +946,15 @@
     async def test_custom_data_identifier(
         self,
         *,
         regex: str,
         sampleText: str,
         ignoreWords: Sequence[str] = ...,
         keywords: Sequence[str] = ...,
-        maximumMatchDistance: int = ...
+        maximumMatchDistance: int = ...,
     ) -> TestCustomDataIdentifierResponseTypeDef:
         """
         Tests a custom data identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.test_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#test_custom_data_identifier)
         """
@@ -1013,28 +1012,28 @@
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
         findingCriteria: FindingCriteriaTypeDef = ...,
         name: str = ...,
-        position: int = ...
+        position: int = ...,
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_findings_filter)
         """
 
     async def update_macie_session(
         self,
         *,
         findingPublishingFrequency: FindingPublishingFrequencyType = ...,
-        status: MacieStatusType = ...
+        status: MacieStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Suspends or re-enables Amazon Macie, or updates the configuration settings for
         a Macie
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_macie_session)
@@ -1070,28 +1069,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_resource_profile)
         """
 
     async def update_resource_profile_detections(
         self,
         *,
         resourceArn: str,
-        suppressDataIdentifiers: Sequence[SuppressDataIdentifierTypeDef] = ...
+        suppressDataIdentifiers: Sequence[SuppressDataIdentifierTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the sensitivity scoring settings for an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_resource_profile_detections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_resource_profile_detections)
         """
 
     async def update_reveal_configuration(
         self,
         *,
         configuration: RevealConfigurationTypeDef,
-        retrievalConfiguration: UpdateRetrievalConfigurationTypeDef = ...
+        retrievalConfiguration: UpdateRetrievalConfigurationTypeDef = ...,
     ) -> UpdateRevealConfigurationResponseTypeDef:
         """
         Updates the status and configuration settings for retrieving occurrences of
         sensitive data reported by
         findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_reveal_configuration)
@@ -1100,15 +1099,15 @@
 
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
         excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
+        includes: SensitivityInspectionTemplateIncludesTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/client.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -215,15 +215,15 @@
     async def create_allow_list(
         self,
         *,
         clientToken: str,
         criteria: AllowListCriteriaTypeDef,
         name: str,
         description: str = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateAllowListResponseTypeDef:
         """
         Creates and defines the settings for an allow list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_allow_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_allow_list)
         """
@@ -239,15 +239,15 @@
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
         scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
         """
@@ -259,15 +259,15 @@
         regex: str,
         clientToken: str = ...,
         description: str = ...,
         ignoreWords: Sequence[str] = ...,
         keywords: Sequence[str] = ...,
         maximumMatchDistance: int = ...,
         severityLevels: Sequence[SeverityLevelTypeDef] = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateCustomDataIdentifierResponseTypeDef:
         """
         Creates and defines the criteria and other settings for a custom data
         identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
@@ -278,15 +278,15 @@
         *,
         action: FindingsFilterActionType,
         findingCriteria: FindingCriteriaTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
-        tags: Mapping[str, str] = ...
+        tags: Mapping[str, str] = ...,
     ) -> CreateFindingsFilterResponseTypeDef:
         """
         Creates and defines the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_findings_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_findings_filter)
         """
@@ -378,15 +378,15 @@
 
     async def describe_buckets(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: BucketSortCriteriaTypeDef = ...
+        sortCriteria: BucketSortCriteriaTypeDef = ...,
     ) -> DescribeBucketsResponseTypeDef:
         """
         Retrieves (queries) statistical data and other information about one or more S3
         buckets that Amazon Macie monitors and analyzes for an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.describe_buckets)
@@ -459,15 +459,15 @@
         """
 
     async def enable_macie(
         self,
         *,
         clientToken: str = ...,
         findingPublishingFrequency: FindingPublishingFrequencyType = ...,
-        status: MacieStatusType = ...
+        status: MacieStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Enables Amazon Macie and specifies the configuration settings for a Macie
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.enable_macie)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#enable_macie)
@@ -570,15 +570,15 @@
 
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
         findingCriteria: FindingCriteriaTypeDef = ...,
         size: int = ...,
-        sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
+        sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...,
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_finding_statistics)
         """
@@ -702,15 +702,15 @@
     async def get_usage_statistics(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
-        timeRange: TimeRangeType = ...
+        timeRange: TimeRangeType = ...,
     ) -> GetUsageStatisticsResponseTypeDef:
         """
         Retrieves (queries) quotas and aggregated usage data for one or more accounts.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_usage_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_usage_statistics)
         """
@@ -735,15 +735,15 @@
 
     async def list_classification_jobs(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: ListJobsSortCriteriaTypeDef = ...
+        sortCriteria: ListJobsSortCriteriaTypeDef = ...,
     ) -> ListClassificationJobsResponseTypeDef:
         """
         Retrieves a subset of information about one or more classification jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_classification_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_classification_jobs)
         """
@@ -771,15 +771,15 @@
 
     async def list_findings(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SortCriteriaTypeDef = ...
+        sortCriteria: SortCriteriaTypeDef = ...,
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_findings)
         """
@@ -900,30 +900,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#put_classification_export_configuration)
         """
 
     async def put_findings_publication_configuration(
         self,
         *,
         clientToken: str = ...,
-        securityHubConfiguration: SecurityHubConfigurationTypeDef = ...
+        securityHubConfiguration: SecurityHubConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the configuration settings for publishing findings to Security Hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.put_findings_publication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#put_findings_publication_configuration)
         """
 
     async def search_resources(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        sortCriteria: SearchResourcesSortCriteriaTypeDef = ...
+        sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
     ) -> SearchResourcesResponseTypeDef:
         """
         Retrieves (queries) statistical data and other information about Amazon Web
         Services resources that Amazon Macie monitors and
         analyzes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.search_resources)
@@ -943,15 +943,15 @@
     async def test_custom_data_identifier(
         self,
         *,
         regex: str,
         sampleText: str,
         ignoreWords: Sequence[str] = ...,
         keywords: Sequence[str] = ...,
-        maximumMatchDistance: int = ...
+        maximumMatchDistance: int = ...,
     ) -> TestCustomDataIdentifierResponseTypeDef:
         """
         Tests a custom data identifier.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.test_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#test_custom_data_identifier)
         """
@@ -1009,28 +1009,28 @@
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
         findingCriteria: FindingCriteriaTypeDef = ...,
         name: str = ...,
-        position: int = ...
+        position: int = ...,
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_findings_filter)
         """
 
     async def update_macie_session(
         self,
         *,
         findingPublishingFrequency: FindingPublishingFrequencyType = ...,
-        status: MacieStatusType = ...
+        status: MacieStatusType = ...,
     ) -> Dict[str, Any]:
         """
         Suspends or re-enables Amazon Macie, or updates the configuration settings for
         a Macie
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_macie_session)
@@ -1066,28 +1066,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_resource_profile)
         """
 
     async def update_resource_profile_detections(
         self,
         *,
         resourceArn: str,
-        suppressDataIdentifiers: Sequence[SuppressDataIdentifierTypeDef] = ...
+        suppressDataIdentifiers: Sequence[SuppressDataIdentifierTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates the sensitivity scoring settings for an S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_resource_profile_detections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_resource_profile_detections)
         """
 
     async def update_reveal_configuration(
         self,
         *,
         configuration: RevealConfigurationTypeDef,
-        retrievalConfiguration: UpdateRetrievalConfigurationTypeDef = ...
+        retrievalConfiguration: UpdateRetrievalConfigurationTypeDef = ...,
     ) -> UpdateRevealConfigurationResponseTypeDef:
         """
         Updates the status and configuration settings for retrieving occurrences of
         sensitive data reported by
         findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_reveal_configuration)
@@ -1096,15 +1096,15 @@
 
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
         excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
+        includes: SensitivityInspectionTemplateIncludesTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/literals.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/literals.py`

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
     "AdminStatusType",
     "AllowListStatusCodeType",
     "AllowsUnencryptedObjectUploadsType",
     "AutomatedDiscoveryStatusType",
     "AvailabilityCodeType",
     "BucketMetadataErrorCodeType",
@@ -98,15 +97,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AdminStatusType = Literal["DISABLING_IN_PROGRESS", "ENABLED"]
 AllowListStatusCodeType = Literal[
     "OK",
     "S3_OBJECT_ACCESS_DENIED",
     "S3_OBJECT_EMPTY",
     "S3_OBJECT_NOT_FOUND",
     "S3_OBJECT_OVERSIZE",
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/literals.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/paginator.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     "ListOrganizationAdminAccountsPaginator",
     "ListResourceProfileArtifactsPaginator",
     "ListResourceProfileDetectionsPaginator",
     "ListSensitivityInspectionTemplatesPaginator",
     "SearchResourcesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -124,15 +123,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#describebucketspaginator)
         """
 
 
@@ -144,15 +143,15 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#getusagestatisticspaginator)
         """
 
 
@@ -178,15 +177,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClassificationJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationjobspaginator)
         """
 
 
@@ -227,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
 
 
@@ -366,13 +365,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/paginator.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#describebucketspaginator)
         """
 
 class GetUsageStatisticsPaginator(AioPaginator):
@@ -140,15 +140,15 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#getusagestatisticspaginator)
         """
 
 class ListAllowListsPaginator(AioPaginator):
@@ -172,15 +172,15 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClassificationJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationjobspaginator)
         """
 
 class ListClassificationScopesPaginator(AioPaginator):
@@ -218,15 +218,15 @@
     """
 
     def paginate(
         self,
         *,
         findingCriteria: FindingCriteriaTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
 
 class ListFindingsFiltersPaginator(AioPaginator):
@@ -348,13 +348,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/type_defs.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptInvitationRequestRequestTypeDef",
     "AccessControlListTypeDef",
     "AccountDetailTypeDef",
     "BlockPublicAccessTypeDef",
     "AdminAccountTypeDef",
     "S3WordsListTypeDef",
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/type_defs.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/waiter.py` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2/waiter.pyi` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/PKG-INFO` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie2
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Macie2 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Macie2 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
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
 
 <a id="types-aiobotocore-macie2"></a>
 
 # types-aiobotocore-macie2
 
 [![PyPI - types-aiobotocore-macie2](https://img.shields.io/pypi/v/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Macie2 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
+[aiobotocore.Macie2 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-macie2-2.9.0/types_aiobotocore_macie2.egg-info/SOURCES.txt` & `types-aiobotocore-macie2-2.9.1/types_aiobotocore_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

