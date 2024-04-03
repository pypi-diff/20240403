# Comparing `tmp/types-aiobotocore-ecr-2.9.0.tar.gz` & `tmp/types-aiobotocore-ecr-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-2.9.0.tar", last modified: Wed Dec 13 19:59:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-2.9.1.tar", last modified: Thu Jan 18 01:20:36 2024, max compression
```

## Comparing `types-aiobotocore-ecr-2.9.0.tar` & `types-aiobotocore-ecr-2.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.565793 types-aiobotocore-ecr-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2023-12-13 19:59:11.561793 types-aiobotocore-ecr-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12938 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:11.565793 types-aiobotocore-ecr-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.561793 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37486 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37482 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2023-12-13 19:45:23.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11968 2023-12-13 19:45:23.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8542 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    43259 2023-12-13 19:45:23.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    43258 2023-12-13 19:45:23.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-12-13 19:45:22.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:11.561793 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14485 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-13 19:59:11.000000 types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.625362 types-aiobotocore-ecr-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14505 2024-01-18 01:20:36.625362 types-aiobotocore-ecr-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12938 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:36.625362 types-aiobotocore-ecr-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.625362 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37500 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37497 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11968 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    43258 2024-01-18 01:07:20.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43258 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:18.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-01-18 01:07:19.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:36.625362 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14505 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 01:20:36.000000 types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-2.9.0/LICENSE` & `types-aiobotocore-ecr-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-ecr-2.9.0/PKG-INFO` & `types-aiobotocore-ecr-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECR 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECR 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
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
 
 <a id="types-aiobotocore-ecr"></a>
 
 # types-aiobotocore-ecr
 
 [![PyPI - types-aiobotocore-ecr](https://img.shields.io/pypi/v/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-2.9.0/README.md` & `types-aiobotocore-ecr-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-2.9.0/setup.py` & `types-aiobotocore-ecr-2.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_ecr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ECR 2.9.0 service generated with mypy-boto3-builder"
-        " 7.21.0"
+        "Type annotations for aiobotocore.ECR 2.9.1 service generated with mypy-boto3-builder"
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
     keywords="aiobotocore ecr type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ecr": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__init__.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     GetLifecyclePolicyPreviewPaginator,
     ListImagesPaginator,
 )
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
 
 Client = ECRClient
 
-
 __all__ = (
     "Client",
     "DescribeImageScanFindingsPaginator",
     "DescribeImagesPaginator",
     "DescribePullThroughCacheRulesPaginator",
     "DescribeRepositoriesPaginator",
     "ECRClient",
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__init__.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/__main__.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECR 2.9.0\nVersion:         2.9.0\nBuilder version:"
-        " 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ECR 2.9.1\nVersion:         2.9.1\nBuilder version:"
+        " 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR\nOther"
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

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/client.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 from .waiter import ImageScanCompleteWaiter, LifecyclePolicyPreviewCompleteWaiter
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ECRClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -172,30 +171,30 @@
         """
 
     async def batch_delete_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> BatchDeleteImageResponseTypeDef:
         """
         Deletes a list of specified images within a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.batch_delete_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#batch_delete_image)
         """
 
     async def batch_get_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
         registryId: str = ...,
-        acceptedMediaTypes: Sequence[str] = ...
+        acceptedMediaTypes: Sequence[str] = ...,
     ) -> BatchGetImageResponseTypeDef:
         """
         Gets detailed information for an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.batch_get_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#batch_get_image)
         """
@@ -228,15 +227,15 @@
 
     async def complete_layer_upload(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         layerDigests: Sequence[str],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> CompleteLayerUploadResponseTypeDef:
         """
         Informs Amazon ECR that the image layer upload has completed for a specified
         registry, repository name, and upload
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.complete_layer_upload)
@@ -246,15 +245,15 @@
     async def create_pull_through_cache_rule(
         self,
         *,
         ecrRepositoryPrefix: str,
         upstreamRegistryUrl: str,
         registryId: str = ...,
         upstreamRegistry: UpstreamRegistryType = ...,
-        credentialArn: str = ...
+        credentialArn: str = ...,
     ) -> CreatePullThroughCacheRuleResponseTypeDef:
         """
         Creates a pull through cache rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.create_pull_through_cache_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#create_pull_through_cache_rule)
         """
@@ -263,15 +262,15 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         imageTagMutability: ImageTagMutabilityType = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
-        encryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateRepositoryResponseTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#create_repository)
         """
@@ -337,15 +336,15 @@
     async def describe_image_scan_findings(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImageScanFindingsResponseTypeDef:
         """
         Returns the scan findings for the specified image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_image_scan_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_image_scan_findings)
         """
@@ -354,30 +353,30 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: DescribeImagesFilterTypeDef = ...
+        filter: DescribeImagesFilterTypeDef = ...,
     ) -> DescribeImagesResponseTypeDef:
         """
         Returns metadata about the images in a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_images)
         """
 
     async def describe_pull_through_cache_rules(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribePullThroughCacheRulesResponseTypeDef:
         """
         Returns the pull through cache rules for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_pull_through_cache_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_pull_through_cache_rules)
         """
@@ -392,15 +391,15 @@
 
     async def describe_repositories(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRepositoriesResponseTypeDef:
         """
         Describes image repositories in a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_repositories)
         """
@@ -453,15 +452,15 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: LifecyclePolicyPreviewFilterTypeDef = ...
+        filter: LifecyclePolicyPreviewFilterTypeDef = ...,
     ) -> GetLifecyclePolicyPreviewResponseTypeDef:
         """
         Retrieves the results of the lifecycle policy preview request for the specified
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.get_lifecycle_policy_preview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#get_lifecycle_policy_preview)
@@ -508,15 +507,15 @@
     async def list_images(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListImagesFilterTypeDef = ...
+        filter: ListImagesFilterTypeDef = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Lists all the image IDs for the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#list_images)
         """
@@ -535,43 +534,43 @@
         self,
         *,
         repositoryName: str,
         imageManifest: str,
         registryId: str = ...,
         imageManifestMediaType: str = ...,
         imageTag: str = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> PutImageResponseTypeDef:
         """
         Creates or updates the image manifest and tags associated with an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image)
         """
 
     async def put_image_scanning_configuration(
         self,
         *,
         repositoryName: str,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutImageScanningConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image_scanning_configuration)
         """
 
     async def put_image_tag_mutability(
         self,
         *,
         repositoryName: str,
         imageTagMutability: ImageTagMutabilityType,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutImageTagMutabilityResponseTypeDef:
         """
         Updates the image tag mutability settings for the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image_tag_mutability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image_tag_mutability)
         """
@@ -675,15 +674,15 @@
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
         layerPartBlob: BlobTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#upload_layer_part)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/client.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -168,30 +168,30 @@
         """
 
     async def batch_delete_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> BatchDeleteImageResponseTypeDef:
         """
         Deletes a list of specified images within a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.batch_delete_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#batch_delete_image)
         """
 
     async def batch_get_image(
         self,
         *,
         repositoryName: str,
         imageIds: Sequence[ImageIdentifierTypeDef],
         registryId: str = ...,
-        acceptedMediaTypes: Sequence[str] = ...
+        acceptedMediaTypes: Sequence[str] = ...,
     ) -> BatchGetImageResponseTypeDef:
         """
         Gets detailed information for an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.batch_get_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#batch_get_image)
         """
@@ -224,15 +224,15 @@
 
     async def complete_layer_upload(
         self,
         *,
         repositoryName: str,
         uploadId: str,
         layerDigests: Sequence[str],
-        registryId: str = ...
+        registryId: str = ...,
     ) -> CompleteLayerUploadResponseTypeDef:
         """
         Informs Amazon ECR that the image layer upload has completed for a specified
         registry, repository name, and upload
         ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.complete_layer_upload)
