# Comparing `tmp/types-aiobotocore-elastic-inference-2.9.0.tar.gz` & `tmp/types-aiobotocore-elastic-inference-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastic-inference-2.9.0.tar", last modified: Wed Dec 13 19:59:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastic-inference-2.9.1.tar", last modified: Thu Jan 18 01:20:38 2024, max compression
```

## Comparing `types-aiobotocore-elastic-inference-2.9.0.tar` & `types-aiobotocore-elastic-inference-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.797775 types-aiobotocore-elastic-inference-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2023-12-13 19:59:13.797775 types-aiobotocore-elastic-inference-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:13.797775 types-aiobotocore-elastic-inference-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.797775 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      970 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8609 2023-12-13 19:45:37.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8607 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2023-12-13 19:45:37.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2023-12-13 19:45:37.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:45:36.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:13.797775 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13605 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-13 19:59:13.000000 types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.701352 types-aiobotocore-elastic-inference-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-01-18 01:20:38.701352 types-aiobotocore-elastic-inference-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:38.701352 types-aiobotocore-elastic-inference-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.701352 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-01-18 01:07:33.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8607 2024-01-18 01:07:33.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-01-18 01:07:33.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-01-18 01:07:33.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:07:32.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:38.701352 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-18 01:20:38.000000 types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/LICENSE` & `types-aiobotocore-elastic-inference-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-elastic-inference-2.9.0/PKG-INFO` & `types-aiobotocore-elastic-inference-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticInference 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticInference 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
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
 
 <a id="types-aiobotocore-elastic-inference"></a>
 
 # types-aiobotocore-elastic-inference
 
 [![PyPI - types-aiobotocore-elastic-inference](https://img.shields.io/pypi/v/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/README.md` & `types-aiobotocore-elastic-inference-2.9.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/setup.py` & `types-aiobotocore-elastic-inference-2.9.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastic-inference",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.ElasticInference 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.ElasticInference 2.9.1 service generated with"
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
     keywords="aiobotocore elastic-inference type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elastic_inference": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__init__.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,9 +22,8 @@
 """
 
 from .client import ElasticInferenceClient
 from .paginator import DescribeAcceleratorsPaginator
 
 Client = ElasticInferenceClient
 
-
 __all__ = ("Client", "DescribeAcceleratorsPaginator", "ElasticInferenceClient")
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__init__.pyi` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/__main__.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticInference 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.ElasticInference 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/client.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ElasticInferenceClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -112,15 +111,15 @@
 
     async def describe_accelerators(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAcceleratorsResponseTypeDef:
         """
         Describes information over a provided set of accelerators belonging to an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/client/#describe_accelerators)
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/client.pyi` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 
     async def describe_accelerators(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         maxResults: int = ...,
-        nextToken: str = ...
+        nextToken: str = ...,
     ) -> DescribeAcceleratorsResponseTypeDef:
         """
         Describes information over a provided set of accelerators belonging to an
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Client.describe_accelerators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/client/#describe_accelerators)
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/literals.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,26 +15,24 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeAcceleratorsPaginatorName",
     "LocationTypeType",
     "ElasticInferenceServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeAcceleratorsPaginatorName = Literal["describe_accelerators"]
 LocationTypeType = Literal["availability-zone", "availability-zone-id", "region"]
 ElasticInferenceServiceName = Literal["elastic-inference"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/literals.pyi` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/paginator.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import DescribeAcceleratorsResponseTypeDef, FilterTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeAcceleratorsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
@@ -48,13 +47,13 @@
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/paginator.pyi` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,13 +45,13 @@
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/type_defs.py` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceleratorTypeOfferingTypeDef",
     "KeyValuePairTypeDef",
     "MemoryInfoTypeDef",
     "DescribeAcceleratorOfferingsRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "FilterTypeDef",
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference/type_defs.pyi` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/PKG-INFO` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.ElasticInference 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.ElasticInference 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
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
 
 <a id="types-aiobotocore-elastic-inference"></a>
 
 # types-aiobotocore-elastic-inference
 
 [![PyPI - types-aiobotocore-elastic-inference](https://img.shields.io/pypi/v/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastic-inference.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastic-inference)](https://pepy.tech/project/types-aiobotocore-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.ElasticInference 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[aiobotocore.ElasticInference 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-elastic-inference-2.9.0/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt` & `types-aiobotocore-elastic-inference-2.9.1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

