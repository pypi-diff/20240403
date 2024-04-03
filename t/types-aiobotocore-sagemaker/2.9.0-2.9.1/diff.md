# Comparing `tmp/types-aiobotocore-sagemaker-2.9.0.tar.gz` & `tmp/types-aiobotocore-sagemaker-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-2.9.0.tar", last modified: Wed Dec 13 20:00:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-2.9.1.tar", last modified: Thu Jan 18 01:21:44 2024, max compression
```

## Comparing `types-aiobotocore-sagemaker-2.9.0.tar` & `types-aiobotocore-sagemaker-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:25.625179 types-aiobotocore-sagemaker-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26997 2023-12-13 20:00:25.625179 types-aiobotocore-sagemaker-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25426 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 20:00:25.625179 types-aiobotocore-sagemaker-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:25.621179 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/
--rw-r--r--   0 runner    (1001) docker     (127)    19439 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19438 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   286491 2023-12-13 19:55:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   286487 2023-12-13 19:55:24.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    61589 2023-12-13 19:55:30.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    61587 2023-12-13 19:55:29.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   106071 2023-12-13 19:55:26.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)   105996 2023-12-13 19:55:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   497964 2023-12-13 19:55:40.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   497963 2023-12-13 19:55:34.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:55:23.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14122 2023-12-13 19:55:26.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14109 2023-12-13 19:55:26.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 20:00:25.625179 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26997 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-12-13 20:00:25.000000 types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:44.457054 types-aiobotocore-sagemaker-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27017 2024-01-18 01:21:44.457054 types-aiobotocore-sagemaker-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25426 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:44.457054 types-aiobotocore-sagemaker-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:44.457054 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286658 2024-01-18 01:17:02.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   286655 2024-01-18 01:16:57.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    61587 2024-01-18 01:17:04.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61587 2024-01-18 01:17:03.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   106136 2024-01-18 01:17:03.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106063 2024-01-18 01:17:02.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   497963 2024-01-18 01:17:15.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   497963 2024-01-18 01:17:09.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:16:56.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-01-18 01:17:03.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-01-18 01:17:03.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:44.457054 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27017 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-18 01:21:44.000000 types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/LICENSE` & `types-aiobotocore-sagemaker-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-sagemaker-2.9.0/PKG-INFO` & `types-aiobotocore-sagemaker-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SageMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SageMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/
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
 
 <a id="types-aiobotocore-sagemaker"></a>
 
 # types-aiobotocore-sagemaker
 
 [![PyPI - types-aiobotocore-sagemaker](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [types-aiobotocore-sagemaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/README.md` & `types-aiobotocore-sagemaker-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [types-aiobotocore-sagemaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/setup.py` & `types-aiobotocore-sagemaker-2.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_sagemaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.SageMaker 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.SageMaker 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore sagemaker type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sagemaker": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__init__.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,14 @@
     ProcessingJobCompletedOrStoppedWaiter,
     TrainingJobCompletedOrStoppedWaiter,
     TransformJobCompletedOrStoppedWaiter,
 )
 
 Client = SageMakerClient
 
-
 __all__ = (
     "Client",
     "EndpointDeletedWaiter",
     "EndpointInServiceWaiter",
     "ImageCreatedWaiter",
     "ImageDeletedWaiter",
     "ImageUpdatedWaiter",
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__init__.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/__main__.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SageMaker 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.SageMaker 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker\nOther"
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

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/client.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,15 +637,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("SageMakerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -742,15 +741,15 @@
         ActionName: str,
         Source: ActionSourceTypeDef,
         ActionType: str,
         Description: str = ...,
         Status: ActionStatusType = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateActionResponseTypeDef:
         """
         Creates an *action*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_action)
         """
@@ -760,15 +759,15 @@
         *,
         AlgorithmName: str,
         TrainingSpecification: TrainingSpecificationTypeDef,
         AlgorithmDescription: str = ...,
         InferenceSpecification: InferenceSpecificationTypeDef = ...,
         ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services
         Marketplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_algorithm)
@@ -780,30 +779,30 @@
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResourceSpec: ResourceSpecTypeDef = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates a running app for the specified UserProfile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app)
         """
 
     async def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
         KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app_image_config)
         """
@@ -812,15 +811,15 @@
         self,
         *,
         Source: ArtifactSourceTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateArtifactResponseTypeDef:
         """
         Creates an *artifact*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_artifact)
         """
@@ -833,15 +832,15 @@
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ModelDeployConfig: ModelDeployConfigTypeDef = ...
+        ModelDeployConfig: ModelDeployConfigTypeDef = ...,
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_auto_ml_job)
         """
@@ -854,15 +853,15 @@
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
-        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
+        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...,
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_auto_ml_job_v2)
@@ -870,29 +869,29 @@
 
     async def create_cluster(
         self,
         *,
         ClusterName: str,
         InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_cluster)
         """
 
     async def create_code_repository(
         self,
         *,
         CodeRepositoryName: str,
         GitConfig: GitConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCodeRepositoryOutputTypeDef:
         """
         Creates a Git repository as a resource in your SageMaker account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_code_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_code_repository)
         """
@@ -903,15 +902,15 @@
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
         VpcConfig: NeoVpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_compilation_job)
         """
@@ -920,15 +919,15 @@
         self,
         *,
         ContextName: str,
         Source: ContextSourceTypeDef,
         ContextType: str,
         Description: str = ...,
         Properties: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateContextResponseTypeDef:
         """
         Creates a *context*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_context)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_context)
         """
@@ -941,15 +940,15 @@
         DataQualityJobInput: DataQualityJobInputTypeDef,
         DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_data_quality_job_definition)
         """
@@ -958,15 +957,15 @@
         self,
         *,
         DeviceFleetName: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         RoleArn: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EnableIotRoleAlias: bool = ...
+        EnableIotRoleAlias: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a device fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_device_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_device_fleet)
         """
@@ -981,15 +980,15 @@
         VpcId: str,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
         DomainSettings: DomainSettingsTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_domain)
         """
@@ -997,15 +996,15 @@
     async def create_edge_deployment_plan(
         self,
         *,
         EdgeDeploymentPlanName: str,
         ModelConfigs: Sequence[EdgeDeploymentModelConfigTypeDef],
         DeviceFleetName: str,
         Stages: Sequence[DeploymentStageTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEdgeDeploymentPlanResponseTypeDef:
         """
         Creates an edge deployment plan, consisting of multiple stages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_edge_deployment_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_edge_deployment_plan)
         """
@@ -1026,30 +1025,30 @@
         EdgePackagingJobName: str,
         CompilationJobName: str,
         ModelName: str,
         ModelVersion: str,
         RoleArn: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         ResourceKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Starts a SageMaker Edge Manager model packaging job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_edge_packaging_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_edge_packaging_job)
         """
 
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         DeploymentConfig: DeploymentConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_endpoint)
         """
@@ -1063,15 +1062,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
         ExplainerConfig: ExplainerConfigTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...,
         ExecutionRoleArn: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        EnableNetworkIsolation: bool = ...
+        EnableNetworkIsolation: bool = ...,
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to
         deploy
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint_config)
@@ -1080,15 +1079,15 @@
 
     async def create_experiment(
         self,
         *,
         ExperimentName: str,
         DisplayName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateExperimentResponseTypeDef:
         """
         Creates a SageMaker *experiment*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_experiment)
         """
@@ -1100,15 +1099,15 @@
         RecordIdentifierFeatureName: str,
         EventTimeFeatureName: str,
         FeatureDefinitions: Sequence[FeatureDefinitionTypeDef],
         OnlineStoreConfig: OnlineStoreConfigTypeDef = ...,
         OfflineStoreConfig: OfflineStoreConfigTypeDef = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFeatureGroupResponseTypeDef:
         """
         Create a new `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_feature_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_feature_group)
         """
@@ -1118,15 +1117,15 @@
         *,
         FlowDefinitionName: str,
         HumanLoopConfig: HumanLoopConfigTypeDef,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
         Creates a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_flow_definition)
         """
@@ -1135,29 +1134,29 @@
         self,
         *,
         HubName: str,
         HubDescription: str,
         HubDisplayName: str = ...,
         HubSearchKeywords: Sequence[str] = ...,
         S3StorageConfig: HubS3StorageConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHubResponseTypeDef:
         """
         Create a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hub)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_hub)
         """
 
     async def create_human_task_ui(
         self,
         *,
         HumanTaskUiName: str,
         UiTemplate: UiTemplateTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHumanTaskUiResponseTypeDef:
         """
         Defines the settings you will use for the human review workflow user interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_human_task_ui)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_human_task_ui)
         """
@@ -1167,15 +1166,15 @@
         *,
         HyperParameterTuningJobName: str,
         HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
         TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
         TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
         WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Autotune: AutotuneTypeDef = ...
+        Autotune: AutotuneTypeDef = ...,
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_hyper_parameter_tuning_job)
         """
@@ -1183,15 +1182,15 @@
     async def create_image(
         self,
         *,
         ImageName: str,
         RoleArn: str,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateImageResponseTypeDef:
         """
         Creates a custom SageMaker image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_image)
         """
@@ -1205,15 +1204,15 @@
         Aliases: Sequence[str] = ...,
         VendorGuidance: VendorGuidanceType = ...,
         JobType: JobTypeType = ...,
         MLFramework: str = ...,
         ProgrammingLang: str = ...,
         Processor: ProcessorType = ...,
         Horovod: bool = ...,
-        ReleaseNotes: str = ...
+        ReleaseNotes: str = ...,
     ) -> CreateImageVersionResponseTypeDef:
         """
         Creates a version of the SageMaker image specified by `ImageName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_image_version)
         """
@@ -1222,15 +1221,15 @@
         self,
         *,
         InferenceComponentName: str,
         EndpointName: str,
         VariantName: str,
         Specification: InferenceComponentSpecificationTypeDef,
         RuntimeConfig: InferenceComponentRuntimeConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceComponentOutputTypeDef:
         """
         Creates an inference component, which is a SageMaker hosting object that you
         can use to deploy a model to an
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_component)
@@ -1246,15 +1245,15 @@
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
         ShadowModeConfig: ShadowModeConfigTypeDef,
         Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
         KmsKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_inference_experiment)
@@ -1266,15 +1265,15 @@
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
         InputConfig: RecommendationJobInputConfigTypeDef,
         JobDescription: str = ...,
         StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_inference_recommendations_job)
         """
@@ -1287,15 +1286,15 @@
         InputConfig: LabelingJobInputConfigTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
         HumanTaskConfig: HumanTaskConfigTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
         LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_labeling_job)
         """
@@ -1306,15 +1305,15 @@
         ModelName: str,
         PrimaryContainer: ContainerDefinitionTypeDef = ...,
         Containers: Sequence[ContainerDefinitionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        EnableNetworkIsolation: bool = ...
+        EnableNetworkIsolation: bool = ...,
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model)
         """
@@ -1327,15 +1326,15 @@
         ModelBiasJobInput: ModelBiasJobInputTypeDef,
         ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_bias_job_definition)
         """
@@ -1343,30 +1342,30 @@
     async def create_model_card(
         self,
         *,
         ModelCardName: str,
         Content: str,
         ModelCardStatus: ModelCardStatusType,
         SecurityConfig: ModelCardSecurityConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelCardResponseTypeDef:
         """
         Creates an Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_card)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card)
         """
 
     async def create_model_card_export_job(
         self,
         *,
         ModelCardName: str,
         ModelCardExportJobName: str,
         OutputConfig: ModelCardExportOutputConfigTypeDef,
-        ModelCardVersion: int = ...
+        ModelCardVersion: int = ...,
     ) -> CreateModelCardExportJobResponseTypeDef:
         """
         Creates an Amazon SageMaker Model Card export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_card_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card_export_job)
         """
@@ -1379,15 +1378,15 @@
         ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
         ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_explainability_job_definition)
         """
@@ -1411,15 +1410,15 @@
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         AdditionalInferenceSpecifications: Sequence[
             AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...,
-        SkipModelValidation: SkipModelValidationType = ...
+        SkipModelValidation: SkipModelValidationType = ...,
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package)
@@ -1427,15 +1426,15 @@
         """
 
     async def create_model_package_group(
         self,
         *,
         ModelPackageGroupName: str,
         ModelPackageGroupDescription: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelPackageGroupOutputTypeDef:
         """
         Creates a model group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_package_group)
         """
@@ -1448,29 +1447,29 @@
         ModelQualityJobInput: ModelQualityJobInputTypeDef,
         ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_quality_job_definition)
         """
 
     async def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
         MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker
         Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_monitoring_schedule)
@@ -1491,29 +1490,29 @@
         DirectInternetAccess: DirectInternetAccessType = ...,
         VolumeSizeInGB: int = ...,
         AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,
         DefaultCodeRepository: str = ...,
         AdditionalCodeRepositories: Sequence[str] = ...,
         RootAccess: RootAccessType = ...,
         PlatformIdentifier: str = ...,
-        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...
+        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,
     ) -> CreateNotebookInstanceOutputTypeDef:
         """
         Creates an SageMaker notebook instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_notebook_instance)
         """
 
     async def create_notebook_instance_lifecycle_config(
         self,
         *,
         NotebookInstanceLifecycleConfigName: str,
         OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
-        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...
+        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
     ) -> CreateNotebookInstanceLifecycleConfigOutputTypeDef:
         """
         Creates a lifecycle configuration that you can associate with a notebook
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance_lifecycle_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_notebook_instance_lifecycle_config)
@@ -1526,15 +1525,15 @@
         ClientRequestToken: str,
         RoleArn: str,
         PipelineDisplayName: str = ...,
         PipelineDefinition: str = ...,
         PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,
         PipelineDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline using a JSON pipeline definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_pipeline)
         """
@@ -1543,15 +1542,15 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SessionExpirationDurationInSeconds: int = ...,
         ExpiresInSeconds: int = ...,
         SpaceName: str = ...,
-        LandingUri: str = ...
+        LandingUri: str = ...,
     ) -> CreatePresignedDomainUrlResponseTypeDef:
         """
         Creates a URL for a specified UserProfile in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_presigned_domain_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_presigned_domain_url)
         """
@@ -1576,30 +1575,30 @@
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
         ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
         NetworkConfig: NetworkConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExperimentConfig: ExperimentConfigTypeDef = ...
+        ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_processing_job)
         """
 
     async def create_project(
         self,
         *,
         ProjectName: str,
         ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
         ProjectDescription: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_project)
@@ -1611,30 +1610,30 @@
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
         SpaceSettings: SpaceSettingsTypeDef = ...,
         SpaceDisplayName: str = ...,
         OwnershipSettings: OwnershipSettingsTypeDef = ...,
-        SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...
+        SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...,
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_space)
         """
 
     async def create_studio_lifecycle_config(
         self,
         *,
         StudioLifecycleConfigName: str,
         StudioLifecycleConfigContent: str,
         StudioLifecycleConfigAppType: StudioLifecycleConfigAppTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStudioLifecycleConfigResponseTypeDef:
         """
         Creates a new Amazon SageMaker Studio Lifecycle Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_studio_lifecycle_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_studio_lifecycle_config)
         """
@@ -1660,15 +1659,15 @@
         DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
         ProfilerConfig: ProfilerConfigTypeDef = ...,
         ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...,
-        InfraCheckConfig: InfraCheckConfigTypeDef = ...
+        InfraCheckConfig: InfraCheckConfigTypeDef = ...,
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_training_job)
         """
@@ -1685,15 +1684,15 @@
         ModelClientConfig: ModelClientConfigTypeDef = ...,
         MaxPayloadInMB: int = ...,
         BatchStrategy: BatchStrategyType = ...,
         Environment: Mapping[str, str] = ...,
         DataCaptureConfig: BatchDataCaptureConfigTypeDef = ...,
         DataProcessing: DataProcessingTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExperimentConfig: ExperimentConfigTypeDef = ...
+        ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateTransformJobResponseTypeDef:
         """
         Starts a transform job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_transform_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_transform_job)
         """
@@ -1701,15 +1700,15 @@
     async def create_trial(
         self,
         *,
         TrialName: str,
         ExperimentName: str,
         DisplayName: str = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrialResponseTypeDef:
         """
         Creates an SageMaker *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_trial)
         """
@@ -1722,15 +1721,15 @@
         Status: TrialComponentStatusTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrialComponentResponseTypeDef:
         """
         Creates a *trial component*, which is a stage of a machine learning *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_trial_component)
         """
@@ -1739,15 +1738,15 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsTypeDef = ...
+        UserSettings: UserSettingsTypeDef = ...,
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_user_profile)
         """
@@ -1756,15 +1755,15 @@
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         SourceIpConfig: SourceIpConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
+        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workforce)
         """
@@ -1773,15 +1772,15 @@
         self,
         *,
         WorkteamName: str,
         MemberDefinitions: Sequence[MemberDefinitionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workteam)
         """
@@ -1805,15 +1804,15 @@
     async def delete_app(
         self,
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to stop and delete an app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_app)
         """
@@ -1979,15 +1978,15 @@
 
     async def delete_hub_content(
         self,
         *,
         HubName: str,
         HubContentType: HubContentTypeType,
         HubContentName: str,
-        HubContentVersion: str
+        HubContentVersion: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete the contents of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_hub_content)
         """