@@ -242,15 +242,15 @@
     async def create_pull_through_cache_rule(
         self,
         *,
         ecrRepositoryPrefix: str,
         upstreamRegistryUrl: str,
         registryId: str = ...,
         upstreamRegistry: UpstreamRegistryType = ...,
-        credentialArn: str = ...
+        credentialArn: str = ...,
     ) -> CreatePullThroughCacheRuleResponseTypeDef:
         """
         Creates a pull through cache rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.create_pull_through_cache_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#create_pull_through_cache_rule)
         """
@@ -259,15 +259,15 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         imageTagMutability: ImageTagMutabilityType = ...,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef = ...,
-        encryptionConfiguration: EncryptionConfigurationTypeDef = ...
+        encryptionConfiguration: EncryptionConfigurationTypeDef = ...,
     ) -> CreateRepositoryResponseTypeDef:
         """
         Creates a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.create_repository)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#create_repository)
         """
@@ -333,15 +333,15 @@
     async def describe_image_scan_findings(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeImageScanFindingsResponseTypeDef:
         """
         Returns the scan findings for the specified image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_image_scan_findings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_image_scan_findings)
         """
@@ -350,30 +350,30 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: DescribeImagesFilterTypeDef = ...
+        filter: DescribeImagesFilterTypeDef = ...,
     ) -> DescribeImagesResponseTypeDef:
         """
         Returns metadata about the images in a repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_images)
         """
 
     async def describe_pull_through_cache_rules(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribePullThroughCacheRulesResponseTypeDef:
         """
         Returns the pull through cache rules for a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_pull_through_cache_rules)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_pull_through_cache_rules)
         """
@@ -388,15 +388,15 @@
 
     async def describe_repositories(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRepositoriesResponseTypeDef:
         """
         Describes image repositories in a registry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.describe_repositories)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#describe_repositories)
         """
@@ -449,15 +449,15 @@
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: LifecyclePolicyPreviewFilterTypeDef = ...
+        filter: LifecyclePolicyPreviewFilterTypeDef = ...,
     ) -> GetLifecyclePolicyPreviewResponseTypeDef:
         """
         Retrieves the results of the lifecycle policy preview request for the specified
         repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.get_lifecycle_policy_preview)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#get_lifecycle_policy_preview)
@@ -504,15 +504,15 @@
     async def list_images(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        filter: ListImagesFilterTypeDef = ...
+        filter: ListImagesFilterTypeDef = ...,
     ) -> ListImagesResponseTypeDef:
         """
         Lists all the image IDs for the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.list_images)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#list_images)
         """
@@ -531,43 +531,43 @@
         self,
         *,
         repositoryName: str,
         imageManifest: str,
         registryId: str = ...,
         imageManifestMediaType: str = ...,
         imageTag: str = ...,
-        imageDigest: str = ...
+        imageDigest: str = ...,
     ) -> PutImageResponseTypeDef:
         """
         Creates or updates the image manifest and tags associated with an image.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image)
         """
 
     async def put_image_scanning_configuration(
         self,
         *,
         repositoryName: str,
         imageScanningConfiguration: ImageScanningConfigurationTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutImageScanningConfigurationResponseTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image_scanning_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image_scanning_configuration)
         """
 
     async def put_image_tag_mutability(
         self,
         *,
         repositoryName: str,
         imageTagMutability: ImageTagMutabilityType,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> PutImageTagMutabilityResponseTypeDef:
         """
         Updates the image tag mutability settings for the specified repository.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.put_image_tag_mutability)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#put_image_tag_mutability)
         """
@@ -671,15 +671,15 @@
         self,
         *,
         repositoryName: str,
         uploadId: str,
         partFirstByte: int,
         partLastByte: int,
         layerPartBlob: BlobTypeDef,
-        registryId: str = ...
+        registryId: str = ...,
     ) -> UploadLayerPartResponseTypeDef:
         """
         Uploads an image layer part to Amazon ECR.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Client.upload_layer_part)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/client/#upload_layer_part)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/literals.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/literals.py`

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
     "DescribeImageScanFindingsPaginatorName",
     "DescribeImagesPaginatorName",
     "DescribePullThroughCacheRulesPaginatorName",
     "DescribeRepositoriesPaginatorName",
     "EncryptionTypeType",
     "FindingSeverityType",
@@ -50,15 +49,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 DescribeImageScanFindingsPaginatorName = Literal["describe_image_scan_findings"]
 DescribeImagesPaginatorName = Literal["describe_images"]
 DescribePullThroughCacheRulesPaginatorName = Literal["describe_pull_through_cache_rules"]
 DescribeRepositoriesPaginatorName = Literal["describe_repositories"]
 EncryptionTypeType = Literal["AES256", "KMS"]
 FindingSeverityType = Literal["CRITICAL", "HIGH", "INFORMATIONAL", "LOW", "MEDIUM", "UNDEFINED"]
 GetLifecyclePolicyPreviewPaginatorName = Literal["get_lifecycle_policy_preview"]
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/literals.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/paginator.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,14 @@
     "DescribeImagesPaginator",
     "DescribePullThroughCacheRulesPaginator",
     "DescribeRepositoriesPaginator",
     "GetLifecyclePolicyPreviewPaginator",
     "ListImagesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -78,15 +77,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 
@@ -99,15 +98,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagespaginator)
         """
 
 
