# Comparing `tmp/types-aiobotocore-compute-optimizer-2.9.0.tar.gz` & `tmp/types-aiobotocore-compute-optimizer-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-compute-optimizer-2.9.0.tar", last modified: Wed Dec 13 19:58:58 2023, max compression
+gzip compressed data, was "types-aiobotocore-compute-optimizer-2.9.1.tar", last modified: Thu Jan 18 01:20:24 2024, max compression
```

## Comparing `types-aiobotocore-compute-optimizer-2.9.0.tar` & `types-aiobotocore-compute-optimizer-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.933897 types-aiobotocore-compute-optimizer-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2023-12-13 19:58:58.933897 types-aiobotocore-compute-optimizer-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12902 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:58.933897 types-aiobotocore-compute-optimizer-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.933897 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28630 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    28626 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    30409 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    30407 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8251 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53128 2023-12-13 19:43:17.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53127 2023-12-13 19:43:16.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:15.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:58.933897 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:58:58.000000 types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.925422 types-aiobotocore-compute-optimizer-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-01-18 01:20:24.925422 types-aiobotocore-compute-optimizer-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12902 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:24.925422 types-aiobotocore-compute-optimizer-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.925422 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28648 2024-01-18 01:05:12.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28645 2024-01-18 01:05:11.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-01-18 01:05:12.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30407 2024-01-18 01:05:12.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-01-18 01:05:12.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-01-18 01:05:12.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53127 2024-01-18 01:05:13.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53127 2024-01-18 01:05:13.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:10.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:24.925422 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14524 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:24.000000 types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/LICENSE` & `types-aiobotocore-compute-optimizer-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ComputeOptimizer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ComputeOptimizer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
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
 
 <a id="types-aiobotocore-compute-optimizer"></a>
 
 # types-aiobotocore-compute-optimizer
 
 [![PyPI - types-aiobotocore-compute-optimizer](https://img.shields.io/pypi/v/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComputeOptimizer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[aiobotocore.ComputeOptimizer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/README.md` & `types-aiobotocore-compute-optimizer-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComputeOptimizer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[aiobotocore.ComputeOptimizer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/setup.py` & `types-aiobotocore-compute-optimizer-2.9.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-compute-optimizer",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ComputeOptimizer 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ComputeOptimizer 2.9.1 service generated with"
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
     keywords="aiobotocore compute-optimizer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_compute_optimizer": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__init__.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     GetLambdaFunctionRecommendationsPaginator,
     GetRecommendationPreferencesPaginator,
     GetRecommendationSummariesPaginator,
 )
 
 Client = ComputeOptimizerClient
 
-
 __all__ = (
     "Client",
     "ComputeOptimizerClient",
     "DescribeRecommendationExportJobsPaginator",
     "GetEnrollmentStatusesForOrganizationPaginator",
     "GetLambdaFunctionRecommendationsPaginator",
     "GetRecommendationPreferencesPaginator",
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__init__.pyi` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/__main__.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ComputeOptimizer 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ComputeOptimizer 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
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

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/client.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ComputeOptimizerClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -146,30 +145,30 @@
         """
 
     async def delete_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],
-        scope: ScopeTypeDef = ...
+        scope: ScopeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a recommendation preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.delete_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#delete_recommendation_preferences)
         """
 
     async def describe_recommendation_export_jobs(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRecommendationExportJobsResponseTypeDef:
         """
         Describes recommendation export jobs created in the last seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.describe_recommendation_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#describe_recommendation_export_jobs)
         """
@@ -179,15 +178,15 @@
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableAutoScalingGroupFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
         includeMemberAccounts: bool = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> ExportAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_auto_scaling_group_recommendations)
         """
@@ -196,15 +195,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableVolumeFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportEBSVolumeRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ebs_volume_recommendations)
         """
@@ -214,15 +213,15 @@
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableInstanceFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
         includeMemberAccounts: bool = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> ExportEC2InstanceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ec2_instance_recommendations)
         """
@@ -231,15 +230,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableECSServiceFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportECSServiceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon ECS services on Fargate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ecs_service_recommendations)
         """
@@ -248,15 +247,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLambdaFunctionFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportLambdaFunctionRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Lambda functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_lambda_function_recommendations)
         """
@@ -265,15 +264,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLicenseFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportLicenseRecommendationsResponseTypeDef:
         """
         Export optimization recommendations for your licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_license_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_license_recommendations)
         """
@@ -296,15 +295,15 @@
         self,
         *,
         accountIds: Sequence[str] = ...,
         autoScalingGroupArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Returns Auto Scaling group recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_auto_scaling_group_recommendations)
         """
@@ -312,15 +311,15 @@
     async def get_ebs_volume_recommendations(
         self,
         *,
         volumeArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetEBSVolumeRecommendationsResponseTypeDef:
         """
         Returns Amazon Elastic Block Store (Amazon EBS) volume recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ebs_volume_recommendations)
         """
@@ -329,15 +328,15 @@
         self,
         *,
         instanceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
         accountIds: Sequence[str] = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetEC2InstanceRecommendationsResponseTypeDef:
         """
         Returns Amazon EC2 instance recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_instance_recommendations)
         """
@@ -346,15 +345,15 @@
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_recommendation_projected_metrics)
@@ -363,15 +362,15 @@
     async def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
         startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef
+        endTime: TimestampTypeDef,
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
@@ -379,15 +378,15 @@
     async def get_ecs_service_recommendations(
         self,
         *,
         serviceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetECSServiceRecommendationsResponseTypeDef:
         """
         Returns Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendations)
         """
@@ -414,15 +413,15 @@
         """
 
     async def get_enrollment_statuses_for_organization(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEnrollmentStatusesForOrganizationResponseTypeDef:
         """
         Returns the Compute Optimizer enrollment (opt-in) status of organization member
         accounts, if your account is an organization management
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_statuses_for_organization)
@@ -432,15 +431,15 @@
     async def get_lambda_function_recommendations(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetLambdaFunctionRecommendationsResponseTypeDef:
         """
         Returns Lambda function recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_lambda_function_recommendations)
         """
@@ -448,15 +447,15 @@
     async def get_license_recommendations(
         self,
         *,
         resourceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetLicenseRecommendationsResponseTypeDef:
         """
         Returns license recommendations for Amazon EC2 instances that run on a specific
         license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_license_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_license_recommendations)
@@ -464,15 +463,15 @@
 
     async def get_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetRecommendationPreferencesResponseTypeDef:
         """
         Returns existing recommendation preferences, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_preferences)
@@ -495,15 +494,15 @@
         scope: ScopeTypeDef = ...,
         enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType = ...,
         inferredWorkloadTypes: InferredWorkloadTypesPreferenceType = ...,
         externalMetricsPreference: ExternalMetricsPreferenceTypeDef = ...,
         lookBackPeriod: LookBackPeriodPreferenceType = ...,
         utilizationPreferences: Sequence[UtilizationPreferenceTypeDef] = ...,
         preferredResources: Sequence[PreferredResourceTypeDef] = ...,
-        savingsEstimationMode: SavingsEstimationModeType = ...
+        savingsEstimationMode: SavingsEstimationModeType = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new recommendation preference or updates an existing recommendation
         preference, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.put_recommendation_preferences)
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/client.pyi` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -142,30 +142,30 @@
         """
 
     async def delete_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],
-        scope: ScopeTypeDef = ...
+        scope: ScopeTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Deletes a recommendation preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.delete_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#delete_recommendation_preferences)
         """
 
     async def describe_recommendation_export_jobs(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> DescribeRecommendationExportJobsResponseTypeDef:
         """
         Describes recommendation export jobs created in the last seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.describe_recommendation_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#describe_recommendation_export_jobs)
         """
@@ -175,15 +175,15 @@
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableAutoScalingGroupFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
         includeMemberAccounts: bool = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> ExportAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_auto_scaling_group_recommendations)
         """
@@ -192,15 +192,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableVolumeFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportEBSVolumeRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ebs_volume_recommendations)
         """
@@ -210,15 +210,15 @@
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableInstanceFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
         includeMemberAccounts: bool = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> ExportEC2InstanceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ec2_instance_recommendations)
         """
@@ -227,15 +227,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableECSServiceFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportECSServiceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon ECS services on Fargate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ecs_service_recommendations)
         """
@@ -244,15 +244,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLambdaFunctionFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportLambdaFunctionRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Lambda functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_lambda_function_recommendations)
         """
@@ -261,15 +261,15 @@
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLicenseFieldType] = ...,
         fileFormat: Literal["Csv"] = ...,
-        includeMemberAccounts: bool = ...
+        includeMemberAccounts: bool = ...,
     ) -> ExportLicenseRecommendationsResponseTypeDef:
         """
         Export optimization recommendations for your licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_license_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_license_recommendations)
         """
@@ -292,15 +292,15 @@
         self,
         *,
         accountIds: Sequence[str] = ...,
         autoScalingGroupArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Returns Auto Scaling group recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_auto_scaling_group_recommendations)
         """
