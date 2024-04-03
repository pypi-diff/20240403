# Comparing `tmp/types-aiobotocore-rekognition-2.9.0.tar.gz` & `tmp/types-aiobotocore-rekognition-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rekognition-2.9.0.tar", last modified: Wed Dec 13 20:00:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-rekognition-2.9.1.tar", last modified: Thu Jan 18 01:21:36 2024, max compression
```

## Comparing `types-aiobotocore-rekognition-2.9.0.tar` & `types-aiobotocore-rekognition-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.005254 types-aiobotocore-rekognition-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2023-12-13 20:00:17.005254 types-aiobotocore-rekognition-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13730 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:17.005254 types-aiobotocore-rekognition-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.001254 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62435 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    62431 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15999 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    15997 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11569 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    89928 2023-12-13 19:54:34.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    89927 2023-12-13 19:54:33.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2023-12-13 19:54:32.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:17.001254 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15309 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-12-13 20:00:16.000000 types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.653089 types-aiobotocore-rekognition-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-01-18 01:21:36.653089 types-aiobotocore-rekognition-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13730 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:36.653089 types-aiobotocore-rekognition-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.653089 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62472 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62469 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15997 2024-01-18 01:16:08.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15997 2024-01-18 01:16:08.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    89927 2024-01-18 01:16:09.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89927 2024-01-18 01:16:09.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-01-18 01:16:07.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:36.653089 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15329 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-18 01:21:36.000000 types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rekognition-2.9.0/LICENSE` & `types-aiobotocore-rekognition-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-rekognition-2.9.0/PKG-INFO` & `types-aiobotocore-rekognition-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Rekognition 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Rekognition 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
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
 
 <a id="types-aiobotocore-rekognition"></a>
 
 # types-aiobotocore-rekognition
 
 [![PyPI - types-aiobotocore-rekognition](https://img.shields.io/pypi/v/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rekognition-2.9.0/README.md` & `types-aiobotocore-rekognition-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rekognition-2.9.0/setup.py` & `types-aiobotocore-rekognition-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rekognition",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_rekognition"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.Rekognition 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.Rekognition 2.9.1 service generated with"
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
     keywords="aiobotocore rekognition type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_rekognition": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__init__.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     ListStreamProcessorsPaginator,
     ListUsersPaginator,
 )
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 Client = RekognitionClient
 
-
 __all__ = (
     "Client",
     "DescribeProjectVersionsPaginator",
     "DescribeProjectsPaginator",
     "ListCollectionsPaginator",
     "ListDatasetEntriesPaginator",
     "ListDatasetLabelsPaginator",
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__init__.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/__main__.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Rekognition 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.Rekognition 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition\nOther"
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

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/client.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -149,26 +149,23 @@
 from .waiter import ProjectVersionRunningWaiter, ProjectVersionTrainingCompletedWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("RekognitionClient",)
 
-
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
@@ -187,15 +184,14 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
-
 class RekognitionClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
     """
 
     meta: ClientMeta
@@ -212,15 +208,15 @@
     async def associate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         UserMatchThreshold: float = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> AssociateFacesResponseTypeDef:
         """
         Associates one or more faces with an existing UserID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#associate_faces)
         """
@@ -243,15 +239,15 @@
 
     async def compare_faces(
         self,
         *,
         SourceImage: ImageTypeDef,
         TargetImage: ImageTypeDef,
         SimilarityThreshold: float = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> CompareFacesResponseTypeDef:
         """
         Compares a face in the *source* input image with each of the 100 largest faces
         detected in the *target* input
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.compare_faces)
@@ -263,15 +259,15 @@
         *,
         SourceProjectArn: str,
         SourceProjectVersionArn: str,
         DestinationProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
         Tags: Mapping[str, str] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> CopyProjectVersionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.copy_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#copy_project_version)
         """
@@ -287,43 +283,43 @@
         """
 
     async def create_dataset(
         self,
         *,
         DatasetType: DatasetTypeType,
         ProjectArn: str,
-        DatasetSource: DatasetSourceTypeDef = ...
+        DatasetSource: DatasetSourceTypeDef = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_dataset)
         """
 
     async def create_face_liveness_session(
         self,
         *,
         KmsKeyId: str = ...,
         Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateFaceLivenessSessionResponseTypeDef:
         """
         This API operation initiates a Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_face_liveness_session)
         """
 
     async def create_project(
         self,
         *,
         ProjectName: str,
         Feature: CustomizationFeatureType = ...,
-        AutoUpdate: ProjectAutoUpdateType = ...
+        AutoUpdate: ProjectAutoUpdateType = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project)
         """