@@ -2259,15 +2258,15 @@
     async def describe_app(
         self,
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> DescribeAppResponseTypeDef:
         """
         Describes the app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#describe_app)
         """
@@ -2488,15 +2487,15 @@
 
     async def describe_hub_content(
         self,
         *,
         HubName: str,
         HubContentType: HubContentTypeType,
         HubContentName: str,
-        HubContentVersion: str = ...
+        HubContentVersion: str = ...,
     ) -> DescribeHubContentResponseTypeDef:
         """
         Describe the content of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#describe_hub_content)
         """
@@ -2928,15 +2927,15 @@
     async def get_scaling_configuration_recommendation(
         self,
         *,
         InferenceRecommendationsJobName: str,
         RecommendationId: str = ...,
         EndpointName: str = ...,
         TargetCpuUtilizationPerCore: int = ...,
-        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
+        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...,
     ) -> GetScalingConfigurationRecommendationResponseTypeDef:
         """
         Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
         """
@@ -2960,15 +2959,15 @@
         HubName: str,
         HubContentDocument: str,
         HubContentVersion: str = ...,
         HubContentDisplayName: str = ...,
         HubContentDescription: str = ...,
         HubContentMarkdown: str = ...,
         HubContentSearchKeywords: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportHubContentResponseTypeDef:
         """
         Import hub content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.import_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#import_hub_content)
         """
@@ -2979,15 +2978,15 @@
         SourceUri: str = ...,
         ActionType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortActionsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListActionsResponseTypeDef:
         """
         Lists the actions in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_actions)
         """
@@ -2997,15 +2996,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: AlgorithmSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListAlgorithmsOutputTypeDef:
         """
         Lists the machine learning algorithms that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_algorithms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_algorithms)
         """
@@ -3013,15 +3012,15 @@
     async def list_aliases(
         self,
         *,
         ImageName: str,
         Alias: str = ...,
         Version: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesResponseTypeDef:
         """
         Lists the aliases of a specified image or image version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_aliases)
         """
@@ -3033,15 +3032,15 @@
         NextToken: str = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListAppImageConfigsResponseTypeDef:
         """
         Lists the AppImageConfigs in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_app_image_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_app_image_configs)
         """
@@ -3051,15 +3050,15 @@
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         DomainIdEquals: str = ...,
         UserProfileNameEquals: str = ...,
-        SpaceNameEquals: str = ...
+        SpaceNameEquals: str = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists apps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_apps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_apps)
         """
@@ -3070,15 +3069,15 @@
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListArtifactsResponseTypeDef:
         """
         Lists the artifacts in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_artifacts)
         """
@@ -3092,15 +3091,15 @@
         DestinationType: str = ...,
         AssociationType: AssociationEdgeTypeType = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortAssociationsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAssociationsResponseTypeDef:
         """
         Lists the associations in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_associations)
         """
@@ -3113,15 +3112,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: AutoMLJobStatusType = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: AutoMLSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAutoMLJobsResponseTypeDef:
         """
         Request a list of jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_auto_ml_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_auto_ml_jobs)
         """
@@ -3131,15 +3130,15 @@
         *,
         AutoMLJobName: str,
         StatusEquals: CandidateStatusType = ...,
         CandidateNameEquals: str = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: CandidateSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCandidatesForAutoMLJobResponseTypeDef:
         """
         List the candidates created for the job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_candidates_for_auto_ml_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_candidates_for_auto_ml_job)
         """
@@ -3150,15 +3149,15 @@
         ClusterName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         InstanceGroupNameContains: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ClusterSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListClusterNodesResponseTypeDef:
         """
         Retrieves the list of instances (also called *nodes* interchangeably) in a
         SageMaker HyperPod
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_cluster_nodes)
@@ -3170,15 +3169,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ClusterSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListClustersResponseTypeDef:
         """
         Retrieves the list of SageMaker HyperPod clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_clusters)
         """
@@ -3190,15 +3189,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: CodeRepositorySortByType = ...,
-        SortOrder: CodeRepositorySortOrderType = ...
+        SortOrder: CodeRepositorySortOrderType = ...,
     ) -> ListCodeRepositoriesOutputTypeDef:
         """
         Gets a list of the Git repositories in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_code_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_code_repositories)
         """
@@ -3211,15 +3210,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: CompilationJobStatusType = ...,
         SortBy: ListCompilationJobsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCompilationJobsResponseTypeDef:
         """
         Lists model compilation jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_compilation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_compilation_jobs)
         """
@@ -3230,15 +3229,15 @@
         SourceUri: str = ...,
         ContextType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortContextsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListContextsResponseTypeDef:
         """
         Lists the contexts in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_contexts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_contexts)
         """
@@ -3249,15 +3248,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListDataQualityJobDefinitionsResponseTypeDef:
         """
         Lists the data quality job definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_data_quality_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_data_quality_job_definitions)
         """
@@ -3269,15 +3268,15 @@
         MaxResults: int = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ListDeviceFleetsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListDeviceFleetsResponseTypeDef:
         """
         Returns a list of devices in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_device_fleets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_device_fleets)
         """
@@ -3285,15 +3284,15 @@
     async def list_devices(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LatestHeartbeatAfter: TimestampTypeDef = ...,
         ModelName: str = ...,
-        DeviceFleetName: str = ...
+        DeviceFleetName: str = ...,
     ) -> ListDevicesResponseTypeDef:
         """
         A list of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_devices)
         """
@@ -3316,15 +3315,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         DeviceFleetNameContains: str = ...,
         SortBy: ListEdgeDeploymentPlansSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListEdgeDeploymentPlansResponseTypeDef:
         """
         Lists all edge deployment plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_edge_deployment_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_edge_deployment_plans)
         """
@@ -3338,15 +3337,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelNameContains: str = ...,
         StatusEquals: EdgePackagingJobStatusType = ...,
         SortBy: ListEdgePackagingJobsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListEdgePackagingJobsResponseTypeDef:
         """
         Returns a list of edge packaging jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_edge_packaging_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_edge_packaging_jobs)
         """
@@ -3356,15 +3355,15 @@
         *,
         SortBy: EndpointConfigSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListEndpointConfigsOutputTypeDef:
         """
         Lists endpoint configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoint_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_endpoint_configs)
         """
@@ -3377,15 +3376,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
-        StatusEquals: EndpointStatusType = ...
+        StatusEquals: EndpointStatusType = ...,
     ) -> ListEndpointsOutputTypeDef:
         """
         Lists endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_endpoints)
         """
@@ -3394,15 +3393,15 @@
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListExperimentsResponseTypeDef:
         """
         Lists all the experiments in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_experiments)
         """
@@ -3414,15 +3413,15 @@
         FeatureGroupStatusEquals: FeatureGroupStatusType = ...,
         OfflineStoreStatusEquals: OfflineStoreStatusValueType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFeatureGroupsResponseTypeDef:
         """
         List `FeatureGroup`s based on given filter and order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_feature_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_feature_groups)
         """
@@ -3430,15 +3429,15 @@
     async def list_flow_definitions(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlowDefinitionsResponseTypeDef:
         """
         Returns information about the flow definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_flow_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_flow_definitions)
         """
@@ -3452,15 +3451,15 @@
         MinVersion: str = ...,
         MaxSchemaVersion: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         SortBy: HubContentSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubContentVersionsResponseTypeDef:
         """
         List hub content versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hub_content_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hub_content_versions)
         """
@@ -3473,15 +3472,15 @@
         NameContains: str = ...,
         MaxSchemaVersion: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         SortBy: HubContentSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubContentsResponseTypeDef:
         """
         List the contents of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hub_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hub_contents)
         """
@@ -3493,15 +3492,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: HubSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubsResponseTypeDef:
         """
         List all existing hubs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hubs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hubs)
         """
@@ -3509,15 +3508,15 @@
     async def list_human_task_uis(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListHumanTaskUisResponseTypeDef:
         """
         Returns information about the human task user interfaces in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_human_task_uis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_human_task_uis)
         """
@@ -3530,15 +3529,15 @@
         SortBy: HyperParameterTuningJobSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
-        StatusEquals: HyperParameterTuningJobStatusType = ...
+        StatusEquals: HyperParameterTuningJobStatusType = ...,
     ) -> ListHyperParameterTuningJobsResponseTypeDef:
         """
         Gets a list of
         [HyperParameterTuningJobSummary](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobSummary.html)
         objects that describe the hyperparameter tuning jobs launched in your
         account.
 
@@ -3553,15 +3552,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ImageVersionSortByType = ...,
-        SortOrder: ImageVersionSortOrderType = ...
+        SortOrder: ImageVersionSortOrderType = ...,
     ) -> ListImageVersionsResponseTypeDef:
         """
         Lists the versions of a specified image and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_image_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_image_versions)
         """
@@ -3573,15 +3572,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ImageSortByType = ...,
-        SortOrder: ImageSortOrderType = ...
+        SortOrder: ImageSortOrderType = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Lists the images in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_images)
         """
@@ -3596,15 +3595,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: InferenceComponentStatusType = ...,
         EndpointNameEquals: str = ...,
-        VariantNameEquals: str = ...
+        VariantNameEquals: str = ...,
     ) -> ListInferenceComponentsOutputTypeDef:
         """
         Lists the inference components in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_components)
         """
@@ -3618,15 +3617,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInferenceExperimentsResponseTypeDef:
         """
         Returns the list of all inference experiments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_experiments)
         """
@@ -3634,15 +3633,15 @@
     async def list_inference_recommendations_job_steps(
         self,
         *,
         JobName: str,
         Status: RecommendationJobStatusType = ...,
         StepType: Literal["BENCHMARK"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListInferenceRecommendationsJobStepsResponseTypeDef:
         """
         Returns a list of the subtasks for an Inference Recommender job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_recommendations_job_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_recommendations_job_steps)
         """
@@ -3657,15 +3656,15 @@
         NameContains: str = ...,
         StatusEquals: RecommendationJobStatusType = ...,
         SortBy: ListInferenceRecommendationsJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ModelNameEquals: str = ...,
-        ModelPackageVersionArnEquals: str = ...
+        ModelPackageVersionArnEquals: str = ...,
     ) -> ListInferenceRecommendationsJobsResponseTypeDef:
         """
         Lists recommendation jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_recommendations_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_recommendations_jobs)
         """
@@ -3678,15 +3677,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: LabelingJobStatusType = ...
+        StatusEquals: LabelingJobStatusType = ...,
     ) -> ListLabelingJobsResponseTypeDef:
         """
         Gets a list of labeling jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_labeling_jobs)
         """
@@ -3697,15 +3696,15 @@
         WorkteamArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         JobReferenceCodeContains: str = ...,
         SortBy: Literal["CreationTime"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListLabelingJobsForWorkteamResponseTypeDef:
         """
         Gets a list of labeling jobs assigned to a specified work team.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs_for_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_labeling_jobs_for_workteam)
         """
@@ -3714,15 +3713,15 @@
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortLineageGroupsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLineageGroupsResponseTypeDef:
         """
         A list of lineage groups shared with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_lineage_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_lineage_groups)
         """
@@ -3733,15 +3732,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelBiasJobDefinitionsResponseTypeDef:
         """
         Lists model bias jobs definitions that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_bias_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_bias_job_definitions)
         """
@@ -3754,15 +3753,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardExportJobNameContains: str = ...,
         StatusEquals: ModelCardExportJobStatusType = ...,
         SortBy: ModelCardExportJobSortByType = ...,
         SortOrder: ModelCardExportJobSortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListModelCardExportJobsResponseTypeDef:
         """
         List the export jobs for the Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_card_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_card_export_jobs)
         """
@@ -3773,15 +3772,15 @@
         ModelCardName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         NextToken: str = ...,
         SortBy: Literal["Version"] = ...,
-        SortOrder: ModelCardSortOrderType = ...
+        SortOrder: ModelCardSortOrderType = ...,
     ) -> ListModelCardVersionsResponseTypeDef:
         """
         List existing versions of an Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_card_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_card_versions)
         """
@@ -3792,15 +3791,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         NextToken: str = ...,
         SortBy: ModelCardSortByType = ...,
-        SortOrder: ModelCardSortOrderType = ...
+        SortOrder: ModelCardSortOrderType = ...,
     ) -> ListModelCardsResponseTypeDef:
         """
         List existing model cards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_cards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_cards)
         """
@@ -3811,29 +3810,29 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelExplainabilityJobDefinitionsResponseTypeDef:
         """
         Lists model explainability job definitions that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_explainability_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_explainability_job_definitions)
         """
 
     async def list_model_metadata(
         self,
         *,
         SearchExpression: ModelMetadataSearchExpressionTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListModelMetadataResponseTypeDef:
         """
         Lists the domain, framework, task, and model name of standard machine learning
         models found in common model
         zoos.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_metadata)
@@ -3845,15 +3844,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ModelPackageGroupSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListModelPackageGroupsOutputTypeDef:
         """
         Gets a list of the model groups in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_package_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_package_groups)
         """
@@ -3866,15 +3865,15 @@
         MaxResults: int = ...,
         NameContains: str = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageType: ModelPackageTypeType = ...,
         NextToken: str = ...,
         SortBy: ModelPackageSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListModelPackagesOutputTypeDef:
         """
         Lists the model packages that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_packages)
         """
@@ -3885,15 +3884,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelQualityJobDefinitionsResponseTypeDef:
         """
         Gets a list of model quality monitoring job definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_quality_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_quality_job_definitions)
         """
@@ -3903,15 +3902,15 @@
         *,
         SortBy: ModelSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelsOutputTypeDef:
         """
         Lists models created with the `CreateModel` API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_models)
         """
@@ -3923,15 +3922,15 @@
         MonitoringAlertName: str = ...,
         SortBy: MonitoringAlertHistorySortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        StatusEquals: MonitoringAlertStatusType = ...
+        StatusEquals: MonitoringAlertStatusType = ...,
     ) -> ListMonitoringAlertHistoryResponseTypeDef:
         """
         Gets a list of past alerts in a model monitoring schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_alert_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_alert_history)
         """
@@ -3959,15 +3958,15 @@
         ScheduledTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ExecutionStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
-        MonitoringTypeEquals: MonitoringTypeType = ...
+        MonitoringTypeEquals: MonitoringTypeType = ...,
     ) -> ListMonitoringExecutionsResponseTypeDef:
         """
         Returns list of all monitoring job executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_executions)
         """
@@ -3983,15 +3982,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ScheduleStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
-        MonitoringTypeEquals: MonitoringTypeType = ...
+        MonitoringTypeEquals: MonitoringTypeType = ...,
     ) -> ListMonitoringSchedulesResponseTypeDef:
         """
         Returns list of all monitoring schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_schedules)
         """
@@ -4003,15 +4002,15 @@
         MaxResults: int = ...,
         SortBy: NotebookInstanceLifecycleConfigSortKeyType = ...,
         SortOrder: NotebookInstanceLifecycleConfigSortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
-        LastModifiedTimeAfter: TimestampTypeDef = ...
+        LastModifiedTimeAfter: TimestampTypeDef = ...,
     ) -> ListNotebookInstanceLifecycleConfigsOutputTypeDef:
         """
         Lists notebook instance lifestyle configurations created with the
         [CreateNotebookInstanceLifecycleConfig](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html)
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instance_lifecycle_configs)
@@ -4029,15 +4028,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: NotebookInstanceStatusType = ...,
         NotebookInstanceLifecycleConfigNameContains: str = ...,
         DefaultCodeRepositoryContains: str = ...,
-        AdditionalCodeRepositoryEquals: str = ...
+        AdditionalCodeRepositoryEquals: str = ...,
     ) -> ListNotebookInstancesOutputTypeDef:
         """
         Returns a list of the SageMaker notebook instances in the requester's account
         in an Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instances)
@@ -4046,15 +4045,15 @@
 
     async def list_pipeline_execution_steps(
         self,
         *,
         PipelineExecutionArn: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListPipelineExecutionStepsResponseTypeDef:
         """
         Gets a list of `PipeLineExecutionStep` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_execution_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipeline_execution_steps)
         """
@@ -4064,15 +4063,15 @@
         *,
         PipelineName: str,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelineExecutionsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPipelineExecutionsResponseTypeDef:
         """
         Gets a list of the pipeline executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipeline_executions)
         """
@@ -4092,15 +4091,15 @@
         *,
         PipelineNamePrefix: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelinesByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPipelinesResponseTypeDef:
         """
         Gets a list of pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipelines)
         """
@@ -4113,15 +4112,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: ProcessingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProcessingJobsResponseTypeDef:
         """
         Lists processing jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_processing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_processing_jobs)
         """
@@ -4131,15 +4130,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ProjectSortByType = ...,
-        SortOrder: ProjectSortOrderType = ...
+        SortOrder: ProjectSortOrderType = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Gets a list of the projects in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_projects)
         """
@@ -4149,15 +4148,15 @@
         *,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: ResourceCatalogSortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourceCatalogsResponseTypeDef:
         """
         Lists Amazon SageMaker Catalogs based on given filters and orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_resource_catalogs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_resource_catalogs)
         """
@@ -4166,15 +4165,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
         DomainIdEquals: str = ...,
-        SpaceNameContains: str = ...
+        SpaceNameContains: str = ...,
     ) -> ListSpacesResponseTypeDef:
         """
         Lists spaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_spaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_spaces)
         """
@@ -4182,15 +4181,15 @@
     async def list_stage_devices(
         self,
         *,
         EdgeDeploymentPlanName: str,
         StageName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ExcludeDevicesDeployedInOtherStage: bool = ...
+        ExcludeDevicesDeployedInOtherStage: bool = ...,
     ) -> ListStageDevicesResponseTypeDef:
         """
         Lists devices allocated to the stage, containing detailed device information
         and deployment
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_stage_devices)
@@ -4205,15 +4204,15 @@
         NameContains: str = ...,
         AppTypeEquals: StudioLifecycleConfigAppTypeType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: StudioLifecycleConfigSortKeyType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListStudioLifecycleConfigsResponseTypeDef:
         """
         Lists the Amazon SageMaker Studio Lifecycle Configurations in your Amazon Web
         Services
         Account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_studio_lifecycle_configs)
@@ -4251,15 +4250,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        WarmPoolStatusEquals: WarmPoolResourceStatusType = ...
+        WarmPoolStatusEquals: WarmPoolResourceStatusType = ...,
     ) -> ListTrainingJobsResponseTypeDef:
         """
         Lists training jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_training_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_training_jobs)
         """