@@ -308,15 +308,15 @@
     async def get_ebs_volume_recommendations(
         self,
         *,
         volumeArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetEBSVolumeRecommendationsResponseTypeDef:
         """
         Returns Amazon Elastic Block Store (Amazon EBS) volume recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ebs_volume_recommendations)
         """
@@ -325,15 +325,15 @@
         self,
         *,
         instanceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
         accountIds: Sequence[str] = ...,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetEC2InstanceRecommendationsResponseTypeDef:
         """
         Returns Amazon EC2 instance recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_instance_recommendations)
         """
@@ -342,15 +342,15 @@
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
         startTime: TimestampTypeDef,
         endTime: TimestampTypeDef,
-        recommendationPreferences: RecommendationPreferencesTypeDef = ...
+        recommendationPreferences: RecommendationPreferencesTypeDef = ...,
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_recommendation_projected_metrics)
@@ -359,15 +359,15 @@
     async def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
         startTime: TimestampTypeDef,
-        endTime: TimestampTypeDef
+        endTime: TimestampTypeDef,
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
@@ -375,15 +375,15 @@
     async def get_ecs_service_recommendations(
         self,
         *,
         serviceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetECSServiceRecommendationsResponseTypeDef:
         """
         Returns Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendations)
         """
@@ -410,15 +410,15 @@
         """
 
     async def get_enrollment_statuses_for_organization(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetEnrollmentStatusesForOrganizationResponseTypeDef:
         """
         Returns the Compute Optimizer enrollment (opt-in) status of organization member
         accounts, if your account is an organization management
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_statuses_for_organization)
@@ -428,15 +428,15 @@
     async def get_lambda_function_recommendations(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetLambdaFunctionRecommendationsResponseTypeDef:
         """
         Returns Lambda function recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_lambda_function_recommendations)
         """
@@ -444,15 +444,15 @@
     async def get_license_recommendations(
         self,
         *,
         resourceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[LicenseRecommendationFilterTypeDef] = ...,
-        accountIds: Sequence[str] = ...
+        accountIds: Sequence[str] = ...,
     ) -> GetLicenseRecommendationsResponseTypeDef:
         """
         Returns license recommendations for Amazon EC2 instances that run on a specific
         license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_license_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_license_recommendations)
@@ -460,15 +460,15 @@
 
     async def get_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         nextToken: str = ...,
-        maxResults: int = ...
+        maxResults: int = ...,
     ) -> GetRecommendationPreferencesResponseTypeDef:
         """
         Returns existing recommendation preferences, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_preferences)