@@ -335,15 +331,15 @@
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
         TrainingData: TrainingDataTypeDef = ...,
         TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...,
         VersionDescription: str = ...,
-        FeatureConfig: CustomizationFeatureConfigTypeDef = ...
+        FeatureConfig: CustomizationFeatureConfigTypeDef = ...,
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of Amazon Rekognition project (like a Custom Labels model
         or a custom adapter) and begins
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -358,15 +354,15 @@
         Name: str,
         Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
         RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
-        DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
+        DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...,
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -475,30 +471,30 @@
 
     async def describe_project_versions(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeProjectVersionsResponseTypeDef:
         """
         Lists and describes the versions of an Amazon Rekognition project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_project_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_project_versions)
         """
 
     async def describe_projects(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProjectNames: Sequence[str] = ...,
-        Features: Sequence[CustomizationFeatureType] = ...
+        Features: Sequence[CustomizationFeatureType] = ...,
     ) -> DescribeProjectsResponseTypeDef:
         """
         Gets information about your Rekognition projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_projects)
         """
@@ -515,15 +511,15 @@
 
     async def detect_custom_labels(
         self,
         *,
         ProjectVersionArn: str,
         Image: ImageTypeDef,
         MaxResults: int = ...,
-        MinConfidence: float = ...
+        MinConfidence: float = ...,
     ) -> DetectCustomLabelsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_custom_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_custom_labels)
         """
@@ -541,15 +537,15 @@
     async def detect_labels(
         self,
         *,
         Image: ImageTypeDef,
         MaxLabels: int = ...,
         MinConfidence: float = ...,
         Features: Sequence[DetectLabelsFeatureNameType] = ...,
-        Settings: DetectLabelsSettingsTypeDef = ...
+        Settings: DetectLabelsSettingsTypeDef = ...,
     ) -> DetectLabelsResponseTypeDef:
         """
         Detects instances of real-world entities within an image (JPEG or PNG) provided
         as
         input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_labels)
@@ -558,28 +554,28 @@
 
     async def detect_moderation_labels(
         self,
         *,
         Image: ImageTypeDef,
         MinConfidence: float = ...,
         HumanLoopConfig: HumanLoopConfigTypeDef = ...,
-        ProjectVersion: str = ...
+        ProjectVersion: str = ...,
     ) -> DetectModerationLabelsResponseTypeDef:
         """
         Detects unsafe content in a specified JPEG or PNG format image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_moderation_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_moderation_labels)
         """
 
     async def detect_protective_equipment(
         self,
         *,
         Image: ImageTypeDef,
-        SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...
+        SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...,
     ) -> DetectProtectiveEquipmentResponseTypeDef:
         """
         Detects Personal Protective Equipment (PPE) worn by people detected in an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_protective_equipment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_protective_equipment)
         """
@@ -596,15 +592,15 @@
 
     async def disassociate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> DisassociateFacesResponseTypeDef:
         """
         Removes the association between a `Face` supplied in an array of `FaceIds` and
         the
         User.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
@@ -647,15 +643,15 @@
 
     async def get_celebrity_recognition(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: CelebrityRecognitionSortByType = ...
+        SortBy: CelebrityRecognitionSortByType = ...,
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
         started by
         StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
@@ -665,15 +661,15 @@
     async def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ContentModerationSortByType = ...,
-        AggregateBy: ContentModerationAggregateByType = ...
+        AggregateBy: ContentModerationAggregateByType = ...,
     ) -> GetContentModerationResponseTypeDef:
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by
         StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
@@ -703,15 +699,15 @@
 
     async def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: FaceSearchSortByType = ...
+        SortBy: FaceSearchSortByType = ...,
     ) -> GetFaceSearchResponseTypeDef:
         """
         Gets the face search results for Amazon Rekognition Video face search started
         by
         StartFaceSearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_search)