@@ -4268,15 +4267,15 @@
         self,
         *,
         HyperParameterTuningJobName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: TrainingJobSortByOptionsType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListTrainingJobsForHyperParameterTuningJobResponseTypeDef:
         """
         Gets a list of
         [TrainingJobSummary](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html)
         objects that describe the training jobs that a hyperparameter tuning job
         launched.
 
@@ -4292,15 +4291,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TransformJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTransformJobsResponseTypeDef:
         """
         Lists transform jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_transform_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_transform_jobs)
         """
@@ -4312,15 +4311,15 @@
         TrialName: str = ...,
         SourceArn: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialComponentsByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTrialComponentsResponseTypeDef:
         """
         Lists the trial components in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trial_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_trial_components)
         """
@@ -4331,15 +4330,15 @@
         ExperimentName: str = ...,
         TrialComponentName: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialsByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTrialsResponseTypeDef:
         """
         Lists the trials in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_trials)
         """
@@ -4348,15 +4347,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: UserProfileSortKeyType = ...,
         DomainIdEquals: str = ...,
-        UserProfileNameContains: str = ...
+        UserProfileNameContains: str = ...,
     ) -> ListUserProfilesResponseTypeDef:
         """
         Lists user profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_user_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_user_profiles)
         """
@@ -4364,15 +4363,15 @@
     async def list_workforces(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkforcesResponseTypeDef:
         """
         Use this operation to list all private and vendor workforces in an Amazon Web
         Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workforces)
@@ -4382,15 +4381,15 @@
     async def list_workteams(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkteamsResponseTypeDef:
         """
         Gets a list of private work teams that you have defined in a region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workteams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_workteams)
         """
@@ -4410,59 +4409,59 @@
         *,
         StartArns: Sequence[str] = ...,
         Direction: DirectionType = ...,
         IncludeEdges: bool = ...,
         Filters: QueryFiltersTypeDef = ...,
         MaxDepth: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> QueryLineageResponseTypeDef:
         """
         Use this action to inspect your lineage and discover relationships between
         entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.query_lineage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#query_lineage)
         """
 
     async def register_devices(
         self,
         *,
         DeviceFleetName: str,
         Devices: Sequence[DeviceTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Register devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.register_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#register_devices)
         """
 
     async def render_ui_template(
         self,
         *,
         Task: RenderableTaskTypeDef,
         RoleArn: str,
         UiTemplate: UiTemplateTypeDef = ...,
-        HumanTaskUiArn: str = ...
+        HumanTaskUiArn: str = ...,
     ) -> RenderUiTemplateResponseTypeDef:
         """
         Renders the UI template so that you can preview the worker's experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.render_ui_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#render_ui_template)
         """
 
     async def retry_pipeline_execution(
         self,
         *,
         PipelineExecutionArn: str,
         ClientRequestToken: str,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> RetryPipelineExecutionResponseTypeDef:
         """
         Retry the execution of the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.retry_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#retry_pipeline_execution)
         """
@@ -4472,15 +4471,15 @@
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        CrossAccountFilterOption: CrossAccountFilterOptionType = ...
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
     ) -> SearchResponseTypeDef:
         """
         Finds SageMaker resources that match a search query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#search)
         """
@@ -4498,15 +4497,15 @@
         """
 
     async def send_pipeline_execution_step_success(
         self,
         *,
         CallbackToken: str,
         OutputParameters: Sequence[OutputParameterTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> SendPipelineExecutionStepSuccessResponseTypeDef:
         """
         Notifies the pipeline that the execution of a callback step succeeded and
         provides a list of the step's output
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.send_pipeline_execution_step_success)
@@ -4560,15 +4559,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...
+        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...,
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#start_pipeline_execution)
         """
@@ -4626,15 +4625,15 @@
     async def stop_inference_experiment(
         self,
         *,
         Name: str,
         ModelVariantActions: Mapping[str, ModelVariantActionType],
         DesiredModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
         DesiredState: InferenceExperimentStopDesiredStateType = ...,
-        Reason: str = ...
+        Reason: str = ...,
     ) -> StopInferenceExperimentResponseTypeDef:
         """
         Stops an inference experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#stop_inference_experiment)
         """
@@ -4714,57 +4713,57 @@
     async def update_action(
         self,
         *,
         ActionName: str,
         Description: str = ...,
         Status: ActionStatusType = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateActionResponseTypeDef:
         """
         Updates an action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_action)
         """
 
     async def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_app_image_config)
         """
 
     async def update_artifact(
         self,
         *,
         ArtifactArn: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateArtifactResponseTypeDef:
         """
         Updates an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_artifact)
         """
 
     async def update_cluster(
         self,
         *,
         ClusterName: str,
-        InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef]
+        InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
     ) -> UpdateClusterResponseTypeDef:
         """
         Update a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_cluster)
         """
@@ -4781,15 +4780,15 @@
 
     async def update_context(
         self,
         *,
         ContextName: str,
         Description: str = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateContextResponseTypeDef:
         """
         Updates a context.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_context)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_context)
         """
@@ -4797,15 +4796,15 @@
     async def update_device_fleet(
         self,
         *,
         DeviceFleetName: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         RoleArn: str = ...,
         Description: str = ...,
-        EnableIotRoleAlias: bool = ...
+        EnableIotRoleAlias: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a fleet of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_device_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_device_fleet)
         """
@@ -4825,15 +4824,15 @@
         *,
         DomainId: str,
         DefaultUserSettings: UserSettingsTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
         DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
         SubnetIds: Sequence[str] = ...,
-        AppNetworkAccessType: AppNetworkAccessTypeType = ...
+        AppNetworkAccessType: AppNetworkAccessTypeType = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_domain)
         """
@@ -4842,15 +4841,15 @@
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
         DeploymentConfig: DeploymentConfigTypeDef = ...,
-        RetainDeploymentConfig: bool = ...
+        RetainDeploymentConfig: bool = ...,
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the new `EndpointConfig` specified in the request, switches to using
         newly created endpoint, and then deletes resources provisioned for the endpoint
         using the previous `EndpointConfig` (there is no availability
         loss).
 
@@ -4858,15 +4857,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_endpoint)
         """
 
     async def update_endpoint_weights_and_capacities(
         self,
         *,
         EndpointName: str,
-        DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef]
+        DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef],
     ) -> UpdateEndpointWeightsAndCapacitiesOutputTypeDef:
         """
         Updates variant weight of one or more variants associated with an existing
         endpoint, or capacity of one variant associated with an existing
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint_weights_and_capacities)
@@ -4884,15 +4883,15 @@
         """
 
     async def update_feature_group(
         self,
         *,
         FeatureGroupName: str,
         FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...,
-        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...
+        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...,
     ) -> UpdateFeatureGroupResponseTypeDef:
         """
         Updates the feature group by either adding features or updating the online
         store
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_group)
@@ -4902,30 +4901,30 @@
     async def update_feature_metadata(
         self,
         *,
         FeatureGroupName: str,
         FeatureName: str,
         Description: str = ...,
         ParameterAdditions: Sequence[FeatureParameterTypeDef] = ...,
-        ParameterRemovals: Sequence[str] = ...
+        ParameterRemovals: Sequence[str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description and parameters of the feature group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_feature_metadata)
         """
 
     async def update_hub(
         self,
         *,
         HubName: str,
         HubDescription: str = ...,
         HubDisplayName: str = ...,
-        HubSearchKeywords: Sequence[str] = ...
+        HubSearchKeywords: Sequence[str] = ...,
     ) -> UpdateHubResponseTypeDef:
         """
         Update a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_hub)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_hub)
         """
@@ -4933,15 +4932,15 @@
     async def update_image(
         self,
         *,
         ImageName: str,
         DeleteProperties: Sequence[str] = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateImageResponseTypeDef:
         """
         Updates the properties of a SageMaker image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image)
         """
@@ -4956,42 +4955,42 @@
         AliasesToDelete: Sequence[str] = ...,
         VendorGuidance: VendorGuidanceType = ...,
         JobType: JobTypeType = ...,
         MLFramework: str = ...,
         ProgrammingLang: str = ...,
         Processor: ProcessorType = ...,
         Horovod: bool = ...,
-        ReleaseNotes: str = ...
+        ReleaseNotes: str = ...,
     ) -> UpdateImageVersionResponseTypeDef:
         """
         Updates the properties of a SageMaker image version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image_version)
         """
 
     async def update_inference_component(
         self,
         *,
         InferenceComponentName: str,
         Specification: InferenceComponentSpecificationTypeDef = ...,
-        RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...
+        RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...,
     ) -> UpdateInferenceComponentOutputTypeDef:
         """
         Updates an inference component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_component)
         """
 
     async def update_inference_component_runtime_config(
         self,
         *,
         InferenceComponentName: str,
-        DesiredRuntimeConfig: InferenceComponentRuntimeConfigTypeDef
+        DesiredRuntimeConfig: InferenceComponentRuntimeConfigTypeDef,
     ) -> UpdateInferenceComponentRuntimeConfigOutputTypeDef:
         """
         Runtime settings for a model that is deployed with an inference component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_component_runtime_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_component_runtime_config)
         """
@@ -5000,15 +4999,15 @@
         self,
         *,
         Name: str,
         Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
         DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigTypeDef = ...
+        ShadowModeConfig: ShadowModeConfigTypeDef = ...,
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_experiment)
         """
@@ -5029,43 +5028,43 @@
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
             AdditionalInferenceSpecificationDefinitionTypeDef
-        ] = ...
+        ] = ...,
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_model_package)
         """
 
     async def update_monitoring_alert(
         self,
         *,
         MonitoringScheduleName: str,
         MonitoringAlertName: str,
         DatapointsToAlert: int,
-        EvaluationPeriod: int
+        EvaluationPeriod: int,
     ) -> UpdateMonitoringAlertResponseTypeDef:
         """
         Update the parameters of a model monitor alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_alert)
         """
 
     async def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_schedule)
         """
@@ -5082,29 +5081,29 @@
         DefaultCodeRepository: str = ...,
         AdditionalCodeRepositories: Sequence[str] = ...,
         AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,
         DisassociateAcceleratorTypes: bool = ...,
         DisassociateDefaultCodeRepository: bool = ...,
         DisassociateAdditionalCodeRepositories: bool = ...,
         RootAccess: RootAccessType = ...,
-        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...
+        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notebook instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_notebook_instance)
         """
 
     async def update_notebook_instance_lifecycle_config(
         self,
         *,
         NotebookInstanceLifecycleConfigName: str,
         OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
-        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...
+        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notebook instance lifecycle configuration created with the
         [CreateNotebookInstanceLifecycleConfig](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html)
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance_lifecycle_config)
@@ -5116,45 +5115,45 @@
         *,
         PipelineName: str,
         PipelineDisplayName: str = ...,
         PipelineDefinition: str = ...,
         PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,
         PipelineDescription: str = ...,
         RoleArn: str = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Updates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_pipeline)
         """
 
     async def update_pipeline_execution(
         self,
         *,
         PipelineExecutionArn: str,
         PipelineExecutionDescription: str = ...,
         PipelineExecutionDisplayName: str = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> UpdatePipelineExecutionResponseTypeDef:
         """
         Updates a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_pipeline_execution)
         """
 
     async def update_project(
         self,
         *,
         ProjectName: str,
         ProjectDescription: str = ...,
         ServiceCatalogProvisioningUpdateDetails: ServiceCatalogProvisioningUpdateDetailsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Updates a machine learning (ML) project that is created from a template that
         sets up an ML pipeline from training to deploying an approved
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_project)
@@ -5163,30 +5162,30 @@
 
     async def update_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         SpaceSettings: SpaceSettingsTypeDef = ...,
-        SpaceDisplayName: str = ...
+        SpaceDisplayName: str = ...,
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_space)
         """
 
     async def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
         ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
-        ResourceConfig: ResourceConfigForUpdateTypeDef = ...
+        ResourceConfig: ResourceConfigForUpdateTypeDef = ...,
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration
         or to change warm pool retention
         length.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_training_job)
@@ -5212,15 +5211,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         ParametersToRemove: Sequence[str] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         InputArtifactsToRemove: Sequence[str] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
-        OutputArtifactsToRemove: Sequence[str] = ...
+        OutputArtifactsToRemove: Sequence[str] = ...,
     ) -> UpdateTrialComponentResponseTypeDef:
         """
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_trial_component)
         """
@@ -5237,30 +5236,30 @@
 
     async def update_workforce(
         self,
         *,
         WorkforceName: str,
         SourceIpConfig: SourceIpConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
+        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workforce)
         """
 
     async def update_workteam(
         self,
         *,
         WorkteamName: str,
         MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
         Description: str = ...,
-        NotificationConfiguration: NotificationConfigurationTypeDef = ...
+        NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workteam)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/client.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -738,15 +738,15 @@
         ActionName: str,
         Source: ActionSourceTypeDef,
         ActionType: str,
         Description: str = ...,
         Status: ActionStatusType = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateActionResponseTypeDef:
         """
         Creates an *action*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_action)
         """
@@ -756,15 +756,15 @@
         *,
         AlgorithmName: str,
         TrainingSpecification: TrainingSpecificationTypeDef,
         AlgorithmDescription: str = ...,
         InferenceSpecification: InferenceSpecificationTypeDef = ...,
         ValidationSpecification: AlgorithmValidationSpecificationTypeDef = ...,
         CertifyForMarketplace: bool = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateAlgorithmOutputTypeDef:
         """
         Create a machine learning algorithm that you can use in SageMaker and list in
         the Amazon Web Services
         Marketplace.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_algorithm)
@@ -776,30 +776,30 @@
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ResourceSpec: ResourceSpecTypeDef = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> CreateAppResponseTypeDef:
         """
         Creates a running app for the specified UserProfile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app)
         """
 
     async def create_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         Tags: Sequence[TagTypeDef] = ...,
         KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
     ) -> CreateAppImageConfigResponseTypeDef:
         """
         Creates a configuration for running a SageMaker image as a KernelGateway app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_app_image_config)
         """
@@ -808,15 +808,15 @@
         self,
         *,
         Source: ArtifactSourceTypeDef,
         ArtifactType: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateArtifactResponseTypeDef:
         """
         Creates an *artifact*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_artifact)
         """
@@ -829,15 +829,15 @@
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         RoleArn: str,
         ProblemType: ProblemTypeType = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         AutoMLJobConfig: AutoMLJobConfigTypeDef = ...,
         GenerateCandidateDefinitionsOnly: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ModelDeployConfig: ModelDeployConfigTypeDef = ...
+        ModelDeployConfig: ModelDeployConfigTypeDef = ...,
     ) -> CreateAutoMLJobResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_auto_ml_job)
         """
@@ -850,15 +850,15 @@
         OutputDataConfig: AutoMLOutputDataConfigTypeDef,
         AutoMLProblemTypeConfig: AutoMLProblemTypeConfigTypeDef,
         RoleArn: str,
         Tags: Sequence[TagTypeDef] = ...,
         SecurityConfig: AutoMLSecurityConfigTypeDef = ...,
         AutoMLJobObjective: AutoMLJobObjectiveTypeDef = ...,
         ModelDeployConfig: ModelDeployConfigTypeDef = ...,
-        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...
+        DataSplitConfig: AutoMLDataSplitConfigTypeDef = ...,
     ) -> CreateAutoMLJobV2ResponseTypeDef:
         """
         Creates an Autopilot job also referred to as Autopilot experiment or AutoML job
         V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_auto_ml_job_v2)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_auto_ml_job_v2)
@@ -866,29 +866,29 @@
 
     async def create_cluster(
         self,
         *,
         ClusterName: str,
         InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
         VpcConfig: VpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateClusterResponseTypeDef:
         """
         Creates a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_cluster)
         """
 
     async def create_code_repository(
         self,
         *,
         CodeRepositoryName: str,
         GitConfig: GitConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCodeRepositoryOutputTypeDef:
         """
         Creates a Git repository as a resource in your SageMaker account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_code_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_code_repository)
         """
@@ -899,15 +899,15 @@
         CompilationJobName: str,
         RoleArn: str,
         OutputConfig: OutputConfigTypeDef,
         StoppingCondition: StoppingConditionTypeDef,
         ModelPackageVersionArn: str = ...,
         InputConfig: InputConfigTypeDef = ...,
         VpcConfig: NeoVpcConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateCompilationJobResponseTypeDef:
         """
         Starts a model compilation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_compilation_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_compilation_job)
         """
@@ -916,15 +916,15 @@
         self,
         *,
         ContextName: str,
         Source: ContextSourceTypeDef,
         ContextType: str,
         Description: str = ...,
         Properties: Mapping[str, str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateContextResponseTypeDef:
         """
         Creates a *context*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_context)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_context)
         """
@@ -937,15 +937,15 @@
         DataQualityJobInput: DataQualityJobInputTypeDef,
         DataQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         DataQualityBaselineConfig: DataQualityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateDataQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors data quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_data_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_data_quality_job_definition)
         """
@@ -954,15 +954,15 @@
         self,
         *,
         DeviceFleetName: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         RoleArn: str = ...,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        EnableIotRoleAlias: bool = ...
+        EnableIotRoleAlias: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a device fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_device_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_device_fleet)
         """
@@ -977,15 +977,15 @@
         VpcId: str,
         Tags: Sequence[TagTypeDef] = ...,
         AppNetworkAccessType: AppNetworkAccessTypeType = ...,
         HomeEfsFileSystemKmsKeyId: str = ...,
         KmsKeyId: str = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
         DomainSettings: DomainSettingsTypeDef = ...,
-        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...
+        DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
     ) -> CreateDomainResponseTypeDef:
         """
         Creates a `Domain`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_domain)
         """
@@ -993,15 +993,15 @@
     async def create_edge_deployment_plan(
         self,
         *,
         EdgeDeploymentPlanName: str,
         ModelConfigs: Sequence[EdgeDeploymentModelConfigTypeDef],
         DeviceFleetName: str,
         Stages: Sequence[DeploymentStageTypeDef] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEdgeDeploymentPlanResponseTypeDef:
         """
         Creates an edge deployment plan, consisting of multiple stages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_edge_deployment_plan)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_edge_deployment_plan)
         """
@@ -1022,30 +1022,30 @@
         EdgePackagingJobName: str,
         CompilationJobName: str,
         ModelName: str,
         ModelVersion: str,
         RoleArn: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         ResourceKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Starts a SageMaker Edge Manager model packaging job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_edge_packaging_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_edge_packaging_job)
         """
 
     async def create_endpoint(
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         DeploymentConfig: DeploymentConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateEndpointOutputTypeDef:
         """
         Creates an endpoint using the endpoint configuration specified in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_endpoint)
         """
@@ -1059,15 +1059,15 @@
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         AsyncInferenceConfig: AsyncInferenceConfigTypeDef = ...,
         ExplainerConfig: ExplainerConfigTypeDef = ...,
         ShadowProductionVariants: Sequence[ProductionVariantTypeDef] = ...,
         ExecutionRoleArn: str = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        EnableNetworkIsolation: bool = ...
+        EnableNetworkIsolation: bool = ...,
     ) -> CreateEndpointConfigOutputTypeDef:
         """
         Creates an endpoint configuration that SageMaker hosting services uses to
         deploy
         models.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_endpoint_config)