@@ -118,15 +117,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 
@@ -137,15 +136,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describerepositoriespaginator)
         """
 
 
@@ -158,15 +157,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 
@@ -178,13 +177,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/paginator.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImageScanFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImageScanFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagescanfindingspaginator)
         """
 
 class DescribeImagesPaginator(AioPaginator):
@@ -95,15 +95,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: DescribeImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describeimagespaginator)
         """
 
 class DescribePullThroughCacheRulesPaginator(AioPaginator):
@@ -113,15 +113,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         ecrRepositoryPrefixes: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribePullThroughCacheRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribePullThroughCacheRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describepullthroughcacherulespaginator)
         """
 
 class DescribeRepositoriesPaginator(AioPaginator):
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         registryId: str = ...,
         repositoryNames: Sequence[str] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRepositoriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.DescribeRepositories.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#describerepositoriespaginator)
         """
 
 class GetLifecyclePolicyPreviewPaginator(AioPaginator):
@@ -151,15 +151,15 @@
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLifecyclePolicyPreviewResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.GetLifecyclePolicyPreview.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#getlifecyclepolicypreviewpaginator)
         """
 
 class ListImagesPaginator(AioPaginator):
@@ -170,13 +170,13 @@
 
     def paginate(
         self,
         *,
         repositoryName: str,
         registryId: str = ...,
         filter: ListImagesFilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListImagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Paginator.ListImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/paginators/#listimagespaginator)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/type_defs.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AttributeTypeDef",
     "AuthorizationDataTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "BatchCheckLayerAvailabilityRequestRequestTypeDef",
     "LayerFailureTypeDef",
     "LayerTypeDef",
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/type_defs.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/waiter.py` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/waiter.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.ImageScanComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/waiters/#imagescancompletewaiter)
         """
 
 
@@ -69,13 +69,13 @@
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.LifecyclePolicyPreviewComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/waiters/#lifecyclepolicypreviewcompletewaiter)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr/waiter.pyi` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr/waiter.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         self,
         *,
         repositoryName: str,
         imageId: ImageIdentifierTypeDef,
         registryId: str = ...,
         nextToken: str = ...,
         maxResults: int = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.ImageScanComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/waiters/#imagescancompletewaiter)
         """
 
 class LifecyclePolicyPreviewCompleteWaiter(AIOWaiter):
@@ -67,13 +67,13 @@
         *,
         repositoryName: str,
         registryId: str = ...,
         imageIds: Sequence[ImageIdentifierTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filter: LifecyclePolicyPreviewFilterTypeDef = ...,
-        WaiterConfig: WaiterConfigTypeDef = ...
+        WaiterConfig: WaiterConfigTypeDef = ...,
     ) -> None:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR.Waiter.LifecyclePolicyPreviewComplete.wait)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/waiters/#lifecyclepolicypreviewcompletewaiter)
         """
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/PKG-INFO` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ECR 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ECR 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/
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
 
 <a id="types-aiobotocore-ecr"></a>
 
 # types-aiobotocore-ecr
 
 [![PyPI - types-aiobotocore-ecr](https://img.shields.io/pypi/v/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ecr)](https://pepy.tech/project/types-aiobotocore-ecr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ECR 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
+[aiobotocore.ECR 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ECR)
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
 [types-aiobotocore-ecr docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-ecr-2.9.0/types_aiobotocore_ecr.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-2.9.1/types_aiobotocore_ecr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