@@ -721,15 +717,15 @@
     async def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: LabelDetectionSortByType = ...,
-        AggregateBy: LabelDetectionAggregateByType = ...
+        AggregateBy: LabelDetectionAggregateByType = ...,
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
         by
         StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
@@ -746,15 +742,15 @@
 
     async def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: PersonTrackingSortByType = ...
+        SortBy: PersonTrackingSortByType = ...,
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started
         by
         StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
@@ -789,15 +785,15 @@
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         ExternalImageId: str = ...,
         DetectionAttributes: Sequence[AttributeType] = ...,
         MaxFaces: int = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> IndexFacesResponseTypeDef:
         """
         Detects faces in the input image and adds them to the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.index_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#index_faces)
         """
@@ -817,15 +813,15 @@
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_entries)
         """
@@ -843,15 +839,15 @@
     async def list_faces(
         self,
         *,
         CollectionId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserId: str = ...,
-        FaceIds: Sequence[str] = ...
+        FaceIds: Sequence[str] = ...,
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_faces)
         """
@@ -931,15 +927,15 @@
 
     async def search_faces(
         self,
         *,
         CollectionId: str,
         FaceId: str,
         MaxFaces: int = ...,
-        FaceMatchThreshold: float = ...
+        FaceMatchThreshold: float = ...,
     ) -> SearchFacesResponseTypeDef:
         """
         For a given input face ID, searches for matching faces in the collection the
         face belongs
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces)
@@ -949,15 +945,15 @@
     async def search_faces_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> SearchFacesByImageResponseTypeDef:
         """
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching
         faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
@@ -967,15 +963,15 @@
     async def search_users(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceId: str = ...,
         UserMatchThreshold: float = ...,
-        MaxUsers: int = ...
+        MaxUsers: int = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users)
         """
@@ -983,30 +979,30 @@
     async def search_users_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         UserMatchThreshold: float = ...,
         MaxUsers: int = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> SearchUsersByImageResponseTypeDef:
         """
         Searches for UserIDs using a supplied image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users_by_image)
         """
 
     async def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartCelebrityRecognitionResponseTypeDef:
         """
         Starts asynchronous recognition of celebrities in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_celebrity_recognition)
         """
@@ -1014,15 +1010,15 @@
     async def start_content_moderation(
         self,
         *,
         Video: VideoTypeDef,
         MinConfidence: float = ...,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartContentModerationResponseTypeDef:
         """
         Starts asynchronous detection of inappropriate, unwanted, or offensive content
         in a stored
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_content_moderation)
@@ -1032,15 +1028,15 @@
     async def start_face_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         FaceAttributes: FaceAttributesType = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartFaceDetectionResponseTypeDef:
         """
         Starts asynchronous detection of faces in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_detection)
         """
@@ -1049,15 +1045,15 @@
         self,
         *,
         Video: VideoTypeDef,
         CollectionId: str,
         ClientRequestToken: str = ...,
         FaceMatchThreshold: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartFaceSearchResponseTypeDef:
         """
         Starts the asynchronous search for faces in a collection that match the faces
         of persons detected in a stored
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_search)
@@ -1069,15 +1065,15 @@
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
         Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
-        Settings: LabelDetectionSettingsTypeDef = ...
+        Settings: LabelDetectionSettingsTypeDef = ...,
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_label_detection)
         """
@@ -1086,30 +1082,30 @@
         self,
         *,
         OperationsConfig: MediaAnalysisOperationsConfigTypeDef,
         Input: MediaAnalysisInputTypeDef,
         OutputConfig: MediaAnalysisOutputConfigTypeDef,
         ClientRequestToken: str = ...,
         JobName: str = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> StartMediaAnalysisJobResponseTypeDef:
         """
         Initiates a new media analysis job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_media_analysis_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_media_analysis_job)
         """
 
     async def start_person_tracking(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartPersonTrackingResponseTypeDef:
         """
         Starts the asynchronous tracking of a person's path in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_person_tracking)
         """
@@ -1128,29 +1124,29 @@
         self,
         *,
         Video: VideoTypeDef,
         SegmentTypes: Sequence[SegmentTypeType],
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
-        Filters: StartSegmentDetectionFiltersTypeDef = ...
+        Filters: StartSegmentDetectionFiltersTypeDef = ...,
     ) -> StartSegmentDetectionResponseTypeDef:
         """
         Starts asynchronous detection of segment detection in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_segment_detection)
         """
 
     async def start_stream_processor(
         self,
         *,
         Name: str,
         StartSelector: StreamProcessingStartSelectorTypeDef = ...,
-        StopSelector: StreamProcessingStopSelectorTypeDef = ...
+        StopSelector: StreamProcessingStopSelectorTypeDef = ...,
     ) -> StartStreamProcessorResponseTypeDef:
         """
         Starts processing a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_stream_processor)
         """