@@ -1076,15 +1076,15 @@
 
     async def create_experiment(
         self,
         *,
         ExperimentName: str,
         DisplayName: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateExperimentResponseTypeDef:
         """
         Creates a SageMaker *experiment*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_experiment)
         """
@@ -1096,15 +1096,15 @@
         RecordIdentifierFeatureName: str,
         EventTimeFeatureName: str,
         FeatureDefinitions: Sequence[FeatureDefinitionTypeDef],
         OnlineStoreConfig: OnlineStoreConfigTypeDef = ...,
         OfflineStoreConfig: OfflineStoreConfigTypeDef = ...,
         RoleArn: str = ...,
         Description: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFeatureGroupResponseTypeDef:
         """
         Create a new `FeatureGroup`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_feature_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_feature_group)
         """
@@ -1114,15 +1114,15 @@
         *,
         FlowDefinitionName: str,
         HumanLoopConfig: HumanLoopConfigTypeDef,
         OutputConfig: FlowDefinitionOutputConfigTypeDef,
         RoleArn: str,
         HumanLoopRequestSource: HumanLoopRequestSourceTypeDef = ...,
         HumanLoopActivationConfig: HumanLoopActivationConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateFlowDefinitionResponseTypeDef:
         """
         Creates a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_flow_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_flow_definition)
         """
@@ -1131,29 +1131,29 @@
         self,
         *,
         HubName: str,
         HubDescription: str,
         HubDisplayName: str = ...,
         HubSearchKeywords: Sequence[str] = ...,
         S3StorageConfig: HubS3StorageConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHubResponseTypeDef:
         """
         Create a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hub)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_hub)
         """
 
     async def create_human_task_ui(
         self,
         *,
         HumanTaskUiName: str,
         UiTemplate: UiTemplateTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateHumanTaskUiResponseTypeDef:
         """
         Defines the settings you will use for the human review workflow user interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_human_task_ui)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_human_task_ui)
         """
@@ -1163,15 +1163,15 @@
         *,
         HyperParameterTuningJobName: str,
         HyperParameterTuningJobConfig: HyperParameterTuningJobConfigTypeDef,
         TrainingJobDefinition: HyperParameterTrainingJobDefinitionTypeDef = ...,
         TrainingJobDefinitions: Sequence[HyperParameterTrainingJobDefinitionTypeDef] = ...,
         WarmStartConfig: HyperParameterTuningJobWarmStartConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Autotune: AutotuneTypeDef = ...
+        Autotune: AutotuneTypeDef = ...,
     ) -> CreateHyperParameterTuningJobResponseTypeDef:
         """
         Starts a hyperparameter tuning job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_hyper_parameter_tuning_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_hyper_parameter_tuning_job)
         """
@@ -1179,15 +1179,15 @@
     async def create_image(
         self,
         *,
         ImageName: str,
         RoleArn: str,
         Description: str = ...,
         DisplayName: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateImageResponseTypeDef:
         """
         Creates a custom SageMaker image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_image)
         """
@@ -1201,15 +1201,15 @@
         Aliases: Sequence[str] = ...,
         VendorGuidance: VendorGuidanceType = ...,
         JobType: JobTypeType = ...,
         MLFramework: str = ...,
         ProgrammingLang: str = ...,
         Processor: ProcessorType = ...,
         Horovod: bool = ...,
-        ReleaseNotes: str = ...
+        ReleaseNotes: str = ...,
     ) -> CreateImageVersionResponseTypeDef:
         """
         Creates a version of the SageMaker image specified by `ImageName`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_image_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_image_version)
         """
@@ -1218,15 +1218,15 @@
         self,
         *,
         InferenceComponentName: str,
         EndpointName: str,
         VariantName: str,
         Specification: InferenceComponentSpecificationTypeDef,
         RuntimeConfig: InferenceComponentRuntimeConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceComponentOutputTypeDef:
         """
         Creates an inference component, which is a SageMaker hosting object that you
         can use to deploy a model to an
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_component)
@@ -1242,15 +1242,15 @@
         EndpointName: str,
         ModelVariants: Sequence[ModelVariantConfigTypeDef],
         ShadowModeConfig: ShadowModeConfigTypeDef,
         Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
         KmsKey: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceExperimentResponseTypeDef:
         """
         Creates an inference experiment using the configurations specified in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_inference_experiment)
@@ -1262,15 +1262,15 @@
         JobName: str,
         JobType: RecommendationJobTypeType,
         RoleArn: str,
         InputConfig: RecommendationJobInputConfigTypeDef,
         JobDescription: str = ...,
         StoppingConditions: RecommendationJobStoppingConditionsTypeDef = ...,
         OutputConfig: RecommendationJobOutputConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateInferenceRecommendationsJobResponseTypeDef:
         """
         Starts a recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_inference_recommendations_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_inference_recommendations_job)
         """
@@ -1283,15 +1283,15 @@
         InputConfig: LabelingJobInputConfigTypeDef,
         OutputConfig: LabelingJobOutputConfigTypeDef,
         RoleArn: str,
         HumanTaskConfig: HumanTaskConfigTypeDef,
         LabelCategoryConfigS3Uri: str = ...,
         StoppingConditions: LabelingJobStoppingConditionsTypeDef = ...,
         LabelingJobAlgorithmsConfig: LabelingJobAlgorithmsConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateLabelingJobResponseTypeDef:
         """
         Creates a job that uses workers to label the data objects in your input dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_labeling_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_labeling_job)
         """
@@ -1302,15 +1302,15 @@
         ModelName: str,
         PrimaryContainer: ContainerDefinitionTypeDef = ...,
         Containers: Sequence[ContainerDefinitionTypeDef] = ...,
         InferenceExecutionConfig: InferenceExecutionConfigTypeDef = ...,
         ExecutionRoleArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VpcConfig: VpcConfigTypeDef = ...,
-        EnableNetworkIsolation: bool = ...
+        EnableNetworkIsolation: bool = ...,
     ) -> CreateModelOutputTypeDef:
         """
         Creates a model in SageMaker.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model)
         """
@@ -1323,15 +1323,15 @@
         ModelBiasJobInput: ModelBiasJobInputTypeDef,
         ModelBiasJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelBiasBaselineConfig: ModelBiasBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelBiasJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model bias job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_bias_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_bias_job_definition)
         """
@@ -1339,30 +1339,30 @@
     async def create_model_card(
         self,
         *,
         ModelCardName: str,
         Content: str,
         ModelCardStatus: ModelCardStatusType,
         SecurityConfig: ModelCardSecurityConfigTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelCardResponseTypeDef:
         """
         Creates an Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_card)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card)
         """
 
     async def create_model_card_export_job(
         self,
         *,
         ModelCardName: str,
         ModelCardExportJobName: str,
         OutputConfig: ModelCardExportOutputConfigTypeDef,
-        ModelCardVersion: int = ...
+        ModelCardVersion: int = ...,
     ) -> CreateModelCardExportJobResponseTypeDef:
         """
         Creates an Amazon SageMaker Model Card export job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_card_export_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_card_export_job)
         """
@@ -1375,15 +1375,15 @@
         ModelExplainabilityJobInput: ModelExplainabilityJobInputTypeDef,
         ModelExplainabilityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelExplainabilityBaselineConfig: ModelExplainabilityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelExplainabilityJobDefinitionResponseTypeDef:
         """
         Creates the definition for a model explainability job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_explainability_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_explainability_job_definition)
         """
@@ -1407,15 +1407,15 @@
         DriftCheckBaselines: DriftCheckBaselinesTypeDef = ...,
         Domain: str = ...,
         Task: str = ...,
         SamplePayloadUrl: str = ...,
         AdditionalInferenceSpecifications: Sequence[
             AdditionalInferenceSpecificationDefinitionTypeDef
         ] = ...,
-        SkipModelValidation: SkipModelValidationType = ...
+        SkipModelValidation: SkipModelValidationType = ...,
     ) -> CreateModelPackageOutputTypeDef:
         """
         Creates a model package that you can use to create SageMaker models or list on
         Amazon Web Services Marketplace, or a versioned model that is part of a model
         group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package)
@@ -1423,15 +1423,15 @@
         """
 
     async def create_model_package_group(
         self,
         *,
         ModelPackageGroupName: str,
         ModelPackageGroupDescription: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelPackageGroupOutputTypeDef:
         """
         Creates a model group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_package_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_package_group)
         """
@@ -1444,29 +1444,29 @@
         ModelQualityJobInput: ModelQualityJobInputTypeDef,
         ModelQualityJobOutputConfig: MonitoringOutputConfigTypeDef,
         JobResources: MonitoringResourcesTypeDef,
         RoleArn: str,
         ModelQualityBaselineConfig: ModelQualityBaselineConfigTypeDef = ...,
         NetworkConfig: MonitoringNetworkConfigTypeDef = ...,
         StoppingCondition: MonitoringStoppingConditionTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateModelQualityJobDefinitionResponseTypeDef:
         """
         Creates a definition for a job that monitors model quality and drift.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_model_quality_job_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_model_quality_job_definition)
         """
 
     async def create_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
         MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateMonitoringScheduleResponseTypeDef:
         """
         Creates a schedule that regularly starts Amazon SageMaker Processing Jobs to
         monitor the data captured for an Amazon SageMaker
         Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_monitoring_schedule)
@@ -1487,29 +1487,29 @@
         DirectInternetAccess: DirectInternetAccessType = ...,
         VolumeSizeInGB: int = ...,
         AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,
         DefaultCodeRepository: str = ...,
         AdditionalCodeRepositories: Sequence[str] = ...,
         RootAccess: RootAccessType = ...,
         PlatformIdentifier: str = ...,
-        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...
+        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,
     ) -> CreateNotebookInstanceOutputTypeDef:
         """
         Creates an SageMaker notebook instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_notebook_instance)
         """
 
     async def create_notebook_instance_lifecycle_config(
         self,
         *,
         NotebookInstanceLifecycleConfigName: str,
         OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
-        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...
+        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
     ) -> CreateNotebookInstanceLifecycleConfigOutputTypeDef:
         """
         Creates a lifecycle configuration that you can associate with a notebook
         instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_notebook_instance_lifecycle_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_notebook_instance_lifecycle_config)
@@ -1522,15 +1522,15 @@
         ClientRequestToken: str,
         RoleArn: str,
         PipelineDisplayName: str = ...,
         PipelineDefinition: str = ...,
         PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,
         PipelineDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates a pipeline using a JSON pipeline definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_pipeline)
         """
@@ -1539,15 +1539,15 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SessionExpirationDurationInSeconds: int = ...,
         ExpiresInSeconds: int = ...,
         SpaceName: str = ...,
-        LandingUri: str = ...
+        LandingUri: str = ...,
     ) -> CreatePresignedDomainUrlResponseTypeDef:
         """
         Creates a URL for a specified UserProfile in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_presigned_domain_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_presigned_domain_url)
         """
@@ -1572,30 +1572,30 @@
         RoleArn: str,
         ProcessingInputs: Sequence[ProcessingInputTypeDef] = ...,
         ProcessingOutputConfig: ProcessingOutputConfigTypeDef = ...,
         StoppingCondition: ProcessingStoppingConditionTypeDef = ...,
         Environment: Mapping[str, str] = ...,
         NetworkConfig: NetworkConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExperimentConfig: ExperimentConfigTypeDef = ...
+        ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateProcessingJobResponseTypeDef:
         """
         Creates a processing job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_processing_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_processing_job)
         """
 
     async def create_project(
         self,
         *,
         ProjectName: str,
         ServiceCatalogProvisioningDetails: ServiceCatalogProvisioningDetailsTypeDef,
         ProjectDescription: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateProjectOutputTypeDef:
         """
         Creates a machine learning (ML) project that can contain one or more templates
         that set up an ML pipeline from training to deploying an approved
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_project)
@@ -1607,30 +1607,30 @@
         *,
         DomainId: str,
         SpaceName: str,
         Tags: Sequence[TagTypeDef] = ...,
         SpaceSettings: SpaceSettingsTypeDef = ...,
         SpaceDisplayName: str = ...,
         OwnershipSettings: OwnershipSettingsTypeDef = ...,
-        SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...
+        SpaceSharingSettings: SpaceSharingSettingsTypeDef = ...,
     ) -> CreateSpaceResponseTypeDef:
         """
         Creates a space used for real time collaboration in a Domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_space)
         """
 
     async def create_studio_lifecycle_config(
         self,
         *,
         StudioLifecycleConfigName: str,
         StudioLifecycleConfigContent: str,
         StudioLifecycleConfigAppType: StudioLifecycleConfigAppTypeType,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateStudioLifecycleConfigResponseTypeDef:
         """
         Creates a new Amazon SageMaker Studio Lifecycle Configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_studio_lifecycle_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_studio_lifecycle_config)
         """
@@ -1656,15 +1656,15 @@
         DebugRuleConfigurations: Sequence[DebugRuleConfigurationTypeDef] = ...,
         TensorBoardOutputConfig: TensorBoardOutputConfigTypeDef = ...,
         ExperimentConfig: ExperimentConfigTypeDef = ...,
         ProfilerConfig: ProfilerConfigTypeDef = ...,
         ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
         Environment: Mapping[str, str] = ...,
         RetryStrategy: RetryStrategyTypeDef = ...,
-        InfraCheckConfig: InfraCheckConfigTypeDef = ...
+        InfraCheckConfig: InfraCheckConfigTypeDef = ...,
     ) -> CreateTrainingJobResponseTypeDef:
         """
         Starts a model training job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_training_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_training_job)
         """
@@ -1681,15 +1681,15 @@
         ModelClientConfig: ModelClientConfigTypeDef = ...,
         MaxPayloadInMB: int = ...,
         BatchStrategy: BatchStrategyType = ...,
         Environment: Mapping[str, str] = ...,
         DataCaptureConfig: BatchDataCaptureConfigTypeDef = ...,
         DataProcessing: DataProcessingTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        ExperimentConfig: ExperimentConfigTypeDef = ...
+        ExperimentConfig: ExperimentConfigTypeDef = ...,
     ) -> CreateTransformJobResponseTypeDef:
         """
         Starts a transform job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_transform_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_transform_job)
         """
@@ -1697,15 +1697,15 @@
     async def create_trial(
         self,
         *,
         TrialName: str,
         ExperimentName: str,
         DisplayName: str = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrialResponseTypeDef:
         """
         Creates an SageMaker *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_trial)
         """
@@ -1718,15 +1718,15 @@
         Status: TrialComponentStatusTypeDef = ...,
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         MetadataProperties: MetadataPropertiesTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTrialComponentResponseTypeDef:
         """
         Creates a *trial component*, which is a stage of a machine learning *trial*.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_trial_component)
         """
@@ -1735,15 +1735,15 @@
         self,
         *,
         DomainId: str,
         UserProfileName: str,
         SingleSignOnUserIdentifier: str = ...,
         SingleSignOnUserValue: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        UserSettings: UserSettingsTypeDef = ...
+        UserSettings: UserSettingsTypeDef = ...,
     ) -> CreateUserProfileResponseTypeDef:
         """
         Creates a user profile.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_user_profile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_user_profile)
         """
@@ -1752,15 +1752,15 @@
         self,
         *,
         WorkforceName: str,
         CognitoConfig: CognitoConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
         SourceIpConfig: SourceIpConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
+        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> CreateWorkforceResponseTypeDef:
         """
         Use this operation to create a workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workforce)
         """
@@ -1769,15 +1769,15 @@
         self,
         *,
         WorkteamName: str,
         MemberDefinitions: Sequence[MemberDefinitionTypeDef],
         Description: str,
         WorkforceName: str = ...,
         NotificationConfiguration: NotificationConfigurationTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateWorkteamResponseTypeDef:
         """
         Creates a new work team for labeling your data.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.create_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#create_workteam)
         """
@@ -1801,15 +1801,15 @@
     async def delete_app(
         self,
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Used to stop and delete an app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_app)
         """
