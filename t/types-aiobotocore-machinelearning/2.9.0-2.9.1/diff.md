# Comparing `tmp/types-aiobotocore-machinelearning-2.9.0.tar.gz` & `tmp/types-aiobotocore-machinelearning-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-machinelearning-2.9.0.tar", last modified: Wed Dec 13 19:59:48 2023, max compression
+gzip compressed data, was "types-aiobotocore-machinelearning-2.9.1.tar", last modified: Thu Jan 18 01:21:11 2024, max compression
```

## Comparing `types-aiobotocore-machinelearning-2.9.0.tar` & `types-aiobotocore-machinelearning-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.961501 types-aiobotocore-machinelearning-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2023-12-13 19:59:48.961501 types-aiobotocore-machinelearning-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:48.961501 types-aiobotocore-machinelearning-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.961501 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      964 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28085 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28081 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10855 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    10853 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30923 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30922 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:49:34.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6336 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2023-12-13 19:49:35.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:48.961501 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15137 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2023-12-13 19:59:48.000000 types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.205204 types-aiobotocore-machinelearning-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-18 01:21:11.205204 types-aiobotocore-machinelearning-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:21:11.205204 types-aiobotocore-machinelearning-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.201204 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28094 2024-01-18 01:11:21.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28091 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-01-18 01:11:22.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10853 2024-01-18 01:11:22.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-01-18 01:11:21.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-01-18 01:11:21.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30922 2024-01-18 01:11:22.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30922 2024-01-18 01:11:22.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:11:19.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-01-18 01:11:21.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6336 2024-01-18 01:11:21.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:21:11.205204 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15157 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-18 01:21:11.000000 types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/LICENSE` & `types-aiobotocore-machinelearning-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-machinelearning-2.9.0/PKG-INFO` & `types-aiobotocore-machinelearning-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MachineLearning 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MachineLearning 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
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
 
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/README.md` & `types-aiobotocore-machinelearning-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/setup.py` & `types-aiobotocore-machinelearning-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-machinelearning",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.MachineLearning 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.MachineLearning 2.9.1 service generated with"
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
     keywords="aiobotocore machinelearning type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_machinelearning": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__init__.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     DataSourceAvailableWaiter,
     EvaluationAvailableWaiter,
     MLModelAvailableWaiter,
 )
 
 Client = MachineLearningClient
 
-
 __all__ = (
     "BatchPredictionAvailableWaiter",
     "Client",
     "DataSourceAvailableWaiter",
     "DescribeBatchPredictionsPaginator",
     "DescribeDataSourcesPaginator",
     "DescribeEvaluationsPaginator",
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__init__.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/__main__.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MachineLearning 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.MachineLearning 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
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

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/client.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("MachineLearningClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -152,15 +151,15 @@
     async def create_batch_prediction(
         self,
         *,
         BatchPredictionId: str,
         MLModelId: str,
         BatchPredictionDataSourceId: str,
         OutputUri: str,
-        BatchPredictionName: str = ...
+        BatchPredictionName: str = ...,
     ) -> CreateBatchPredictionOutputTypeDef:
         """
         Generates predictions for a group of observations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_batch_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_batch_prediction)
         """
@@ -168,15 +167,15 @@
     async def create_data_source_from_rds(
         self,
         *,
         DataSourceId: str,
         RDSData: RDSDataSpecTypeDef,
         RoleARN: str,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromRDSOutputTypeDef:
         """
         Creates a `DataSource` object from an `Amazon Relational Database Service
         <http://aws.amazon.com/rds/>`__ (Amazon
         RDS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_rds)
@@ -186,45 +185,45 @@
     async def create_data_source_from_redshift(
         self,
         *,
         DataSourceId: str,
         DataSpec: RedshiftDataSpecTypeDef,
         RoleARN: str,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromRedshiftOutputTypeDef:
         """
         Creates a `DataSource` from a database hosted on an Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_redshift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_data_source_from_redshift)
         """
 
     async def create_data_source_from_s3(
         self,
         *,
         DataSourceId: str,
         DataSpec: S3DataSpecTypeDef,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromS3OutputTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_data_source_from_s3)
         """
 
     async def create_evaluation(
         self,
         *,
         EvaluationId: str,
         MLModelId: str,
         EvaluationDataSourceId: str,
-        EvaluationName: str = ...
+        EvaluationName: str = ...,
     ) -> CreateEvaluationOutputTypeDef:
         """
         Creates a new `Evaluation` of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_evaluation)
         """
@@ -234,15 +233,15 @@
         *,
         MLModelId: str,
         MLModelType: MLModelTypeType,
         TrainingDataSourceId: str,
         MLModelName: str = ...,
         Parameters: Mapping[str, str] = ...,
         Recipe: str = ...,
-        RecipeUri: str = ...
+        RecipeUri: str = ...,
     ) -> CreateMLModelOutputTypeDef:
         """
         Creates a new `MLModel` using the `DataSource` and the recipe as information
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_ml_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_ml_model)
@@ -321,15 +320,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeBatchPredictionsOutputTypeDef:
         """
         Returns a list of `BatchPrediction` operations that match the search criteria
         in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_batch_predictions)