@@ -1158,15 +1154,15 @@
     async def start_text_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
-        Filters: StartTextDetectionFiltersTypeDef = ...
+        Filters: StartTextDetectionFiltersTypeDef = ...,
     ) -> StartTextDetectionResponseTypeDef:
         """
         Starts asynchronous detection of text in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_text_detection)
         """
@@ -1222,15 +1218,15 @@
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
         RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
-        ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
+        ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...,
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_stream_processor)
         """
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/client.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,21 +151,23 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("RekognitionClient",)
 
+
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     HumanLoopQuotaExceededException: Type[BotocoreClientError]
     IdempotentParameterMismatchException: Type[BotocoreClientError]
     ImageTooLargeException: Type[BotocoreClientError]
@@ -184,14 +186,15 @@
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceNotReadyException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     SessionNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     VideoTooLargeException: Type[BotocoreClientError]
 
+
 class RekognitionClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/)
     """
 
     meta: ClientMeta
@@ -208,15 +211,15 @@
     async def associate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
         UserMatchThreshold: float = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> AssociateFacesResponseTypeDef:
         """
         Associates one or more faces with an existing UserID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.associate_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#associate_faces)
         """
@@ -239,15 +242,15 @@
 
     async def compare_faces(
         self,
         *,
         SourceImage: ImageTypeDef,
         TargetImage: ImageTypeDef,
         SimilarityThreshold: float = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> CompareFacesResponseTypeDef:
         """
         Compares a face in the *source* input image with each of the 100 largest faces
         detected in the *target* input
         image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.compare_faces)
@@ -259,15 +262,15 @@
         *,
         SourceProjectArn: str,
         SourceProjectVersionArn: str,
         DestinationProjectArn: str,
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
         Tags: Mapping[str, str] = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> CopyProjectVersionResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.copy_project_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#copy_project_version)
         """
@@ -283,43 +286,43 @@
         """
 
     async def create_dataset(
         self,
         *,
         DatasetType: DatasetTypeType,
         ProjectArn: str,
-        DatasetSource: DatasetSourceTypeDef = ...
+        DatasetSource: DatasetSourceTypeDef = ...,
     ) -> CreateDatasetResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_dataset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_dataset)
         """
 
     async def create_face_liveness_session(
         self,
         *,
         KmsKeyId: str = ...,
         Settings: CreateFaceLivenessSessionRequestSettingsTypeDef = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> CreateFaceLivenessSessionResponseTypeDef:
         """
         This API operation initiates a Face Liveness session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_face_liveness_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_face_liveness_session)
         """
 
     async def create_project(
         self,
         *,
         ProjectName: str,
         Feature: CustomizationFeatureType = ...,
-        AutoUpdate: ProjectAutoUpdateType = ...
+        AutoUpdate: ProjectAutoUpdateType = ...,
     ) -> CreateProjectResponseTypeDef:
         """
         Creates a new Amazon Rekognition project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#create_project)
         """
@@ -331,15 +334,15 @@
         VersionName: str,
         OutputConfig: OutputConfigTypeDef,
         TrainingData: TrainingDataTypeDef = ...,
         TestingData: TestingDataTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         KmsKeyId: str = ...,
         VersionDescription: str = ...,
-        FeatureConfig: CustomizationFeatureConfigTypeDef = ...
+        FeatureConfig: CustomizationFeatureConfigTypeDef = ...,
     ) -> CreateProjectVersionResponseTypeDef:
         """
         Creates a new version of Amazon Rekognition project (like a Custom Labels model
         or a custom adapter) and begins
         training.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_project_version)
@@ -354,15 +357,15 @@
         Name: str,
         Settings: StreamProcessorSettingsTypeDef,
         RoleArn: str,
         Tags: Mapping[str, str] = ...,
         NotificationChannel: StreamProcessorNotificationChannelTypeDef = ...,
         KmsKeyId: str = ...,
         RegionsOfInterest: Sequence[RegionOfInterestTypeDef] = ...,
-        DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...
+        DataSharingPreference: StreamProcessorDataSharingPreferenceTypeDef = ...,
     ) -> CreateStreamProcessorResponseTypeDef:
         """
         Creates an Amazon Rekognition stream processor that you can use to detect and
         recognize faces or to detect labels in a streaming
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.create_stream_processor)
@@ -471,30 +474,30 @@
 
     async def describe_project_versions(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> DescribeProjectVersionsResponseTypeDef:
         """
         Lists and describes the versions of an Amazon Rekognition project.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_project_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_project_versions)
         """
 
     async def describe_projects(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         ProjectNames: Sequence[str] = ...,
-        Features: Sequence[CustomizationFeatureType] = ...
+        Features: Sequence[CustomizationFeatureType] = ...,
     ) -> DescribeProjectsResponseTypeDef:
         """
         Gets information about your Rekognition projects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.describe_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#describe_projects)
         """
@@ -511,15 +514,15 @@
 
     async def detect_custom_labels(
         self,
         *,
         ProjectVersionArn: str,
         Image: ImageTypeDef,
         MaxResults: int = ...,
-        MinConfidence: float = ...
+        MinConfidence: float = ...,
     ) -> DetectCustomLabelsResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_custom_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_custom_labels)
         """
@@ -537,15 +540,15 @@
     async def detect_labels(
         self,
         *,
         Image: ImageTypeDef,
         MaxLabels: int = ...,
         MinConfidence: float = ...,
         Features: Sequence[DetectLabelsFeatureNameType] = ...,
-        Settings: DetectLabelsSettingsTypeDef = ...
+        Settings: DetectLabelsSettingsTypeDef = ...,
     ) -> DetectLabelsResponseTypeDef:
         """
         Detects instances of real-world entities within an image (JPEG or PNG) provided
         as
         input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_labels)