@@ -1975,15 +1975,15 @@
 
     async def delete_hub_content(
         self,
         *,
         HubName: str,
         HubContentType: HubContentTypeType,
         HubContentName: str,
-        HubContentVersion: str
+        HubContentVersion: str,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete the contents of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.delete_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#delete_hub_content)
         """
@@ -2255,15 +2255,15 @@
     async def describe_app(
         self,
         *,
         DomainId: str,
         AppType: AppTypeType,
         AppName: str,
         UserProfileName: str = ...,
-        SpaceName: str = ...
+        SpaceName: str = ...,
     ) -> DescribeAppResponseTypeDef:
         """
         Describes the app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#describe_app)
         """
@@ -2484,15 +2484,15 @@
 
     async def describe_hub_content(
         self,
         *,
         HubName: str,
         HubContentType: HubContentTypeType,
         HubContentName: str,
-        HubContentVersion: str = ...
+        HubContentVersion: str = ...,
     ) -> DescribeHubContentResponseTypeDef:
         """
         Describe the content of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.describe_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#describe_hub_content)
         """
@@ -2924,15 +2924,15 @@
     async def get_scaling_configuration_recommendation(
         self,
         *,
         InferenceRecommendationsJobName: str,
         RecommendationId: str = ...,
         EndpointName: str = ...,
         TargetCpuUtilizationPerCore: int = ...,
-        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...
+        ScalingPolicyObjective: ScalingPolicyObjectiveTypeDef = ...,
     ) -> GetScalingConfigurationRecommendationResponseTypeDef:
         """
         Starts an Amazon SageMaker Inference Recommender autoscaling recommendation job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.get_scaling_configuration_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#get_scaling_configuration_recommendation)
         """
@@ -2956,15 +2956,15 @@
         HubName: str,
         HubContentDocument: str,
         HubContentVersion: str = ...,
         HubContentDisplayName: str = ...,
         HubContentDescription: str = ...,
         HubContentMarkdown: str = ...,
         HubContentSearchKeywords: Sequence[str] = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> ImportHubContentResponseTypeDef:
         """
         Import hub content.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.import_hub_content)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#import_hub_content)
         """
@@ -2975,15 +2975,15 @@
         SourceUri: str = ...,
         ActionType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortActionsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListActionsResponseTypeDef:
         """
         Lists the actions in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_actions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_actions)
         """
@@ -2993,15 +2993,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: AlgorithmSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListAlgorithmsOutputTypeDef:
         """
         Lists the machine learning algorithms that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_algorithms)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_algorithms)
         """
@@ -3009,15 +3009,15 @@
     async def list_aliases(
         self,
         *,
         ImageName: str,
         Alias: str = ...,
         Version: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAliasesResponseTypeDef:
         """
         Lists the aliases of a specified image or image version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_aliases)
         """
@@ -3029,15 +3029,15 @@
         NextToken: str = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListAppImageConfigsResponseTypeDef:
         """
         Lists the AppImageConfigs in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_app_image_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_app_image_configs)
         """
@@ -3047,15 +3047,15 @@
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         DomainIdEquals: str = ...,
         UserProfileNameEquals: str = ...,
-        SpaceNameEquals: str = ...
+        SpaceNameEquals: str = ...,
     ) -> ListAppsResponseTypeDef:
         """
         Lists apps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_apps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_apps)
         """
@@ -3066,15 +3066,15 @@
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListArtifactsResponseTypeDef:
         """
         Lists the artifacts in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_artifacts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_artifacts)
         """
@@ -3088,15 +3088,15 @@
         DestinationType: str = ...,
         AssociationType: AssociationEdgeTypeType = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortAssociationsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListAssociationsResponseTypeDef:
         """
         Lists the associations in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_associations)
         """
@@ -3109,15 +3109,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: AutoMLJobStatusType = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: AutoMLSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListAutoMLJobsResponseTypeDef:
         """
         Request a list of jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_auto_ml_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_auto_ml_jobs)
         """
@@ -3127,15 +3127,15 @@
         *,
         AutoMLJobName: str,
         StatusEquals: CandidateStatusType = ...,
         CandidateNameEquals: str = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: CandidateSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListCandidatesForAutoMLJobResponseTypeDef:
         """
         List the candidates created for the job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_candidates_for_auto_ml_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_candidates_for_auto_ml_job)
         """
@@ -3146,15 +3146,15 @@
         ClusterName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         InstanceGroupNameContains: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ClusterSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListClusterNodesResponseTypeDef:
         """
         Retrieves the list of instances (also called *nodes* interchangeably) in a
         SageMaker HyperPod
         cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_cluster_nodes)
@@ -3166,15 +3166,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ClusterSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListClustersResponseTypeDef:
         """
         Retrieves the list of SageMaker HyperPod clusters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_clusters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_clusters)
         """
@@ -3186,15 +3186,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: CodeRepositorySortByType = ...,
-        SortOrder: CodeRepositorySortOrderType = ...
+        SortOrder: CodeRepositorySortOrderType = ...,
     ) -> ListCodeRepositoriesOutputTypeDef:
         """
         Gets a list of the Git repositories in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_code_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_code_repositories)
         """
@@ -3207,15 +3207,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: CompilationJobStatusType = ...,
         SortBy: ListCompilationJobsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListCompilationJobsResponseTypeDef:
         """
         Lists model compilation jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_compilation_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_compilation_jobs)
         """
@@ -3226,15 +3226,15 @@
         SourceUri: str = ...,
         ContextType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortContextsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListContextsResponseTypeDef:
         """
         Lists the contexts in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_contexts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_contexts)
         """
@@ -3245,15 +3245,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListDataQualityJobDefinitionsResponseTypeDef:
         """
         Lists the data quality job definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_data_quality_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_data_quality_job_definitions)
         """
@@ -3265,15 +3265,15 @@
         MaxResults: int = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ListDeviceFleetsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListDeviceFleetsResponseTypeDef:
         """
         Returns a list of devices in the fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_device_fleets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_device_fleets)
         """
@@ -3281,15 +3281,15 @@
     async def list_devices(
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         LatestHeartbeatAfter: TimestampTypeDef = ...,
         ModelName: str = ...,
-        DeviceFleetName: str = ...
+        DeviceFleetName: str = ...,
     ) -> ListDevicesResponseTypeDef:
         """
         A list of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_devices)
         """
@@ -3312,15 +3312,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         DeviceFleetNameContains: str = ...,
         SortBy: ListEdgeDeploymentPlansSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListEdgeDeploymentPlansResponseTypeDef:
         """
         Lists all edge deployment plans.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_edge_deployment_plans)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_edge_deployment_plans)
         """
@@ -3334,15 +3334,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelNameContains: str = ...,
         StatusEquals: EdgePackagingJobStatusType = ...,
         SortBy: ListEdgePackagingJobsSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListEdgePackagingJobsResponseTypeDef:
         """
         Returns a list of edge packaging jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_edge_packaging_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_edge_packaging_jobs)
         """
@@ -3352,15 +3352,15 @@
         *,
         SortBy: EndpointConfigSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListEndpointConfigsOutputTypeDef:
         """
         Lists endpoint configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoint_configs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_endpoint_configs)
         """
@@ -3373,15 +3373,15 @@
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
-        StatusEquals: EndpointStatusType = ...
+        StatusEquals: EndpointStatusType = ...,
     ) -> ListEndpointsOutputTypeDef:
         """
         Lists endpoints.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_endpoints)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_endpoints)
         """
@@ -3390,15 +3390,15 @@
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListExperimentsResponseTypeDef:
         """
         Lists all the experiments in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_experiments)
         """
@@ -3410,15 +3410,15 @@
         FeatureGroupStatusEquals: FeatureGroupStatusType = ...,
         OfflineStoreStatusEquals: OfflineStoreStatusValueType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListFeatureGroupsResponseTypeDef:
         """
         List `FeatureGroup`s based on given filter and order.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_feature_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_feature_groups)
         """
@@ -3426,15 +3426,15 @@
     async def list_flow_definitions(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListFlowDefinitionsResponseTypeDef:
         """
         Returns information about the flow definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_flow_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_flow_definitions)
         """
@@ -3448,15 +3448,15 @@
         MinVersion: str = ...,
         MaxSchemaVersion: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         SortBy: HubContentSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubContentVersionsResponseTypeDef:
         """
         List hub content versions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hub_content_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hub_content_versions)
         """
@@ -3469,15 +3469,15 @@
         NameContains: str = ...,
         MaxSchemaVersion: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         SortBy: HubContentSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubContentsResponseTypeDef:
         """
         List the contents of a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hub_contents)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hub_contents)
         """
@@ -3489,15 +3489,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: HubSortByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListHubsResponseTypeDef:
         """
         List all existing hubs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_hubs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_hubs)
         """
@@ -3505,15 +3505,15 @@
     async def list_human_task_uis(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListHumanTaskUisResponseTypeDef:
         """
         Returns information about the human task user interfaces in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_human_task_uis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_human_task_uis)
         """
@@ -3526,15 +3526,15 @@
         SortBy: HyperParameterTuningJobSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
-        StatusEquals: HyperParameterTuningJobStatusType = ...
+        StatusEquals: HyperParameterTuningJobStatusType = ...,
     ) -> ListHyperParameterTuningJobsResponseTypeDef:
         """
         Gets a list of
         [HyperParameterTuningJobSummary](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_HyperParameterTuningJobSummary.html)
         objects that describe the hyperparameter tuning jobs launched in your
         account.
 
@@ -3549,15 +3549,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         SortBy: ImageVersionSortByType = ...,
-        SortOrder: ImageVersionSortOrderType = ...
+        SortOrder: ImageVersionSortOrderType = ...,
     ) -> ListImageVersionsResponseTypeDef:
         """
         Lists the versions of a specified image and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_image_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_image_versions)
         """
@@ -3569,15 +3569,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ImageSortByType = ...,
-        SortOrder: ImageSortOrderType = ...
+        SortOrder: ImageSortOrderType = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Lists the images in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_images)
         """
@@ -3592,15 +3592,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: InferenceComponentStatusType = ...,
         EndpointNameEquals: str = ...,
-        VariantNameEquals: str = ...
+        VariantNameEquals: str = ...,
     ) -> ListInferenceComponentsOutputTypeDef:
         """
         Lists the inference components in your account and their properties.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_components)
         """
@@ -3614,15 +3614,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListInferenceExperimentsResponseTypeDef:
         """
         Returns the list of all inference experiments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_experiments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_experiments)
         """
@@ -3630,15 +3630,15 @@
     async def list_inference_recommendations_job_steps(
         self,
         *,
         JobName: str,
         Status: RecommendationJobStatusType = ...,
         StepType: Literal["BENCHMARK"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListInferenceRecommendationsJobStepsResponseTypeDef:
         """
         Returns a list of the subtasks for an Inference Recommender job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_recommendations_job_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_recommendations_job_steps)
         """
@@ -3653,15 +3653,15 @@
         NameContains: str = ...,
         StatusEquals: RecommendationJobStatusType = ...,
         SortBy: ListInferenceRecommendationsJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         ModelNameEquals: str = ...,
-        ModelPackageVersionArnEquals: str = ...
+        ModelPackageVersionArnEquals: str = ...,
     ) -> ListInferenceRecommendationsJobsResponseTypeDef:
         """
         Lists recommendation jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_inference_recommendations_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_inference_recommendations_jobs)
         """
@@ -3674,15 +3674,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        StatusEquals: LabelingJobStatusType = ...
+        StatusEquals: LabelingJobStatusType = ...,
     ) -> ListLabelingJobsResponseTypeDef:
         """
         Gets a list of labeling jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_labeling_jobs)
         """
@@ -3693,15 +3693,15 @@
         WorkteamArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         JobReferenceCodeContains: str = ...,
         SortBy: Literal["CreationTime"] = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListLabelingJobsForWorkteamResponseTypeDef:
         """
         Gets a list of labeling jobs assigned to a specified work team.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_labeling_jobs_for_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_labeling_jobs_for_workteam)
         """
@@ -3710,15 +3710,15 @@
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortLineageGroupsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListLineageGroupsResponseTypeDef:
         """
         A list of lineage groups shared with your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_lineage_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_lineage_groups)
         """
@@ -3729,15 +3729,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelBiasJobDefinitionsResponseTypeDef:
         """
         Lists model bias jobs definitions that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_bias_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_bias_job_definitions)
         """
@@ -3750,15 +3750,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardExportJobNameContains: str = ...,
         StatusEquals: ModelCardExportJobStatusType = ...,
         SortBy: ModelCardExportJobSortByType = ...,
         SortOrder: ModelCardExportJobSortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListModelCardExportJobsResponseTypeDef:
         """
         List the export jobs for the Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_card_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_card_export_jobs)
         """
@@ -3769,15 +3769,15 @@
         ModelCardName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         NextToken: str = ...,
         SortBy: Literal["Version"] = ...,
-        SortOrder: ModelCardSortOrderType = ...
+        SortOrder: ModelCardSortOrderType = ...,
     ) -> ListModelCardVersionsResponseTypeDef:
         """
         List existing versions of an Amazon SageMaker Model Card.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_card_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_card_versions)
         """
@@ -3788,15 +3788,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         NextToken: str = ...,
         SortBy: ModelCardSortByType = ...,
-        SortOrder: ModelCardSortOrderType = ...
+        SortOrder: ModelCardSortOrderType = ...,
     ) -> ListModelCardsResponseTypeDef:
         """
         List existing model cards.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_cards)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_cards)
         """
@@ -3807,29 +3807,29 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelExplainabilityJobDefinitionsResponseTypeDef:
         """
         Lists model explainability job definitions that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_explainability_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_explainability_job_definitions)
         """
 
     async def list_model_metadata(
         self,
         *,
         SearchExpression: ModelMetadataSearchExpressionTypeDef = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListModelMetadataResponseTypeDef:
         """
         Lists the domain, framework, task, and model name of standard machine learning
         models found in common model
         zoos.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_metadata)
@@ -3841,15 +3841,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ModelPackageGroupSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListModelPackageGroupsOutputTypeDef:
         """
         Gets a list of the model groups in your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_package_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_package_groups)
         """
@@ -3862,15 +3862,15 @@
         MaxResults: int = ...,
         NameContains: str = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageType: ModelPackageTypeType = ...,
         NextToken: str = ...,
         SortBy: ModelPackageSortByType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListModelPackagesOutputTypeDef:
         """
         Lists the model packages that have been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_packages)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_packages)
         """
@@ -3881,15 +3881,15 @@
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelQualityJobDefinitionsResponseTypeDef:
         """
         Gets a list of model quality monitoring job definitions in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_model_quality_job_definitions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_model_quality_job_definitions)
         """
@@ -3899,15 +3899,15 @@
         *,
         SortBy: ModelSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
-        CreationTimeAfter: TimestampTypeDef = ...
+        CreationTimeAfter: TimestampTypeDef = ...,
     ) -> ListModelsOutputTypeDef:
         """
         Lists models created with the `CreateModel` API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_models)
         """
@@ -3919,15 +3919,15 @@
         MonitoringAlertName: str = ...,
         SortBy: MonitoringAlertHistorySortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        StatusEquals: MonitoringAlertStatusType = ...
+        StatusEquals: MonitoringAlertStatusType = ...,
     ) -> ListMonitoringAlertHistoryResponseTypeDef:
         """
         Gets a list of past alerts in a model monitoring schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_alert_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_alert_history)
         """
@@ -3955,15 +3955,15 @@
         ScheduledTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ExecutionStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
-        MonitoringTypeEquals: MonitoringTypeType = ...
+        MonitoringTypeEquals: MonitoringTypeType = ...,
     ) -> ListMonitoringExecutionsResponseTypeDef:
         """
         Returns list of all monitoring job executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_executions)
         """
@@ -3979,15 +3979,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ScheduleStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
-        MonitoringTypeEquals: MonitoringTypeType = ...
+        MonitoringTypeEquals: MonitoringTypeType = ...,
     ) -> ListMonitoringSchedulesResponseTypeDef:
         """
         Returns list of all monitoring schedules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_monitoring_schedules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_monitoring_schedules)
         """
@@ -3999,15 +3999,15 @@
         MaxResults: int = ...,
         SortBy: NotebookInstanceLifecycleConfigSortKeyType = ...,
         SortOrder: NotebookInstanceLifecycleConfigSortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
-        LastModifiedTimeAfter: TimestampTypeDef = ...
+        LastModifiedTimeAfter: TimestampTypeDef = ...,
     ) -> ListNotebookInstanceLifecycleConfigsOutputTypeDef:
         """
         Lists notebook instance lifestyle configurations created with the
         [CreateNotebookInstanceLifecycleConfig](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html)
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instance_lifecycle_configs)
@@ -4025,15 +4025,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: NotebookInstanceStatusType = ...,
         NotebookInstanceLifecycleConfigNameContains: str = ...,
         DefaultCodeRepositoryContains: str = ...,
-        AdditionalCodeRepositoryEquals: str = ...
+        AdditionalCodeRepositoryEquals: str = ...,
     ) -> ListNotebookInstancesOutputTypeDef:
         """
         Returns a list of the SageMaker notebook instances in the requester's account
         in an Amazon Web Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_notebook_instances)
@@ -4042,15 +4042,15 @@
 
     async def list_pipeline_execution_steps(
         self,
         *,
         PipelineExecutionArn: str = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListPipelineExecutionStepsResponseTypeDef:
         """
         Gets a list of `PipeLineExecutionStep` objects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_execution_steps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipeline_execution_steps)
         """
@@ -4060,15 +4060,15 @@
         *,
         PipelineName: str,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelineExecutionsByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPipelineExecutionsResponseTypeDef:
         """
         Gets a list of the pipeline executions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipeline_executions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipeline_executions)
         """
@@ -4088,15 +4088,15 @@
         *,
         PipelineNamePrefix: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelinesByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListPipelinesResponseTypeDef:
         """
         Gets a list of pipelines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_pipelines)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_pipelines)
         """
@@ -4109,15 +4109,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: ProcessingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListProcessingJobsResponseTypeDef:
         """
         Lists processing jobs that satisfy various filters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_processing_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_processing_jobs)
         """
@@ -4127,15 +4127,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         MaxResults: int = ...,
         NameContains: str = ...,
         NextToken: str = ...,
         SortBy: ProjectSortByType = ...,
-        SortOrder: ProjectSortOrderType = ...
+        SortOrder: ProjectSortOrderType = ...,
     ) -> ListProjectsOutputTypeDef:
         """
         Gets a list of the projects in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_projects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_projects)
         """
@@ -4145,15 +4145,15 @@
         *,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: ResourceCatalogSortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListResourceCatalogsResponseTypeDef:
         """
         Lists Amazon SageMaker Catalogs based on given filters and orders.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_resource_catalogs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_resource_catalogs)
         """
@@ -4162,15 +4162,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
         DomainIdEquals: str = ...,
-        SpaceNameContains: str = ...
+        SpaceNameContains: str = ...,
     ) -> ListSpacesResponseTypeDef:
         """
         Lists spaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_spaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_spaces)
         """
@@ -4178,15 +4178,15 @@
     async def list_stage_devices(
         self,
         *,
         EdgeDeploymentPlanName: str,
         StageName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
-        ExcludeDevicesDeployedInOtherStage: bool = ...
+        ExcludeDevicesDeployedInOtherStage: bool = ...,
     ) -> ListStageDevicesResponseTypeDef:
         """
         Lists devices allocated to the stage, containing detailed device information
         and deployment
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_stage_devices)
@@ -4201,15 +4201,15 @@
         NameContains: str = ...,
         AppTypeEquals: StudioLifecycleConfigAppTypeType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: StudioLifecycleConfigSortKeyType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListStudioLifecycleConfigsResponseTypeDef:
         """
         Lists the Amazon SageMaker Studio Lifecycle Configurations in your Amazon Web
         Services
         Account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_studio_lifecycle_configs)
@@ -4247,15 +4247,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        WarmPoolStatusEquals: WarmPoolResourceStatusType = ...
+        WarmPoolStatusEquals: WarmPoolResourceStatusType = ...,
     ) -> ListTrainingJobsResponseTypeDef:
         """
         Lists training jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_training_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_training_jobs)
         """
@@ -4264,15 +4264,15 @@
         self,
         *,
         HyperParameterTuningJobName: str,
         NextToken: str = ...,
         MaxResults: int = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: TrainingJobSortByOptionsType = ...,
-        SortOrder: SortOrderType = ...
+        SortOrder: SortOrderType = ...,
     ) -> ListTrainingJobsForHyperParameterTuningJobResponseTypeDef:
         """
         Gets a list of
         [TrainingJobSummary](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_TrainingJobSummary.html)
         objects that describe the training jobs that a hyperparameter tuning job
         launched.
 