@@ -491,15 +491,15 @@
         scope: ScopeTypeDef = ...,
         enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType = ...,
         inferredWorkloadTypes: InferredWorkloadTypesPreferenceType = ...,
         externalMetricsPreference: ExternalMetricsPreferenceTypeDef = ...,
         lookBackPeriod: LookBackPeriodPreferenceType = ...,
         utilizationPreferences: Sequence[UtilizationPreferenceTypeDef] = ...,
         preferredResources: Sequence[PreferredResourceTypeDef] = ...,
-        savingsEstimationMode: SavingsEstimationModeType = ...
+        savingsEstimationMode: SavingsEstimationModeType = ...,
     ) -> Dict[str, Any]:
         """
         Creates a new recommendation preference or updates an existing recommendation
         preference, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.put_recommendation_preferences)
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/literals.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/literals.py`

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
     "AutoScalingConfigurationType",
     "CpuVendorArchitectureType",
     "CurrencyType",
     "CurrentPerformanceRiskType",
     "CustomizableMetricHeadroomType",
     "CustomizableMetricNameType",
@@ -96,15 +95,14 @@
     "ComputeOptimizerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 AutoScalingConfigurationType = Literal["TargetTrackingScalingCpu", "TargetTrackingScalingMemory"]
 CpuVendorArchitectureType = Literal["AWS_ARM64", "CURRENT"]
 CurrencyType = Literal["CNY", "USD"]
 CurrentPerformanceRiskType = Literal["High", "Low", "Medium", "VeryLow"]
 CustomizableMetricHeadroomType = Literal["PERCENT_0", "PERCENT_20", "PERCENT_30"]
 CustomizableMetricNameType = Literal["CpuUtilization"]
 CustomizableMetricThresholdType = Literal["P90", "P95", "P99_5"]
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/literals.pyi` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/paginator.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,14 @@
     "DescribeRecommendationExportJobsPaginator",
     "GetEnrollmentStatusesForOrganizationPaginator",
     "GetLambdaFunctionRecommendationsPaginator",
     "GetRecommendationPreferencesPaginator",
     "GetRecommendationSummariesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -74,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 
@@ -92,15 +91,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 
@@ -112,15 +111,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 
@@ -131,15 +130,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/paginator.pyi` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 class GetEnrollmentStatusesForOrganizationPaginator(AioPaginator):
@@ -88,15 +88,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 class GetLambdaFunctionRecommendationsPaginator(AioPaginator):
@@ -107,15 +107,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 class GetRecommendationPreferencesPaginator(AioPaginator):
@@ -125,15 +125,15 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
 class GetRecommendationSummariesPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/type_defs.py` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "AutoScalingGroupEstimatedMonthlySavingsTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer/type_defs.pyi` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ComputeOptimizer 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ComputeOptimizer 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
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
 
 <a id="types-aiobotocore-compute-optimizer"></a>
 
 # types-aiobotocore-compute-optimizer
 
 [![PyPI - types-aiobotocore-compute-optimizer](https://img.shields.io/pypi/v/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ComputeOptimizer 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
+[aiobotocore.ComputeOptimizer 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-compute-optimizer-2.9.0/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt` & `types-aiobotocore-compute-optimizer-2.9.1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