@@ -554,28 +557,28 @@
 
     async def detect_moderation_labels(
         self,
         *,
         Image: ImageTypeDef,
         MinConfidence: float = ...,
         HumanLoopConfig: HumanLoopConfigTypeDef = ...,
-        ProjectVersion: str = ...
+        ProjectVersion: str = ...,
     ) -> DetectModerationLabelsResponseTypeDef:
         """
         Detects unsafe content in a specified JPEG or PNG format image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_moderation_labels)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_moderation_labels)
         """
 
     async def detect_protective_equipment(
         self,
         *,
         Image: ImageTypeDef,
-        SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...
+        SummarizationAttributes: ProtectiveEquipmentSummarizationAttributesTypeDef = ...,
     ) -> DetectProtectiveEquipmentResponseTypeDef:
         """
         Detects Personal Protective Equipment (PPE) worn by people detected in an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.detect_protective_equipment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#detect_protective_equipment)
         """
@@ -592,15 +595,15 @@
 
     async def disassociate_faces(
         self,
         *,
         CollectionId: str,
         UserId: str,
         FaceIds: Sequence[str],
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> DisassociateFacesResponseTypeDef:
         """
         Removes the association between a `Face` supplied in an array of `FaceIds` and
         the
         User.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.disassociate_faces)
@@ -643,15 +646,15 @@
 
     async def get_celebrity_recognition(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: CelebrityRecognitionSortByType = ...
+        SortBy: CelebrityRecognitionSortByType = ...,
     ) -> GetCelebrityRecognitionResponseTypeDef:
         """
         Gets the celebrity recognition results for a Amazon Rekognition Video analysis
         started by
         StartCelebrityRecognition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_celebrity_recognition)