@@ -4288,15 +4288,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TransformJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListTransformJobsResponseTypeDef:
         """
         Lists transform jobs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_transform_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_transform_jobs)
         """
@@ -4308,15 +4308,15 @@
         TrialName: str = ...,
         SourceArn: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialComponentsByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTrialComponentsResponseTypeDef:
         """
         Lists the trial components in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trial_components)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_trial_components)
         """
@@ -4327,15 +4327,15 @@
         ExperimentName: str = ...,
         TrialComponentName: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialsByType = ...,
         SortOrder: SortOrderType = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> ListTrialsResponseTypeDef:
         """
         Lists the trials in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_trials)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_trials)
         """
@@ -4344,15 +4344,15 @@
         self,
         *,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortOrder: SortOrderType = ...,
         SortBy: UserProfileSortKeyType = ...,
         DomainIdEquals: str = ...,
-        UserProfileNameContains: str = ...
+        UserProfileNameContains: str = ...,
     ) -> ListUserProfilesResponseTypeDef:
         """
         Lists user profiles.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_user_profiles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_user_profiles)
         """
@@ -4360,15 +4360,15 @@
     async def list_workforces(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkforcesResponseTypeDef:
         """
         Use this operation to list all private and vendor workforces in an Amazon Web
         Services
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workforces)
@@ -4378,15 +4378,15 @@
     async def list_workteams(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         NextToken: str = ...,
-        MaxResults: int = ...
+        MaxResults: int = ...,
     ) -> ListWorkteamsResponseTypeDef:
         """
         Gets a list of private work teams that you have defined in a region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.list_workteams)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#list_workteams)
         """
@@ -4406,59 +4406,59 @@
         *,
         StartArns: Sequence[str] = ...,
         Direction: DirectionType = ...,
         IncludeEdges: bool = ...,
         Filters: QueryFiltersTypeDef = ...,
         MaxDepth: int = ...,
         MaxResults: int = ...,
-        NextToken: str = ...
+        NextToken: str = ...,
     ) -> QueryLineageResponseTypeDef:
         """
         Use this action to inspect your lineage and discover relationships between
         entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.query_lineage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#query_lineage)
         """
 
     async def register_devices(
         self,
         *,
         DeviceFleetName: str,
         Devices: Sequence[DeviceTypeDef],
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Register devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.register_devices)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#register_devices)
         """
 
     async def render_ui_template(
         self,
         *,
         Task: RenderableTaskTypeDef,
         RoleArn: str,
         UiTemplate: UiTemplateTypeDef = ...,
-        HumanTaskUiArn: str = ...
+        HumanTaskUiArn: str = ...,
     ) -> RenderUiTemplateResponseTypeDef:
         """
         Renders the UI template so that you can preview the worker's experience.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.render_ui_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#render_ui_template)
         """
 
     async def retry_pipeline_execution(
         self,
         *,
         PipelineExecutionArn: str,
         ClientRequestToken: str,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> RetryPipelineExecutionResponseTypeDef:
         """
         Retry the execution of the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.retry_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#retry_pipeline_execution)
         """
@@ -4468,15 +4468,15 @@
         *,
         Resource: ResourceTypeType,
         SearchExpression: "SearchExpressionTypeDef" = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
-        CrossAccountFilterOption: CrossAccountFilterOptionType = ...
+        CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
     ) -> SearchResponseTypeDef:
         """
         Finds SageMaker resources that match a search query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.search)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#search)
         """
@@ -4494,15 +4494,15 @@
         """
 
     async def send_pipeline_execution_step_success(
         self,
         *,
         CallbackToken: str,
         OutputParameters: Sequence[OutputParameterTypeDef] = ...,
-        ClientRequestToken: str = ...
+        ClientRequestToken: str = ...,
     ) -> SendPipelineExecutionStepSuccessResponseTypeDef:
         """
         Notifies the pipeline that the execution of a callback step succeeded and
         provides a list of the step's output
         parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.send_pipeline_execution_step_success)
@@ -4556,15 +4556,15 @@
         *,
         PipelineName: str,
         ClientRequestToken: str,
         PipelineExecutionDisplayName: str = ...,
         PipelineParameters: Sequence[ParameterTypeDef] = ...,
         PipelineExecutionDescription: str = ...,
         ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
-        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...
+        SelectiveExecutionConfig: SelectiveExecutionConfigTypeDef = ...,
     ) -> StartPipelineExecutionResponseTypeDef:
         """
         Starts a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.start_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#start_pipeline_execution)
         """
@@ -4622,15 +4622,15 @@
     async def stop_inference_experiment(
         self,
         *,
         Name: str,
         ModelVariantActions: Mapping[str, ModelVariantActionType],
         DesiredModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
         DesiredState: InferenceExperimentStopDesiredStateType = ...,
-        Reason: str = ...
+        Reason: str = ...,
     ) -> StopInferenceExperimentResponseTypeDef:
         """
         Stops an inference experiment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.stop_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#stop_inference_experiment)
         """
@@ -4710,57 +4710,57 @@
     async def update_action(
         self,
         *,
         ActionName: str,
         Description: str = ...,
         Status: ActionStatusType = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateActionResponseTypeDef:
         """
         Updates an action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_action)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_action)
         """
 
     async def update_app_image_config(
         self,
         *,
         AppImageConfigName: str,
         KernelGatewayImageConfig: KernelGatewayImageConfigTypeDef = ...,
-        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...
+        JupyterLabAppImageConfig: JupyterLabAppImageConfigTypeDef = ...,
     ) -> UpdateAppImageConfigResponseTypeDef:
         """
         Updates the properties of an AppImageConfig.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_app_image_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_app_image_config)
         """
 
     async def update_artifact(
         self,
         *,
         ArtifactArn: str,
         ArtifactName: str = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateArtifactResponseTypeDef:
         """
         Updates an artifact.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_artifact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_artifact)
         """
 
     async def update_cluster(
         self,
         *,
         ClusterName: str,
-        InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef]
+        InstanceGroups: Sequence[ClusterInstanceGroupSpecificationTypeDef],
     ) -> UpdateClusterResponseTypeDef:
         """
         Update a SageMaker HyperPod cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_cluster)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_cluster)
         """
@@ -4777,15 +4777,15 @@
 
     async def update_context(
         self,
         *,
         ContextName: str,
         Description: str = ...,
         Properties: Mapping[str, str] = ...,
-        PropertiesToRemove: Sequence[str] = ...
+        PropertiesToRemove: Sequence[str] = ...,
     ) -> UpdateContextResponseTypeDef:
         """
         Updates a context.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_context)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_context)
         """
@@ -4793,15 +4793,15 @@
     async def update_device_fleet(
         self,
         *,
         DeviceFleetName: str,
         OutputConfig: EdgeOutputConfigTypeDef,
         RoleArn: str = ...,
         Description: str = ...,
-        EnableIotRoleAlias: bool = ...
+        EnableIotRoleAlias: bool = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates a fleet of devices.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_device_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_device_fleet)
         """
@@ -4821,15 +4821,15 @@
         *,
         DomainId: str,
         DefaultUserSettings: UserSettingsTypeDef = ...,
         DomainSettingsForUpdate: DomainSettingsForUpdateTypeDef = ...,
         DefaultSpaceSettings: DefaultSpaceSettingsTypeDef = ...,
         AppSecurityGroupManagement: AppSecurityGroupManagementType = ...,
         SubnetIds: Sequence[str] = ...,
-        AppNetworkAccessType: AppNetworkAccessTypeType = ...
+        AppNetworkAccessType: AppNetworkAccessTypeType = ...,
     ) -> UpdateDomainResponseTypeDef:
         """
         Updates the default settings for new user profiles in the domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_domain)
         """
@@ -4838,15 +4838,15 @@
         self,
         *,
         EndpointName: str,
         EndpointConfigName: str,
         RetainAllVariantProperties: bool = ...,
         ExcludeRetainedVariantProperties: Sequence[VariantPropertyTypeDef] = ...,
         DeploymentConfig: DeploymentConfigTypeDef = ...,
-        RetainDeploymentConfig: bool = ...
+        RetainDeploymentConfig: bool = ...,
     ) -> UpdateEndpointOutputTypeDef:
         """
         Deploys the new `EndpointConfig` specified in the request, switches to using
         newly created endpoint, and then deletes resources provisioned for the endpoint
         using the previous `EndpointConfig` (there is no availability
         loss).
 
@@ -4854,15 +4854,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_endpoint)
         """
 
     async def update_endpoint_weights_and_capacities(
         self,
         *,
         EndpointName: str,
-        DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef]
+        DesiredWeightsAndCapacities: Sequence[DesiredWeightAndCapacityTypeDef],
     ) -> UpdateEndpointWeightsAndCapacitiesOutputTypeDef:
         """
         Updates variant weight of one or more variants associated with an existing
         endpoint, or capacity of one variant associated with an existing
         endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_endpoint_weights_and_capacities)
@@ -4880,15 +4880,15 @@
         """
 
     async def update_feature_group(
         self,
         *,
         FeatureGroupName: str,
         FeatureAdditions: Sequence[FeatureDefinitionTypeDef] = ...,
-        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...
+        OnlineStoreConfig: OnlineStoreConfigUpdateTypeDef = ...,
     ) -> UpdateFeatureGroupResponseTypeDef:
         """
         Updates the feature group by either adding features or updating the online
         store
         configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_group)
@@ -4898,30 +4898,30 @@
     async def update_feature_metadata(
         self,
         *,
         FeatureGroupName: str,
         FeatureName: str,
         Description: str = ...,
         ParameterAdditions: Sequence[FeatureParameterTypeDef] = ...,
-        ParameterRemovals: Sequence[str] = ...
+        ParameterRemovals: Sequence[str] = ...,
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description and parameters of the feature group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_feature_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_feature_metadata)
         """
 
     async def update_hub(
         self,
         *,
         HubName: str,
         HubDescription: str = ...,
         HubDisplayName: str = ...,
-        HubSearchKeywords: Sequence[str] = ...
+        HubSearchKeywords: Sequence[str] = ...,
     ) -> UpdateHubResponseTypeDef:
         """
         Update a hub.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_hub)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_hub)
         """
@@ -4929,15 +4929,15 @@
     async def update_image(
         self,
         *,
         ImageName: str,
         DeleteProperties: Sequence[str] = ...,
         Description: str = ...,
         DisplayName: str = ...,
-        RoleArn: str = ...
+        RoleArn: str = ...,
     ) -> UpdateImageResponseTypeDef:
         """
         Updates the properties of a SageMaker image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image)
         """
@@ -4952,42 +4952,42 @@
         AliasesToDelete: Sequence[str] = ...,
         VendorGuidance: VendorGuidanceType = ...,
         JobType: JobTypeType = ...,
         MLFramework: str = ...,
         ProgrammingLang: str = ...,
         Processor: ProcessorType = ...,
         Horovod: bool = ...,
-        ReleaseNotes: str = ...
+        ReleaseNotes: str = ...,
     ) -> UpdateImageVersionResponseTypeDef:
         """
         Updates the properties of a SageMaker image version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_image_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_image_version)
         """
 
     async def update_inference_component(
         self,
         *,
         InferenceComponentName: str,
         Specification: InferenceComponentSpecificationTypeDef = ...,
-        RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...
+        RuntimeConfig: InferenceComponentRuntimeConfigTypeDef = ...,
     ) -> UpdateInferenceComponentOutputTypeDef:
         """
         Updates an inference component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_component)
         """
 
     async def update_inference_component_runtime_config(
         self,
         *,
         InferenceComponentName: str,
-        DesiredRuntimeConfig: InferenceComponentRuntimeConfigTypeDef
+        DesiredRuntimeConfig: InferenceComponentRuntimeConfigTypeDef,
     ) -> UpdateInferenceComponentRuntimeConfigOutputTypeDef:
         """
         Runtime settings for a model that is deployed with an inference component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_component_runtime_config)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_component_runtime_config)
         """
@@ -4996,15 +4996,15 @@
         self,
         *,
         Name: str,
         Schedule: InferenceExperimentScheduleTypeDef = ...,
         Description: str = ...,
         ModelVariants: Sequence[ModelVariantConfigTypeDef] = ...,
         DataStorageConfig: InferenceExperimentDataStorageConfigTypeDef = ...,
-        ShadowModeConfig: ShadowModeConfigTypeDef = ...
+        ShadowModeConfig: ShadowModeConfigTypeDef = ...,
     ) -> UpdateInferenceExperimentResponseTypeDef:
         """
         Updates an inference experiment that you created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_inference_experiment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_inference_experiment)
         """
@@ -5025,43 +5025,43 @@
         ModelPackageArn: str,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ApprovalDescription: str = ...,
         CustomerMetadataProperties: Mapping[str, str] = ...,
         CustomerMetadataPropertiesToRemove: Sequence[str] = ...,
         AdditionalInferenceSpecificationsToAdd: Sequence[
             AdditionalInferenceSpecificationDefinitionTypeDef
-        ] = ...
+        ] = ...,
     ) -> UpdateModelPackageOutputTypeDef:
         """
         Updates a versioned model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_model_package)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_model_package)
         """
 
     async def update_monitoring_alert(
         self,
         *,
         MonitoringScheduleName: str,
         MonitoringAlertName: str,
         DatapointsToAlert: int,
-        EvaluationPeriod: int
+        EvaluationPeriod: int,
     ) -> UpdateMonitoringAlertResponseTypeDef:
         """
         Update the parameters of a model monitor alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_alert)
         """
 
     async def update_monitoring_schedule(
         self,
         *,
         MonitoringScheduleName: str,
-        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef
+        MonitoringScheduleConfig: MonitoringScheduleConfigTypeDef,
     ) -> UpdateMonitoringScheduleResponseTypeDef:
         """
         Updates a previously created schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_monitoring_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_monitoring_schedule)
         """
@@ -5078,29 +5078,29 @@
         DefaultCodeRepository: str = ...,
         AdditionalCodeRepositories: Sequence[str] = ...,
         AcceleratorTypes: Sequence[NotebookInstanceAcceleratorTypeType] = ...,
         DisassociateAcceleratorTypes: bool = ...,
         DisassociateDefaultCodeRepository: bool = ...,
         DisassociateAdditionalCodeRepositories: bool = ...,
         RootAccess: RootAccessType = ...,
-        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...
+        InstanceMetadataServiceConfiguration: InstanceMetadataServiceConfigurationTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notebook instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_notebook_instance)
         """
 
     async def update_notebook_instance_lifecycle_config(
         self,
         *,
         NotebookInstanceLifecycleConfigName: str,
         OnCreate: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
-        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...
+        OnStart: Sequence[NotebookInstanceLifecycleHookTypeDef] = ...,
     ) -> Dict[str, Any]:
         """
         Updates a notebook instance lifecycle configuration created with the
         [CreateNotebookInstanceLifecycleConfig](https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_CreateNotebookInstanceLifecycleConfig.html)
         API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_notebook_instance_lifecycle_config)
@@ -5112,45 +5112,45 @@
         *,
         PipelineName: str,
         PipelineDisplayName: str = ...,
         PipelineDefinition: str = ...,
         PipelineDefinitionS3Location: PipelineDefinitionS3LocationTypeDef = ...,
         PipelineDescription: str = ...,
         RoleArn: str = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> UpdatePipelineResponseTypeDef:
         """
         Updates a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_pipeline)
         """
 
     async def update_pipeline_execution(
         self,
         *,
         PipelineExecutionArn: str,
         PipelineExecutionDescription: str = ...,
         PipelineExecutionDisplayName: str = ...,
-        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...
+        ParallelismConfiguration: ParallelismConfigurationTypeDef = ...,
     ) -> UpdatePipelineExecutionResponseTypeDef:
         """
         Updates a pipeline execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_pipeline_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_pipeline_execution)
         """
 
     async def update_project(
         self,
         *,
         ProjectName: str,
         ProjectDescription: str = ...,
         ServiceCatalogProvisioningUpdateDetails: ServiceCatalogProvisioningUpdateDetailsTypeDef = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
     ) -> UpdateProjectOutputTypeDef:
         """
         Updates a machine learning (ML) project that is created from a template that
         sets up an ML pipeline from training to deploying an approved
         model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_project)