@@ -345,15 +344,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeDataSourcesOutputTypeDef:
         """
         Returns a list of `DataSource` that match the search criteria in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_data_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_data_sources)
         """
@@ -367,15 +366,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeEvaluationsOutputTypeDef:
         """
         Returns a list of `DescribeEvaluations` that match the search criteria in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_evaluations)
@@ -390,15 +389,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeMLModelsOutputTypeDef:
         """
         Returns a list of `MLModel` that match the search criteria in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_ml_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_ml_models)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/client.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     async def create_batch_prediction(
         self,
         *,
         BatchPredictionId: str,
         MLModelId: str,
         BatchPredictionDataSourceId: str,
         OutputUri: str,
-        BatchPredictionName: str = ...
+        BatchPredictionName: str = ...,
     ) -> CreateBatchPredictionOutputTypeDef:
         """
         Generates predictions for a group of observations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_batch_prediction)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_batch_prediction)
         """
@@ -164,15 +164,15 @@
     async def create_data_source_from_rds(
         self,
         *,
         DataSourceId: str,
         RDSData: RDSDataSpecTypeDef,
         RoleARN: str,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromRDSOutputTypeDef:
         """
         Creates a `DataSource` object from an `Amazon Relational Database Service
         <http://aws.amazon.com/rds/>`__ (Amazon
         RDS).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_rds)
@@ -182,45 +182,45 @@
     async def create_data_source_from_redshift(
         self,
         *,
         DataSourceId: str,
         DataSpec: RedshiftDataSpecTypeDef,
         RoleARN: str,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromRedshiftOutputTypeDef:
         """
         Creates a `DataSource` from a database hosted on an Amazon Redshift cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_redshift)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_data_source_from_redshift)
         """
 
     async def create_data_source_from_s3(
         self,
         *,
         DataSourceId: str,
         DataSpec: S3DataSpecTypeDef,
         DataSourceName: str = ...,
-        ComputeStatistics: bool = ...
+        ComputeStatistics: bool = ...,
     ) -> CreateDataSourceFromS3OutputTypeDef:
         """
         Creates a `DataSource` object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_data_source_from_s3)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_data_source_from_s3)
         """
 
     async def create_evaluation(
         self,
         *,
         EvaluationId: str,
         MLModelId: str,
         EvaluationDataSourceId: str,
-        EvaluationName: str = ...
+        EvaluationName: str = ...,
     ) -> CreateEvaluationOutputTypeDef:
         """
         Creates a new `Evaluation` of an `MLModel`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_evaluation)
         """
@@ -230,15 +230,15 @@
         *,
         MLModelId: str,
         MLModelType: MLModelTypeType,
         TrainingDataSourceId: str,
         MLModelName: str = ...,
         Parameters: Mapping[str, str] = ...,
         Recipe: str = ...,
-        RecipeUri: str = ...
+        RecipeUri: str = ...,
     ) -> CreateMLModelOutputTypeDef:
         """
         Creates a new `MLModel` using the `DataSource` and the recipe as information
         sources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.create_ml_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#create_ml_model)