@@ -661,15 +664,15 @@
     async def get_content_moderation(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ContentModerationSortByType = ...,
-        AggregateBy: ContentModerationAggregateByType = ...
+        AggregateBy: ContentModerationAggregateByType = ...,
     ) -> GetContentModerationResponseTypeDef:
         """
         Gets the inappropriate, unwanted, or offensive content analysis results for a
         Amazon Rekognition Video analysis started by
         StartContentModeration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_content_moderation)
@@ -699,15 +702,15 @@
 
     async def get_face_search(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: FaceSearchSortByType = ...
+        SortBy: FaceSearchSortByType = ...,
     ) -> GetFaceSearchResponseTypeDef:
         """
         Gets the face search results for Amazon Rekognition Video face search started
         by
         StartFaceSearch.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_face_search)
@@ -717,15 +720,15 @@
     async def get_label_detection(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: LabelDetectionSortByType = ...,
-        AggregateBy: LabelDetectionAggregateByType = ...
+        AggregateBy: LabelDetectionAggregateByType = ...,
     ) -> GetLabelDetectionResponseTypeDef:
         """
         Gets the label detection results of a Amazon Rekognition Video analysis started
         by
         StartLabelDetection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_label_detection)
@@ -742,15 +745,15 @@
 
     async def get_person_tracking(
         self,
         *,
         JobId: str,
         MaxResults: int = ...,
         NextToken: str = ...,
-        SortBy: PersonTrackingSortByType = ...
+        SortBy: PersonTrackingSortByType = ...,
     ) -> GetPersonTrackingResponseTypeDef:
         """
         Gets the path tracking results of a Amazon Rekognition Video analysis started
         by
         StartPersonTracking.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.get_person_tracking)
@@ -785,15 +788,15 @@
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         ExternalImageId: str = ...,
         DetectionAttributes: Sequence[AttributeType] = ...,
         MaxFaces: int = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> IndexFacesResponseTypeDef:
         """
         Detects faces in the input image and adds them to the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.index_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#index_faces)
         """
@@ -813,15 +816,15 @@
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListDatasetEntriesResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_dataset_entries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_dataset_entries)
         """
@@ -839,15 +842,15 @@
     async def list_faces(
         self,
         *,
         CollectionId: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         UserId: str = ...,
-        FaceIds: Sequence[str] = ...
+        FaceIds: Sequence[str] = ...,
     ) -> ListFacesResponseTypeDef:
         """
         Returns metadata for faces in the specified collection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.list_faces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#list_faces)
         """
@@ -927,15 +930,15 @@
 
     async def search_faces(
         self,
         *,
         CollectionId: str,
         FaceId: str,
         MaxFaces: int = ...,
-        FaceMatchThreshold: float = ...
+        FaceMatchThreshold: float = ...,
     ) -> SearchFacesResponseTypeDef:
         """
         For a given input face ID, searches for matching faces in the collection the
         face belongs
         to.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces)