@@ -5159,30 +5159,30 @@
 
     async def update_space(
         self,
         *,
         DomainId: str,
         SpaceName: str,
         SpaceSettings: SpaceSettingsTypeDef = ...,
-        SpaceDisplayName: str = ...
+        SpaceDisplayName: str = ...,
     ) -> UpdateSpaceResponseTypeDef:
         """
         Updates the settings of a space.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_space)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_space)
         """
 
     async def update_training_job(
         self,
         *,
         TrainingJobName: str,
         ProfilerConfig: ProfilerConfigForUpdateTypeDef = ...,
         ProfilerRuleConfigurations: Sequence[ProfilerRuleConfigurationTypeDef] = ...,
-        ResourceConfig: ResourceConfigForUpdateTypeDef = ...
+        ResourceConfig: ResourceConfigForUpdateTypeDef = ...,
     ) -> UpdateTrainingJobResponseTypeDef:
         """
         Update a model training job to request a new Debugger profiling configuration
         or to change warm pool retention
         length.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_training_job)
@@ -5208,15 +5208,15 @@
         StartTime: TimestampTypeDef = ...,
         EndTime: TimestampTypeDef = ...,
         Parameters: Mapping[str, TrialComponentParameterValueTypeDef] = ...,
         ParametersToRemove: Sequence[str] = ...,
         InputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
         InputArtifactsToRemove: Sequence[str] = ...,
         OutputArtifacts: Mapping[str, TrialComponentArtifactTypeDef] = ...,
-        OutputArtifactsToRemove: Sequence[str] = ...
+        OutputArtifactsToRemove: Sequence[str] = ...,
     ) -> UpdateTrialComponentResponseTypeDef:
         """
         Updates one or more properties of a trial component.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_trial_component)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_trial_component)
         """
@@ -5233,30 +5233,30 @@
 
     async def update_workforce(
         self,
         *,
         WorkforceName: str,
         SourceIpConfig: SourceIpConfigTypeDef = ...,
         OidcConfig: OidcConfigTypeDef = ...,
-        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...
+        WorkforceVpcConfig: WorkforceVpcConfigRequestTypeDef = ...,
     ) -> UpdateWorkforceResponseTypeDef:
         """
         Use this operation to update your workforce.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workforce)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workforce)
         """
 
     async def update_workteam(
         self,
         *,
         WorkteamName: str,
         MemberDefinitions: Sequence[MemberDefinitionTypeDef] = ...,
         Description: str = ...,
-        NotificationConfiguration: NotificationConfigurationTypeDef = ...
+        NotificationConfiguration: NotificationConfigurationTypeDef = ...,
     ) -> UpdateWorkteamResponseTypeDef:
         """
         Updates an existing work team with new member definitions or description.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Client.update_workteam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/client/#update_workteam)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/literals.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/literals.py`

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
     "ActionStatusType",
     "AdditionalS3DataSourceDataTypeType",
     "AggregationTransformationValueType",
     "AlgorithmSortByType",
     "AlgorithmStatusType",
     "AppImageConfigSortKeyType",
@@ -372,15 +371,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 ActionStatusType = Literal["Completed", "Failed", "InProgress", "Stopped", "Stopping", "Unknown"]
 AdditionalS3DataSourceDataTypeType = Literal["S3Object"]
 AggregationTransformationValueType = Literal["avg", "first", "max", "min", "sum"]
 AlgorithmSortByType = Literal["CreationTime", "Name"]
 AlgorithmStatusType = Literal["Completed", "Deleting", "Failed", "InProgress", "Pending"]
 AppImageConfigSortKeyType = Literal["CreationTime", "LastModifiedTime", "Name"]
 AppInstanceTypeType = Literal[
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/literals.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/paginator.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -339,15 +339,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListActionsPaginator",
     "ListAlgorithmsPaginator",
     "ListAliasesPaginator",
     "ListAppImageConfigsPaginator",
     "ListAppsPaginator",
     "ListArtifactsPaginator",
@@ -415,15 +414,14 @@
     "ListTrialsPaginator",
     "ListUserProfilesPaginator",
     "ListWorkforcesPaginator",
     "ListWorkteamsPaginator",
     "SearchPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -441,15 +439,15 @@
         *,
         SourceUri: str = ...,
         ActionType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortActionsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listactionspaginator)
         """
 
 
@@ -463,15 +461,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: AlgorithmSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAlgorithmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAlgorithms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listalgorithmspaginator)
         """
 
 
@@ -483,15 +481,15 @@
 
     def paginate(
         self,
         *,
         ImageName: str,
         Alias: str = ...,
         Version: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listaliasespaginator)
         """
 
 
@@ -507,15 +505,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppImageConfigsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAppImageConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listappimageconfigspaginator)
         """
 
 
@@ -529,15 +527,15 @@
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         DomainIdEquals: str = ...,
         UserProfileNameEquals: str = ...,
         SpaceNameEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListApps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listappspaginator)
         """
 
 
@@ -552,15 +550,15 @@
         *,
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListArtifactsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listartifactspaginator)
         """
 
 
@@ -578,15 +576,15 @@
         SourceType: str = ...,
         DestinationType: str = ...,
         AssociationType: AssociationEdgeTypeType = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortAssociationsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listassociationspaginator)
         """
 
 
@@ -603,15 +601,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: AutoMLJobStatusType = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: AutoMLSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAutoMLJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAutoMLJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listautomljobspaginator)
         """
 
 
@@ -625,15 +623,15 @@
         self,
         *,
         AutoMLJobName: str,
         StatusEquals: CandidateStatusType = ...,
         CandidateNameEquals: str = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: CandidateSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCandidatesForAutoMLJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCandidatesForAutoMLJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcandidatesforautomljobpaginator)
         """
 
 
@@ -648,15 +646,15 @@
         *,
         ClusterName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         InstanceGroupNameContains: str = ...,
         SortBy: ClusterSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClusterNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListClusterNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listclusternodespaginator)
         """
 
 
@@ -670,15 +668,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ClusterSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listclusterspaginator)
         """
 
 
@@ -694,15 +692,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: CodeRepositorySortByType = ...,
         SortOrder: CodeRepositorySortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCodeRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCodeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcoderepositoriespaginator)
         """
 
 
@@ -719,15 +717,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: CompilationJobStatusType = ...,
         SortBy: ListCompilationJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCompilationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCompilationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcompilationjobspaginator)
         """
 
 
@@ -742,15 +740,15 @@
         *,
         SourceUri: str = ...,
         ContextType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortContextsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContextsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListContexts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcontextspaginator)
         """
 
 
@@ -765,15 +763,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataQualityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDataQualityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdataqualityjobdefinitionspaginator)
         """
 
 
@@ -789,15 +787,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ListDeviceFleetsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDeviceFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdevicefleetspaginator)
         """
 
 
@@ -809,15 +807,15 @@
 
     def paginate(
         self,
         *,
         LatestHeartbeatAfter: TimestampTypeDef = ...,
         ModelName: str = ...,
         DeviceFleetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdevicespaginator)
         """
 
 
@@ -849,15 +847,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         DeviceFleetNameContains: str = ...,
         SortBy: ListEdgeDeploymentPlansSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEdgeDeploymentPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEdgeDeploymentPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listedgedeploymentplanspaginator)
         """
 
 
@@ -875,15 +873,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelNameContains: str = ...,
         StatusEquals: EdgePackagingJobStatusType = ...,
         SortBy: ListEdgePackagingJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEdgePackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEdgePackagingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listedgepackagingjobspaginator)
         """
 
 
@@ -897,15 +895,15 @@
         self,
         *,
         SortBy: EndpointConfigSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEndpointConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listendpointconfigspaginator)
         """
 
 
@@ -922,15 +920,15 @@
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: EndpointStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listendpointspaginator)
         """
 
 
@@ -943,15 +941,15 @@
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listexperimentspaginator)
         """
 
 
@@ -967,15 +965,15 @@
         NameContains: str = ...,
         FeatureGroupStatusEquals: FeatureGroupStatusType = ...,
         OfflineStoreStatusEquals: OfflineStoreStatusValueType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFeatureGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListFeatureGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listfeaturegroupspaginator)
         """
 
 
@@ -987,15 +985,15 @@
 
     def paginate(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFlowDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListFlowDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listflowdefinitionspaginator)
         """
 
 
@@ -1007,15 +1005,15 @@
 
     def paginate(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHumanTaskUisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListHumanTaskUis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listhumantaskuispaginator)
         """
 
 
@@ -1032,15 +1030,15 @@
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         StatusEquals: HyperParameterTuningJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHyperParameterTuningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListHyperParameterTuningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listhyperparametertuningjobspaginator)
         """
 
 
@@ -1056,15 +1054,15 @@
         ImageName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: ImageVersionSortByType = ...,
         SortOrder: ImageVersionSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListImageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listimageversionspaginator)
         """
 
 
@@ -1080,15 +1078,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ImageSortByType = ...,
         SortOrder: ImageSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listimagespaginator)
         """
 
 
@@ -1107,15 +1105,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: InferenceComponentStatusType = ...,
         EndpointNameEquals: str = ...,
         VariantNameEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencecomponentspaginator)
         """
 
 
@@ -1133,15 +1131,15 @@
         StatusEquals: InferenceExperimentStatusType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceExperimentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferenceexperimentspaginator)
         """
 
 
@@ -1153,15 +1151,15 @@
 
     def paginate(
         self,
         *,
         JobName: str,
         Status: RecommendationJobStatusType = ...,
         StepType: Literal["BENCHMARK"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceRecommendationsJobStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceRecommendationsJobSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencerecommendationsjobstepspaginator)
         """
 
 
@@ -1180,15 +1178,15 @@
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: RecommendationJobStatusType = ...,
         SortBy: ListInferenceRecommendationsJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
         ModelNameEquals: str = ...,
         ModelPackageVersionArnEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceRecommendationsJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceRecommendationsJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencerecommendationsjobspaginator)
         """
 
 
@@ -1205,15 +1203,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: LabelingJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLabelingJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlabelingjobspaginator)
         """
 
 
@@ -1228,15 +1226,15 @@
         *,
         WorkteamArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         JobReferenceCodeContains: str = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLabelingJobsForWorkteamResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobsForWorkteam.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlabelingjobsforworkteampaginator)
         """
 
 
@@ -1249,15 +1247,15 @@
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortLineageGroupsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLineageGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLineageGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlineagegroupspaginator)
         """
 
 
@@ -1272,15 +1270,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelBiasJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelBiasJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelbiasjobdefinitionspaginator)
         """
 
 
@@ -1297,15 +1295,15 @@
         ModelCardVersion: int = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardExportJobNameContains: str = ...,
         StatusEquals: ModelCardExportJobStatusType = ...,
         SortBy: ModelCardExportJobSortByType = ...,
         SortOrder: ModelCardExportJobSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCardExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardexportjobspaginator)
         """
 
 
@@ -1320,15 +1318,15 @@
         *,
         ModelCardName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         SortBy: Literal["Version"] = ...,
         SortOrder: ModelCardSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCardVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardversionspaginator)
         """
 
 
@@ -1343,15 +1341,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         SortBy: ModelCardSortByType = ...,
         SortOrder: ModelCardSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardspaginator)
         """
 
 
@@ -1366,15 +1364,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelExplainabilityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelExplainabilityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelexplainabilityjobdefinitionspaginator)
         """
 
 
@@ -1384,15 +1382,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         SearchExpression: ModelMetadataSearchExpressionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelMetadataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelmetadatapaginator)
         """
 
 
@@ -1406,15 +1404,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ModelPackageGroupSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelPackageGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelPackageGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelpackagegroupspaginator)
         """
 
 
@@ -1431,15 +1429,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageType: ModelPackageTypeType = ...,
         SortBy: ModelPackageSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelpackagespaginator)
         """
 
 
@@ -1454,15 +1452,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelQualityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelQualityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelqualityjobdefinitionspaginator)
         """
 
 
@@ -1476,15 +1474,15 @@
         self,
         *,
         SortBy: ModelSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelspaginator)
         """
 
 
@@ -1500,15 +1498,15 @@
         MonitoringScheduleName: str = ...,
         MonitoringAlertName: str = ...,
         SortBy: MonitoringAlertHistorySortKeyType = ...,
         SortOrder: SortOrderType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         StatusEquals: MonitoringAlertStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringAlertHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringAlertHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringalerthistorypaginator)
         """
 
 
@@ -1545,15 +1543,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ExecutionStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
         MonitoringTypeEquals: MonitoringTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringexecutionspaginator)
         """
 
 
@@ -1573,15 +1571,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ScheduleStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
         MonitoringTypeEquals: MonitoringTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringschedulespaginator)
         """
 
 
@@ -1597,15 +1595,15 @@
         SortBy: NotebookInstanceLifecycleConfigSortKeyType = ...,
         SortOrder: NotebookInstanceLifecycleConfigSortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookInstanceLifecycleConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListNotebookInstanceLifecycleConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listnotebookinstancelifecycleconfigspaginator)
         """
 
 
@@ -1625,15 +1623,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: NotebookInstanceStatusType = ...,
         NotebookInstanceLifecycleConfigNameContains: str = ...,
         DefaultCodeRepositoryContains: str = ...,
         AdditionalCodeRepositoryEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListNotebookInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listnotebookinstancespaginator)
         """
 
 
@@ -1644,15 +1642,15 @@
     """
 
     def paginate(
         self,
         *,
         PipelineExecutionArn: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelineExecutionStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelineExecutionSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelineexecutionstepspaginator)
         """
 
 
@@ -1666,15 +1664,15 @@
         self,
         *,
         PipelineName: str,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelineExecutionsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelineExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelineExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelineexecutionspaginator)
         """
 
 
@@ -1703,15 +1701,15 @@
         self,
         *,
         PipelineNamePrefix: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelinesByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelinespaginator)
         """
 
 
@@ -1728,15 +1726,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: ProcessingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProcessingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListProcessingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listprocessingjobspaginator)
         """
 
 
@@ -1750,15 +1748,15 @@
         self,
         *,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: ResourceCatalogSortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
         """
 
 
@@ -1771,15 +1769,15 @@
     def paginate(
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
         DomainIdEquals: str = ...,
         SpaceNameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListSpaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listspacespaginator)
         """
 
 
@@ -1791,15 +1789,15 @@
 
     def paginate(
         self,
         *,
         EdgeDeploymentPlanName: str,
         StageName: str,
         ExcludeDevicesDeployedInOtherStage: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStageDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListStageDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#liststagedevicespaginator)
         """
 
 
@@ -1816,15 +1814,15 @@
         AppTypeEquals: StudioLifecycleConfigAppTypeType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: StudioLifecycleConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioLifecycleConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListStudioLifecycleConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#liststudiolifecycleconfigspaginator)
         """
 
 
@@ -1872,15 +1870,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         WarmPoolStatusEquals: WarmPoolResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrainingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrainingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrainingjobspaginator)
         """
 
 
@@ -1893,15 +1891,15 @@
     def paginate(
         self,
         *,
         HyperParameterTuningJobName: str,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: TrainingJobSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrainingJobsForHyperParameterTuningJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrainingJobsForHyperParameterTuningJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrainingjobsforhyperparametertuningjobpaginator)
         """
 
 
@@ -1918,15 +1916,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TransformJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransformJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTransformJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtransformjobspaginator)
         """
 
 
@@ -1942,15 +1940,15 @@
         ExperimentName: str = ...,
         TrialName: str = ...,
         SourceArn: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialComponentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrialComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrialComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrialcomponentspaginator)
         """
 
 
@@ -1965,15 +1963,15 @@
         *,
         ExperimentName: str = ...,
         TrialComponentName: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrialsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrials.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrialspaginator)
         """
 
 
@@ -1986,15 +1984,15 @@
     def paginate(
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: UserProfileSortKeyType = ...,
         DomainIdEquals: str = ...,
         UserProfileNameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listuserprofilespaginator)
         """
 
 
@@ -2006,15 +2004,15 @@
 
     def paginate(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkforcesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkforces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listworkforcespaginator)
         """
 
 
@@ -2026,15 +2024,15 @@
 
     def paginate(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkteamsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkteams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listworkteamspaginator)
         """
 
 
@@ -2048,13 +2046,13 @@
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: SearchExpressionTypeDef = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/paginator.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,15 @@
         *,
         SourceUri: str = ...,
         ActionType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortActionsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListActions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listactionspaginator)
         """
 
 class ListAlgorithmsPaginator(AioPaginator):
@@ -458,15 +458,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: AlgorithmSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAlgorithmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAlgorithms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listalgorithmspaginator)
         """
 
 class ListAliasesPaginator(AioPaginator):
@@ -477,15 +477,15 @@
 
     def paginate(
         self,
         *,
         ImageName: str,
         Alias: str = ...,
         Version: int = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAliases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listaliasespaginator)
         """
 
 class ListAppImageConfigsPaginator(AioPaginator):
@@ -500,15 +500,15 @@
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: AppImageConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppImageConfigsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAppImageConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listappimageconfigspaginator)
         """
 
 class ListAppsPaginator(AioPaginator):
@@ -521,15 +521,15 @@
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
         DomainIdEquals: str = ...,
         UserProfileNameEquals: str = ...,
         SpaceNameEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAppsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListApps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listappspaginator)
         """
 
 class ListArtifactsPaginator(AioPaginator):
@@ -543,15 +543,15 @@
         *,
         SourceUri: str = ...,
         ArtifactType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListArtifactsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listartifactspaginator)
         """
 
 class ListAssociationsPaginator(AioPaginator):
@@ -568,15 +568,15 @@
         SourceType: str = ...,
         DestinationType: str = ...,
         AssociationType: AssociationEdgeTypeType = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortAssociationsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listassociationspaginator)
         """
 
 class ListAutoMLJobsPaginator(AioPaginator):
@@ -592,15 +592,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: AutoMLJobStatusType = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: AutoMLSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListAutoMLJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListAutoMLJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listautomljobspaginator)
         """
 
 class ListCandidatesForAutoMLJobPaginator(AioPaginator):
@@ -613,15 +613,15 @@
         self,
         *,
         AutoMLJobName: str,
         StatusEquals: CandidateStatusType = ...,
         CandidateNameEquals: str = ...,
         SortOrder: AutoMLSortOrderType = ...,
         SortBy: CandidateSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCandidatesForAutoMLJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCandidatesForAutoMLJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcandidatesforautomljobpaginator)
         """
 
 class ListClusterNodesPaginator(AioPaginator):
@@ -635,15 +635,15 @@
         *,
         ClusterName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         InstanceGroupNameContains: str = ...,
         SortBy: ClusterSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClusterNodesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListClusterNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listclusternodespaginator)
         """
 
 class ListClustersPaginator(AioPaginator):
@@ -656,15 +656,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ClusterSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listclusterspaginator)
         """
 
 class ListCodeRepositoriesPaginator(AioPaginator):
