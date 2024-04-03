# Comparing `tmp/types-aiobotocore-cost-optimization-hub-2.9.0.tar.gz` & `tmp/types-aiobotocore-cost-optimization-hub-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cost-optimization-hub-2.9.0.tar", last modified: Wed Dec 13 19:59:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-cost-optimization-hub-2.9.1.tar", last modified: Thu Jan 18 01:20:27 2024, max compression
```

## Comparing `types-aiobotocore-cost-optimization-hub-2.9.0.tar` & `types-aiobotocore-cost-optimization-hub-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.977872 types-aiobotocore-cost-optimization-hub-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2023-12-13 19:59:01.977872 types-aiobotocore-cost-optimization-hub-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:01.977872 types-aiobotocore-cost-optimization-hub-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.977872 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11460 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    24479 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24478 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:37.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:01.977872 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-12-13 19:59:01.000000 types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.721409 types-aiobotocore-cost-optimization-hub-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-01-18 01:20:27.721409 types-aiobotocore-cost-optimization-hub-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:27.721409 types-aiobotocore-cost-optimization-hub-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.721409 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-01-18 01:05:34.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24478 2024-01-18 01:05:33.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:32.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:27.721409 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14187 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-01-18 01:20:27.000000 types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/LICENSE` & `types-aiobotocore-cost-optimization-hub-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/PKG-INFO` & `types-aiobotocore-cost-optimization-hub-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cost-optimization-hub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostOptimizationHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostOptimizationHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/
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
 
 <a id="types-aiobotocore-cost-optimization-hub"></a>
 
 # types-aiobotocore-cost-optimization-hub
 
 [![PyPI - types-aiobotocore-cost-optimization-hub](https://img.shields.io/pypi/v/types-aiobotocore-cost-optimization-hub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cost-optimization-hub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cost-optimization-hub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cost-optimization-hub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cost-optimization-hub)](https://pepy.tech/project/types-aiobotocore-cost-optimization-hub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostOptimizationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
+[aiobotocore.CostOptimizationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
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
 [types-aiobotocore-cost-optimization-hub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/README.md` & `types-aiobotocore-cost-optimization-hub-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cost-optimization-hub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cost-optimization-hub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cost-optimization-hub)](https://pepy.tech/project/types-aiobotocore-cost-optimization-hub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostOptimizationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
+[aiobotocore.CostOptimizationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
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
 [types-aiobotocore-cost-optimization-hub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/setup.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,50 +7,49 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cost-optimization-hub",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_cost_optimization_hub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.CostOptimizationHub 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.CostOptimizationHub 2.9.1 service generated with"
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
     keywords=(
         "aiobotocore cost-optimization-hub type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cost_optimization_hub": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         'typing-extensions>=4.1.0; python_version<"3.12"',
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__init__.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ListEnrollmentStatusesPaginator,
     ListRecommendationsPaginator,
     ListRecommendationSummariesPaginator,
 )
 
 Client = CostOptimizationHubClient
 
-
 __all__ = (
     "Client",
     "CostOptimizationHubClient",
     "ListEnrollmentStatusesPaginator",
     "ListRecommendationSummariesPaginator",
     "ListRecommendationsPaginator",
 )
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__init__.pyi` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/__main__.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostOptimizationHub 2.9.0\nVersion:        "
-        " 2.9.0\nBuilder version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.CostOptimizationHub 2.9.1\nVersion:        "
+        " 2.9.1\nBuilder version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub\nOther"
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

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/client.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,35 +44,31 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("CostOptimizationHubClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class CostOptimizationHubClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/)
     """
 
     meta: ClientMeta
@@ -140,30 +136,30 @@
 
     async def list_enrollment_statuses(
         self,
         *,
         accountId: str = ...,
         includeOrganizationInfo: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnrollmentStatusesResponseTypeDef:
         """
         Retrieves the enrollment status for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_enrollment_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_enrollment_statuses)
         """
 
     async def list_recommendation_summaries(
         self,
         *,
         groupBy: str,
         filter: FilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRecommendationSummariesResponseTypeDef:
         """
         Returns a concise representation of savings estimates for resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_recommendation_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_recommendation_summaries)
         """
@@ -171,15 +167,15 @@
     async def list_recommendations(
         self,
         *,
         filter: FilterTypeDef = ...,
         includeAllRecommendations: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: OrderByTypeDef = ...
+        orderBy: OrderByTypeDef = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Returns a list of recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_recommendations)
         """
@@ -196,15 +192,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#update_enrollment_status)
         """
 
     async def update_preferences(
         self,
         *,
         memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType = ...,
-        savingsEstimationMode: SavingsEstimationModeType = ...
+        savingsEstimationMode: SavingsEstimationModeType = ...,
     ) -> UpdatePreferencesResponseTypeDef:
         """
         Updates a set of preferences for an account in order to add account-specific
         preferences into the
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.update_preferences)
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/client.pyi` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,29 +46,32 @@
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = ("CostOptimizationHubClient",)
 
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
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class CostOptimizationHubClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/)
     """
 
     meta: ClientMeta
@@ -136,30 +139,30 @@
 
     async def list_enrollment_statuses(
         self,
         *,
         accountId: str = ...,
         includeOrganizationInfo: bool = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListEnrollmentStatusesResponseTypeDef:
         """
         Retrieves the enrollment status for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_enrollment_statuses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_enrollment_statuses)
         """
 
     async def list_recommendation_summaries(
         self,
         *,
         groupBy: str,
         filter: FilterTypeDef = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> ListRecommendationSummariesResponseTypeDef:
         """
         Returns a concise representation of savings estimates for resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_recommendation_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_recommendation_summaries)
         """
@@ -167,15 +170,15 @@
     async def list_recommendations(
         self,
         *,
         filter: FilterTypeDef = ...,
         includeAllRecommendations: bool = ...,
         maxResults: int = ...,
         nextToken: str = ...,
-        orderBy: OrderByTypeDef = ...
+        orderBy: OrderByTypeDef = ...,
     ) -> ListRecommendationsResponseTypeDef:
         """
         Returns a list of recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.list_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#list_recommendations)
         """
@@ -192,15 +195,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/client/#update_enrollment_status)
         """
 
     async def update_preferences(
         self,
         *,
         memberAccountDiscountVisibility: MemberAccountDiscountVisibilityType = ...,
-        savingsEstimationMode: SavingsEstimationModeType = ...
+        savingsEstimationMode: SavingsEstimationModeType = ...,
     ) -> UpdatePreferencesResponseTypeDef:
         """
         Updates a set of preferences for an account in order to add account-specific
         preferences into the
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Client.update_preferences)
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/literals.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/literals.py`

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
     "ActionTypeType",
     "EnrollmentStatusType",
     "ImplementationEffortType",
     "ListEnrollmentStatusesPaginatorName",
     "ListRecommendationSummariesPaginatorName",
     "ListRecommendationsPaginatorName",
@@ -35,15 +34,14 @@
     "CostOptimizationHubServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ActionTypeType = Literal[
     "MigrateToGraviton",
     "PurchaseReservedInstances",
     "PurchaseSavingsPlans",
     "Rightsize",
     "Stop",
     "Upgrade",
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/literals.pyi` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/paginator.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
 __all__ = (
     "ListEnrollmentStatusesPaginator",
     "ListRecommendationSummariesPaginator",
     "ListRecommendationsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -63,15 +62,15 @@
     """
 
     def paginate(
         self,
         *,
         accountId: str = ...,
         includeOrganizationInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnrollmentStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListEnrollmentStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listenrollmentstatusespaginator)
         """
 
 
@@ -82,15 +81,15 @@
     """
 
     def paginate(
         self,
         *,
         groupBy: str,
         filter: FilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendationSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listrecommendationsummariespaginator)
         """
 
 
@@ -102,13 +101,13 @@
 
     def paginate(
         self,
         *,
         filter: FilterTypeDef = ...,
         includeAllRecommendations: bool = ...,
         orderBy: OrderByTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listrecommendationspaginator)
         """
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/paginator.pyi` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
 
     def paginate(
         self,
         *,
         accountId: str = ...,
         includeOrganizationInfo: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListEnrollmentStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListEnrollmentStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listenrollmentstatusespaginator)
         """
 
 class ListRecommendationSummariesPaginator(AioPaginator):
@@ -78,15 +78,15 @@
     """
 
     def paginate(
         self,
         *,
         groupBy: str,
         filter: FilterTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendationSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listrecommendationsummariespaginator)
         """
 
 class ListRecommendationsPaginator(AioPaginator):
@@ -97,13 +97,13 @@
 
     def paginate(
         self,
         *,
         filter: FilterTypeDef = ...,
         includeAllRecommendations: bool = ...,
         orderBy: OrderByTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/paginators/#listrecommendationspaginator)
         """
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/type_defs.py` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountEnrollmentStatusTypeDef",
     "BlockStoragePerformanceConfigurationTypeDef",
     "ComputeConfigurationTypeDef",
     "ComputeSavingsPlansConfigurationTypeDef",
     "StorageConfigurationTypeDef",
     "InstanceConfigurationTypeDef",
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub/type_defs.pyi` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/PKG-INFO` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cost-optimization-hub
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.CostOptimizationHub 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.CostOptimizationHub 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/
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
 
 <a id="types-aiobotocore-cost-optimization-hub"></a>
 
 # types-aiobotocore-cost-optimization-hub
 
 [![PyPI - types-aiobotocore-cost-optimization-hub](https://img.shields.io/pypi/v/types-aiobotocore-cost-optimization-hub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cost-optimization-hub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cost-optimization-hub.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cost-optimization-hub)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cost-optimization-hub)](https://pepy.tech/project/types-aiobotocore-cost-optimization-hub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.CostOptimizationHub 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
+[aiobotocore.CostOptimizationHub 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#CostOptimizationHub)
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
 [types-aiobotocore-cost-optimization-hub docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cost_optimization_hub/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-cost-optimization-hub-2.9.0/types_aiobotocore_cost_optimization_hub.egg-info/SOURCES.txt` & `types-aiobotocore-cost-optimization-hub-2.9.1/types_aiobotocore_cost_optimization_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