@@ -945,15 +948,15 @@
     async def search_faces_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         MaxFaces: int = ...,
         FaceMatchThreshold: float = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> SearchFacesByImageResponseTypeDef:
         """
         For a given input image, first detects the largest face in the image, and then
         searches the specified collection for matching
         faces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_faces_by_image)
@@ -963,15 +966,15 @@
     async def search_users(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceId: str = ...,
         UserMatchThreshold: float = ...,
-        MaxUsers: int = ...
+        MaxUsers: int = ...,
     ) -> SearchUsersResponseTypeDef:
         """
         Searches for UserIDs within a collection based on a `FaceId` or `UserId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users)
         """
@@ -979,30 +982,30 @@
     async def search_users_by_image(
         self,
         *,
         CollectionId: str,
         Image: ImageTypeDef,
         UserMatchThreshold: float = ...,
         MaxUsers: int = ...,
-        QualityFilter: QualityFilterType = ...
+        QualityFilter: QualityFilterType = ...,
     ) -> SearchUsersByImageResponseTypeDef:
         """
         Searches for UserIDs using a supplied image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.search_users_by_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#search_users_by_image)
         """
 
     async def start_celebrity_recognition(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartCelebrityRecognitionResponseTypeDef:
         """
         Starts asynchronous recognition of celebrities in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_celebrity_recognition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_celebrity_recognition)
         """
@@ -1010,15 +1013,15 @@
     async def start_content_moderation(
         self,
         *,
         Video: VideoTypeDef,
         MinConfidence: float = ...,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartContentModerationResponseTypeDef:
         """
         Starts asynchronous detection of inappropriate, unwanted, or offensive content
         in a stored
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_content_moderation)
@@ -1028,15 +1031,15 @@
     async def start_face_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         FaceAttributes: FaceAttributesType = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartFaceDetectionResponseTypeDef:
         """
         Starts asynchronous detection of faces in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_face_detection)
         """
@@ -1045,15 +1048,15 @@
         self,
         *,
         Video: VideoTypeDef,
         CollectionId: str,
         ClientRequestToken: str = ...,
         FaceMatchThreshold: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartFaceSearchResponseTypeDef:
         """
         Starts the asynchronous search for faces in a collection that match the faces
         of persons detected in a stored
         video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_face_search)
@@ -1065,15 +1068,15 @@
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         MinConfidence: float = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
         Features: Sequence[Literal["GENERAL_LABELS"]] = ...,
-        Settings: LabelDetectionSettingsTypeDef = ...
+        Settings: LabelDetectionSettingsTypeDef = ...,
     ) -> StartLabelDetectionResponseTypeDef:
         """
         Starts asynchronous detection of labels in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_label_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_label_detection)
         """
@@ -1082,30 +1085,30 @@
         self,
         *,
         OperationsConfig: MediaAnalysisOperationsConfigTypeDef,
         Input: MediaAnalysisInputTypeDef,
         OutputConfig: MediaAnalysisOutputConfigTypeDef,
         ClientRequestToken: str = ...,
         JobName: str = ...,
-        KmsKeyId: str = ...
+        KmsKeyId: str = ...,
     ) -> StartMediaAnalysisJobResponseTypeDef:
         """
         Initiates a new media analysis job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_media_analysis_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_media_analysis_job)
         """
 
     async def start_person_tracking(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
-        JobTag: str = ...
+        JobTag: str = ...,
     ) -> StartPersonTrackingResponseTypeDef:
         """
         Starts the asynchronous tracking of a person's path in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_person_tracking)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_person_tracking)
         """
@@ -1124,29 +1127,29 @@
         self,
         *,
         Video: VideoTypeDef,
         SegmentTypes: Sequence[SegmentTypeType],
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
-        Filters: StartSegmentDetectionFiltersTypeDef = ...
+        Filters: StartSegmentDetectionFiltersTypeDef = ...,
     ) -> StartSegmentDetectionResponseTypeDef:
         """
         Starts asynchronous detection of segment detection in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_segment_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_segment_detection)
         """
 
     async def start_stream_processor(
         self,
         *,
         Name: str,
         StartSelector: StreamProcessingStartSelectorTypeDef = ...,
-        StopSelector: StreamProcessingStopSelectorTypeDef = ...
+        StopSelector: StreamProcessingStopSelectorTypeDef = ...,
     ) -> StartStreamProcessorResponseTypeDef:
         """
         Starts processing a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_stream_processor)
         """
@@ -1154,15 +1157,15 @@
     async def start_text_detection(
         self,
         *,
         Video: VideoTypeDef,
         ClientRequestToken: str = ...,
         NotificationChannel: NotificationChannelTypeDef = ...,
         JobTag: str = ...,
-        Filters: StartTextDetectionFiltersTypeDef = ...
+        Filters: StartTextDetectionFiltersTypeDef = ...,
     ) -> StartTextDetectionResponseTypeDef:
         """
         Starts asynchronous detection of text in a stored video.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.start_text_detection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#start_text_detection)
         """
@@ -1218,15 +1221,15 @@
     async def update_stream_processor(
         self,
         *,
         Name: str,
         SettingsForUpdate: StreamProcessorSettingsForUpdateTypeDef = ...,
         RegionsOfInterestForUpdate: Sequence[RegionOfInterestTypeDef] = ...,
         DataSharingPreferenceForUpdate: StreamProcessorDataSharingPreferenceTypeDef = ...,
-        ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...
+        ParametersToDelete: Sequence[StreamProcessorParameterToDeleteType] = ...,
     ) -> Dict[str, Any]:
         """
         Allows you to update a stream processor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Client.update_stream_processor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/client/#update_stream_processor)
         """
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/literals.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/literals.py`

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
     "AttributeType",
     "BodyPartType",
     "CelebrityRecognitionSortByType",
     "ContentClassifierType",
     "ContentModerationAggregateByType",
     "ContentModerationSortByType",