@@ -679,15 +679,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: CodeRepositorySortByType = ...,
         SortOrder: CodeRepositorySortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCodeRepositoriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCodeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcoderepositoriespaginator)
         """
 
 class ListCompilationJobsPaginator(AioPaginator):
@@ -703,15 +703,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: CompilationJobStatusType = ...,
         SortBy: ListCompilationJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListCompilationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListCompilationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcompilationjobspaginator)
         """
 
 class ListContextsPaginator(AioPaginator):
@@ -725,15 +725,15 @@
         *,
         SourceUri: str = ...,
         ContextType: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortContextsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListContextsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListContexts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listcontextspaginator)
         """
 
 class ListDataQualityJobDefinitionsPaginator(AioPaginator):
@@ -747,15 +747,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDataQualityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDataQualityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdataqualityjobdefinitionspaginator)
         """
 
 class ListDeviceFleetsPaginator(AioPaginator):
@@ -770,15 +770,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ListDeviceFleetsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDeviceFleetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDeviceFleets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdevicefleetspaginator)
         """
 
 class ListDevicesPaginator(AioPaginator):
@@ -789,15 +789,15 @@
 
     def paginate(
         self,
         *,
         LatestHeartbeatAfter: TimestampTypeDef = ...,
         ModelName: str = ...,
         DeviceFleetName: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listdevicespaginator)
         """
 
 class ListDomainsPaginator(AioPaginator):
@@ -827,15 +827,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         DeviceFleetNameContains: str = ...,
         SortBy: ListEdgeDeploymentPlansSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEdgeDeploymentPlansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEdgeDeploymentPlans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listedgedeploymentplanspaginator)
         """
 
 class ListEdgePackagingJobsPaginator(AioPaginator):
@@ -852,15 +852,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelNameContains: str = ...,
         StatusEquals: EdgePackagingJobStatusType = ...,
         SortBy: ListEdgePackagingJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEdgePackagingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEdgePackagingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listedgepackagingjobspaginator)
         """
 
 class ListEndpointConfigsPaginator(AioPaginator):
@@ -873,15 +873,15 @@
         self,
         *,
         SortBy: EndpointConfigSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEndpointConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listendpointconfigspaginator)
         """
 
 class ListEndpointsPaginator(AioPaginator):
@@ -897,15 +897,15 @@
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: EndpointStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEndpointsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListEndpoints.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listendpointspaginator)
         """
 
 class ListExperimentsPaginator(AioPaginator):
@@ -917,15 +917,15 @@
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListExperimentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listexperimentspaginator)
         """
 
 class ListFeatureGroupsPaginator(AioPaginator):
@@ -940,15 +940,15 @@
         NameContains: str = ...,
         FeatureGroupStatusEquals: FeatureGroupStatusType = ...,
         OfflineStoreStatusEquals: OfflineStoreStatusValueType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: FeatureGroupSortOrderType = ...,
         SortBy: FeatureGroupSortByType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFeatureGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListFeatureGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listfeaturegroupspaginator)
         """
 
 class ListFlowDefinitionsPaginator(AioPaginator):
@@ -959,15 +959,15 @@
 
     def paginate(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListFlowDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListFlowDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listflowdefinitionspaginator)
         """
 
 class ListHumanTaskUisPaginator(AioPaginator):
@@ -978,15 +978,15 @@
 
     def paginate(
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHumanTaskUisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListHumanTaskUis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listhumantaskuispaginator)
         """
 
 class ListHyperParameterTuningJobsPaginator(AioPaginator):
@@ -1002,15 +1002,15 @@
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         StatusEquals: HyperParameterTuningJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListHyperParameterTuningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListHyperParameterTuningJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listhyperparametertuningjobspaginator)
         """
 
 class ListImageVersionsPaginator(AioPaginator):
@@ -1025,15 +1025,15 @@
         ImageName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: ImageVersionSortByType = ...,
         SortOrder: ImageVersionSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListImageVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listimageversionspaginator)
         """
 
 class ListImagesPaginator(AioPaginator):
@@ -1048,15 +1048,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ImageSortByType = ...,
         SortOrder: ImageSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listimagespaginator)
         """
 
 class ListInferenceComponentsPaginator(AioPaginator):
@@ -1074,15 +1074,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: InferenceComponentStatusType = ...,
         EndpointNameEquals: str = ...,
         VariantNameEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceComponentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencecomponentspaginator)
         """
 
 class ListInferenceExperimentsPaginator(AioPaginator):
@@ -1099,15 +1099,15 @@
         StatusEquals: InferenceExperimentStatusType = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         SortBy: SortInferenceExperimentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceExperimentsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceExperiments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferenceexperimentspaginator)
         """
 
 class ListInferenceRecommendationsJobStepsPaginator(AioPaginator):
@@ -1118,15 +1118,15 @@
 
     def paginate(
         self,
         *,
         JobName: str,
         Status: RecommendationJobStatusType = ...,
         StepType: Literal["BENCHMARK"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceRecommendationsJobStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceRecommendationsJobSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencerecommendationsjobstepspaginator)
         """
 
 class ListInferenceRecommendationsJobsPaginator(AioPaginator):
@@ -1144,15 +1144,15 @@
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: RecommendationJobStatusType = ...,
         SortBy: ListInferenceRecommendationsJobsSortByType = ...,
         SortOrder: SortOrderType = ...,
         ModelNameEquals: str = ...,
         ModelPackageVersionArnEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListInferenceRecommendationsJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListInferenceRecommendationsJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listinferencerecommendationsjobspaginator)
         """
 
 class ListLabelingJobsPaginator(AioPaginator):
@@ -1168,15 +1168,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         StatusEquals: LabelingJobStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLabelingJobsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlabelingjobspaginator)
         """
 
 class ListLabelingJobsForWorkteamPaginator(AioPaginator):
@@ -1190,15 +1190,15 @@
         *,
         WorkteamArn: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         JobReferenceCodeContains: str = ...,
         SortBy: Literal["CreationTime"] = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLabelingJobsForWorkteamResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLabelingJobsForWorkteam.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlabelingjobsforworkteampaginator)
         """
 
 class ListLineageGroupsPaginator(AioPaginator):
@@ -1210,15 +1210,15 @@
     def paginate(
         self,
         *,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortLineageGroupsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListLineageGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListLineageGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listlineagegroupspaginator)
         """
 
 class ListModelBiasJobDefinitionsPaginator(AioPaginator):
@@ -1232,15 +1232,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelBiasJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelBiasJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelbiasjobdefinitionspaginator)
         """
 
 class ListModelCardExportJobsPaginator(AioPaginator):
@@ -1256,15 +1256,15 @@
         ModelCardVersion: int = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardExportJobNameContains: str = ...,
         StatusEquals: ModelCardExportJobStatusType = ...,
         SortBy: ModelCardExportJobSortByType = ...,
         SortOrder: ModelCardExportJobSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCardExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardexportjobspaginator)
         """
 
 class ListModelCardVersionsPaginator(AioPaginator):
@@ -1278,15 +1278,15 @@
         *,
         ModelCardName: str,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         SortBy: Literal["Version"] = ...,
         SortOrder: ModelCardSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCardVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardversionspaginator)
         """
 
 class ListModelCardsPaginator(AioPaginator):
@@ -1300,15 +1300,15 @@
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelCardStatus: ModelCardStatusType = ...,
         SortBy: ModelCardSortByType = ...,
         SortOrder: ModelCardSortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelCardsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelCards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelcardspaginator)
         """
 
 class ListModelExplainabilityJobDefinitionsPaginator(AioPaginator):
@@ -1322,15 +1322,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelExplainabilityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelExplainabilityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelexplainabilityjobdefinitionspaginator)
         """
 
 class ListModelMetadataPaginator(AioPaginator):
@@ -1339,15 +1339,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelmetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         SearchExpression: ModelMetadataSearchExpressionTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelMetadataResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelmetadatapaginator)
         """
 
 class ListModelPackageGroupsPaginator(AioPaginator):
@@ -1360,15 +1360,15 @@
         self,
         *,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         SortBy: ModelPackageGroupSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelPackageGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelPackageGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelpackagegroupspaginator)
         """
 
 class ListModelPackagesPaginator(AioPaginator):
@@ -1384,15 +1384,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         ModelApprovalStatus: ModelApprovalStatusType = ...,
         ModelPackageGroupName: str = ...,
         ModelPackageType: ModelPackageTypeType = ...,
         SortBy: ModelPackageSortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelPackagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelPackages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelpackagespaginator)
         """
 
 class ListModelQualityJobDefinitionsPaginator(AioPaginator):
@@ -1406,15 +1406,15 @@
         *,
         EndpointName: str = ...,
         SortBy: MonitoringJobDefinitionSortKeyType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelQualityJobDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModelQualityJobDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelqualityjobdefinitionspaginator)
         """
 
 class ListModelsPaginator(AioPaginator):
@@ -1427,15 +1427,15 @@
         self,
         *,
         SortBy: ModelSortKeyType = ...,
         SortOrder: OrderKeyType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmodelspaginator)
         """
 
 class ListMonitoringAlertHistoryPaginator(AioPaginator):
@@ -1450,15 +1450,15 @@
         MonitoringScheduleName: str = ...,
         MonitoringAlertName: str = ...,
         SortBy: MonitoringAlertHistorySortKeyType = ...,
         SortOrder: SortOrderType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         StatusEquals: MonitoringAlertStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringAlertHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringAlertHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringalerthistorypaginator)
         """
 
 class ListMonitoringAlertsPaginator(AioPaginator):
@@ -1493,15 +1493,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ExecutionStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
         MonitoringTypeEquals: MonitoringTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringexecutionspaginator)
         """
 
 class ListMonitoringSchedulesPaginator(AioPaginator):
@@ -1520,15 +1520,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: ScheduleStatusType = ...,
         MonitoringJobDefinitionName: str = ...,
         MonitoringTypeEquals: MonitoringTypeType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListMonitoringSchedulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListMonitoringSchedules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listmonitoringschedulespaginator)
         """
 
 class ListNotebookInstanceLifecycleConfigsPaginator(AioPaginator):
@@ -1543,15 +1543,15 @@
         SortBy: NotebookInstanceLifecycleConfigSortKeyType = ...,
         SortOrder: NotebookInstanceLifecycleConfigSortOrderType = ...,
         NameContains: str = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookInstanceLifecycleConfigsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListNotebookInstanceLifecycleConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listnotebookinstancelifecycleconfigspaginator)
         """
 
 class ListNotebookInstancesPaginator(AioPaginator):
@@ -1570,15 +1570,15 @@
         CreationTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         StatusEquals: NotebookInstanceStatusType = ...,
         NotebookInstanceLifecycleConfigNameContains: str = ...,
         DefaultCodeRepositoryContains: str = ...,
         AdditionalCodeRepositoryEquals: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListNotebookInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListNotebookInstances.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listnotebookinstancespaginator)
         """
 
 class ListPipelineExecutionStepsPaginator(AioPaginator):
@@ -1588,15 +1588,15 @@
     """
 
     def paginate(
         self,
         *,
         PipelineExecutionArn: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelineExecutionStepsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelineExecutionSteps.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelineexecutionstepspaginator)
         """
 
 class ListPipelineExecutionsPaginator(AioPaginator):
@@ -1609,15 +1609,15 @@
         self,
         *,
         PipelineName: str,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelineExecutionsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelineExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelineExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelineexecutionspaginator)
         """
 
 class ListPipelineParametersForExecutionPaginator(AioPaginator):
@@ -1644,15 +1644,15 @@
         self,
         *,
         PipelineNamePrefix: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortPipelinesByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listpipelinespaginator)
         """
 
 class ListProcessingJobsPaginator(AioPaginator):
@@ -1668,15 +1668,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: ProcessingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListProcessingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListProcessingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listprocessingjobspaginator)
         """
 
 class ListResourceCatalogsPaginator(AioPaginator):
@@ -1689,15 +1689,15 @@
         self,
         *,
         NameContains: str = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: ResourceCatalogSortOrderType = ...,
         SortBy: Literal["CreationTime"] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListResourceCatalogsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListResourceCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listresourcecatalogspaginator)
         """
 
 class ListSpacesPaginator(AioPaginator):
@@ -1709,15 +1709,15 @@
     def paginate(
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: SpaceSortKeyType = ...,
         DomainIdEquals: str = ...,
         SpaceNameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListSpacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListSpaces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listspacespaginator)
         """
 
 class ListStageDevicesPaginator(AioPaginator):
@@ -1728,15 +1728,15 @@
 
     def paginate(
         self,
         *,
         EdgeDeploymentPlanName: str,
         StageName: str,
         ExcludeDevicesDeployedInOtherStage: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStageDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListStageDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#liststagedevicespaginator)
         """
 
 class ListStudioLifecycleConfigsPaginator(AioPaginator):
@@ -1752,15 +1752,15 @@
         AppTypeEquals: StudioLifecycleConfigAppTypeType = ...,
         CreationTimeBefore: TimestampTypeDef = ...,
         CreationTimeAfter: TimestampTypeDef = ...,
         ModifiedTimeBefore: TimestampTypeDef = ...,
         ModifiedTimeAfter: TimestampTypeDef = ...,
         SortBy: StudioLifecycleConfigSortKeyType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListStudioLifecycleConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListStudioLifecycleConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#liststudiolifecycleconfigspaginator)
         """
 
 class ListSubscribedWorkteamsPaginator(AioPaginator):
@@ -1805,15 +1805,15 @@
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
         WarmPoolStatusEquals: WarmPoolResourceStatusType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrainingJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrainingJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrainingjobspaginator)
         """
 
 class ListTrainingJobsForHyperParameterTuningJobPaginator(AioPaginator):
@@ -1825,15 +1825,15 @@
     def paginate(
         self,
         *,
         HyperParameterTuningJobName: str,
         StatusEquals: TrainingJobStatusType = ...,
         SortBy: TrainingJobSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrainingJobsForHyperParameterTuningJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrainingJobsForHyperParameterTuningJob.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrainingjobsforhyperparametertuningjobpaginator)
         """
 
 class ListTransformJobsPaginator(AioPaginator):
@@ -1849,15 +1849,15 @@
         CreationTimeBefore: TimestampTypeDef = ...,
         LastModifiedTimeAfter: TimestampTypeDef = ...,
         LastModifiedTimeBefore: TimestampTypeDef = ...,
         NameContains: str = ...,
         StatusEquals: TransformJobStatusType = ...,
         SortBy: SortByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTransformJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTransformJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtransformjobspaginator)
         """
 
 class ListTrialComponentsPaginator(AioPaginator):
@@ -1872,15 +1872,15 @@
         ExperimentName: str = ...,
         TrialName: str = ...,
         SourceArn: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialComponentsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrialComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrialComponents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrialcomponentspaginator)
         """
 
 class ListTrialsPaginator(AioPaginator):
@@ -1894,15 +1894,15 @@
         *,
         ExperimentName: str = ...,
         TrialComponentName: str = ...,
         CreatedAfter: TimestampTypeDef = ...,
         CreatedBefore: TimestampTypeDef = ...,
         SortBy: SortTrialsByType = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListTrialsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListTrials.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listtrialspaginator)
         """
 
 class ListUserProfilesPaginator(AioPaginator):
@@ -1914,15 +1914,15 @@
     def paginate(
         self,
         *,
         SortOrder: SortOrderType = ...,
         SortBy: UserProfileSortKeyType = ...,
         DomainIdEquals: str = ...,
         UserProfileNameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListUserProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListUserProfiles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listuserprofilespaginator)
         """
 
 class ListWorkforcesPaginator(AioPaginator):
@@ -1933,15 +1933,15 @@
 
     def paginate(
         self,
         *,
         SortBy: ListWorkforcesSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkforcesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkforces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listworkforcespaginator)
         """
 
 class ListWorkteamsPaginator(AioPaginator):
@@ -1952,15 +1952,15 @@
 
     def paginate(
         self,
         *,
         SortBy: ListWorkteamsSortByOptionsType = ...,
         SortOrder: SortOrderType = ...,
         NameContains: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListWorkteamsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.ListWorkteams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#listworkteamspaginator)
         """
 
 class SearchPaginator(AioPaginator):
@@ -1973,13 +1973,13 @@
         self,
         *,
         Resource: ResourceTypeType,
         SearchExpression: SearchExpressionTypeDef = ...,
         SortBy: str = ...,
         SortOrder: SearchSortOrderType = ...,
         CrossAccountFilterOption: CrossAccountFilterOptionType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[SearchResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/type_defs.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActionSourceTypeDef",
     "AddAssociationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "AdditionalS3DataSourceTypeDef",
     "AgentVersionTypeDef",
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/type_defs.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/waiter.py` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     async def wait(
         self,
         *,
         ImageName: str,
         Version: int = ...,
         Alias: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionCreated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/waiters/#imageversioncreatedwaiter)
         """
 
 
@@ -159,15 +159,15 @@
 
     async def wait(
         self,
         *,
         ImageName: str,
         Version: int = ...,
         Alias: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/waiters/#imageversiondeletedwaiter)
         """
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker/waiter.pyi` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 
     async def wait(
         self,
         *,
         ImageName: str,
         Version: int = ...,
         Alias: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionCreated.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/waiters/#imageversioncreatedwaiter)
         """
 
 class ImageVersionDeletedWaiter(AIOWaiter):
@@ -152,15 +152,15 @@
 
     async def wait(
         self,
         *,
         ImageName: str,
         Version: int = ...,
         Alias: str = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker.Waiter.ImageVersionDeleted.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/waiters/#imageversiondeletedwaiter)
         """
 
 class NotebookInstanceDeletedWaiter(AIOWaiter):
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.SageMaker 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.SageMaker 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/
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
 
 <a id="types-aiobotocore-sagemaker"></a>
 
 # types-aiobotocore-sagemaker
 
 [![PyPI - types-aiobotocore-sagemaker](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker)](https://pepy.tech/project/types-aiobotocore-sagemaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.SageMaker 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
+[aiobotocore.SageMaker 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#SageMaker)
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
 [types-aiobotocore-sagemaker docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-sagemaker-2.9.0/types_aiobotocore_sagemaker.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-2.9.1/types_aiobotocore_sagemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