@@ -317,15 +317,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeBatchPredictionsOutputTypeDef:
         """
         Returns a list of `BatchPrediction` operations that match the search criteria
         in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_batch_predictions)
@@ -341,15 +341,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeDataSourcesOutputTypeDef:
         """
         Returns a list of `DataSource` that match the search criteria in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_data_sources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_data_sources)
         """
@@ -363,15 +363,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeEvaluationsOutputTypeDef:
         """
         Returns a list of `DescribeEvaluations` that match the search criteria in the
         request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_evaluations)
@@ -386,15 +386,15 @@
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
-        Limit: int = ...
+        Limit: int = ...,
     ) -> DescribeMLModelsOutputTypeDef:
         """
         Returns a list of `MLModel` that match the search criteria in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Client.describe_ml_models)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/client/#describe_ml_models)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/literals.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/literals.py`

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
     "AlgorithmType",
     "BatchPredictionAvailableWaiterName",
     "BatchPredictionFilterVariableType",
     "DataSourceAvailableWaiterName",
     "DataSourceFilterVariableType",
     "DescribeBatchPredictionsPaginatorName",
@@ -44,15 +43,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AlgorithmType = Literal["sgd"]
 BatchPredictionAvailableWaiterName = Literal["batch_prediction_available"]
 BatchPredictionFilterVariableType = Literal[
     "CreatedAt",
     "DataSourceId",
     "DataURI",
     "IAMUser",
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/literals.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/paginator.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 __all__ = (
     "DescribeBatchPredictionsPaginator",
     "DescribeDataSourcesPaginator",
     "DescribeEvaluationsPaginator",
     "DescribeMLModelsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -79,15 +78,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 
@@ -105,15 +104,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 
@@ -131,15 +130,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 
@@ -157,13 +156,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/paginator.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 class DescribeDataSourcesPaginator(AioPaginator):
@@ -101,15 +101,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 class DescribeEvaluationsPaginator(AioPaginator):
@@ -126,15 +126,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 class DescribeMLModelsPaginator(AioPaginator):
@@ -151,13 +151,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/type_defs.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/type_defs.py`

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
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
     "S3DataSpecTypeDef",
     "CreateEvaluationInputRequestTypeDef",
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/type_defs.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/waiter.py` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.BatchPredictionAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#batchpredictionavailablewaiter)
         """
 
 
@@ -90,15 +90,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.DataSourceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#datasourceavailablewaiter)
         """
 
 
@@ -118,15 +118,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.EvaluationAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#evaluationavailablewaiter)
         """
 
 
@@ -146,13 +146,13 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.MLModelAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#mlmodelavailablewaiter)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning/waiter.pyi` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.BatchPredictionAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#batchpredictionavailablewaiter)
         """
 
 class DataSourceAvailableWaiter(AIOWaiter):
@@ -88,15 +88,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.DataSourceAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#datasourceavailablewaiter)
         """
 
 class EvaluationAvailableWaiter(AIOWaiter):
@@ -115,15 +115,15 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.EvaluationAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#evaluationavailablewaiter)
         """
 
 class MLModelAvailableWaiter(AIOWaiter):
@@ -142,13 +142,13 @@
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         Limit: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Waiter.MLModelAvailable.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/waiters/#mlmodelavailablewaiter)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/PKG-INFO` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.MachineLearning 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.MachineLearning 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
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
 
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.MachineLearning 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
+[aiobotocore.MachineLearning 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
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
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-machinelearning-2.9.0/types_aiobotocore_machinelearning.egg-info/SOURCES.txt` & `types-aiobotocore-machinelearning-2.9.1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