@@ -79,15 +78,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AttributeType = Literal[
     "AGE_RANGE",
     "ALL",
     "BEARD",
     "DEFAULT",
     "EMOTIONS",
     "EYEGLASSES",
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/literals.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/paginator.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     "ListDatasetLabelsPaginator",
     "ListFacesPaginator",
     "ListProjectPoliciesPaginator",
     "ListStreamProcessorsPaginator",
     "ListUsersPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -86,15 +85,15 @@
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeProjectVersionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
         """
 
 
@@ -105,15 +104,15 @@
     """
 
     def paginate(
         self,
         *,
         ProjectNames: Sequence[str] = ...,
         Features: Sequence[CustomizationFeatureType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
         """
 
 
@@ -142,15 +141,15 @@
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
         """
 
 
@@ -177,15 +176,15 @@
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
         """
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/paginator.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
 
     def paginate(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeProjectVersionsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectversionspaginator)
         """
 
 class DescribeProjectsPaginator(AioPaginator):
@@ -101,15 +101,15 @@
     """
 
     def paginate(
         self,
         *,
         ProjectNames: Sequence[str] = ...,
         Features: Sequence[CustomizationFeatureType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeProjectsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#describeprojectspaginator)
         """
 
 class ListCollectionsPaginator(AioPaginator):
@@ -136,15 +136,15 @@
         self,
         *,
         DatasetArn: str,
         ContainsLabels: Sequence[str] = ...,
         Labeled: bool = ...,
         SourceRefContains: str = ...,
         HasErrors: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listdatasetentriespaginator)
         """
 
 class ListDatasetLabelsPaginator(AioPaginator):
@@ -169,15 +169,15 @@
 
     def paginate(
         self,
         *,
         CollectionId: str,
         UserId: str = ...,
         FaceIds: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/paginators/#listfacespaginator)
         """
 
 class ListProjectPoliciesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/type_defs.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgeRangeTypeDef",
     "AssociateFacesRequestRequestTypeDef",
     "AssociatedFaceTypeDef",
     "ResponseMetadataTypeDef",
     "UnsuccessfulFaceAssociationTypeDef",
     "AudioMetadataTypeDef",
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/type_defs.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/waiter.py` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/waiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     async def wait(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/waiters/#projectversionrunningwaiter)
         """
 
 
@@ -62,13 +62,13 @@
     async def wait(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionTrainingCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/waiters/#projectversiontrainingcompletedwaiter)
         """
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition/waiter.pyi` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition/waiter.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     async def wait(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionRunning.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/waiters/#projectversionrunningwaiter)
         """
 
 class ProjectVersionTrainingCompletedWaiter(AIOWaiter):
@@ -60,13 +60,13 @@
     async def wait(
         self,
         *,
         ProjectArn: str,
         VersionNames: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Waiter.ProjectVersionTrainingCompleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/waiters/#projectversiontrainingcompletedwaiter)
         """
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/PKG-INFO` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rekognition
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.Rekognition 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.Rekognition 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/
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
 
 <a id="types-aiobotocore-rekognition"></a>
 
 # types-aiobotocore-rekognition
 
 [![PyPI - types-aiobotocore-rekognition](https://img.shields.io/pypi/v/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-rekognition.svg?color=blue)](https://pypi.org/project/types-aiobotocore-rekognition)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-rekognition)](https://pepy.tech/project/types-aiobotocore-rekognition)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.Rekognition 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
+[aiobotocore.Rekognition 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
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
 [types-aiobotocore-rekognition docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rekognition/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-rekognition-2.9.0/types_aiobotocore_rekognition.egg-info/SOURCES.txt` & `types-aiobotocore-rekognition-2.9.1/types_aiobotocore_rekognition.egg-info/SOURCES.txt`

 * *Files identical despite different names*

