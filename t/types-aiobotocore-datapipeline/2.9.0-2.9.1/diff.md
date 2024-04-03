# Comparing `tmp/types-aiobotocore-datapipeline-2.9.0.tar.gz` & `tmp/types-aiobotocore-datapipeline-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-datapipeline-2.9.0.tar", last modified: Wed Dec 13 19:59:03 2023, max compression
+gzip compressed data, was "types-aiobotocore-datapipeline-2.9.1.tar", last modified: Thu Jan 18 01:20:29 2024, max compression
```

## Comparing `types-aiobotocore-datapipeline-2.9.0.tar` & `types-aiobotocore-datapipeline-2.9.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.833857 types-aiobotocore-datapipeline-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2023-12-13 19:59:03.833857 types-aiobotocore-datapipeline-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11925 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:59:03.833857 types-aiobotocore-datapipeline-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.833857 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      952 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18148 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8799 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13442 2023-12-13 19:43:48.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13441 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-12-13 19:43:47.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:59:03.833857 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13508 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      908 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-12-13 19:59:03.000000 types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.429400 types-aiobotocore-datapipeline-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-01-18 01:20:29.429400 types-aiobotocore-datapipeline-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11925 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:20:29.429400 types-aiobotocore-datapipeline-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.429400 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18158 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-18 01:05:42.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:20:29.429400 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-01-18 01:20:29.000000 types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/LICENSE` & `types-aiobotocore-datapipeline-2.9.1/LICENSE`

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

### Comparing `types-aiobotocore-datapipeline-2.9.0/PKG-INFO` & `types-aiobotocore-datapipeline-2.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataPipeline 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataPipeline 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
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
 
 <a id="types-aiobotocore-datapipeline"></a>
 
 # types-aiobotocore-datapipeline
 
 [![PyPI - types-aiobotocore-datapipeline](https://img.shields.io/pypi/v/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datapipeline)](https://pepy.tech/project/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/README.md` & `types-aiobotocore-datapipeline-2.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datapipeline)](https://pepy.tech/project/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/setup.py` & `types-aiobotocore-datapipeline-2.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,48 +7,47 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-datapipeline",
-    version="2.9.0",
+    version="2.9.1",
     packages=["types_aiobotocore_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.DataPipeline 2.9.0 service generated with"
-        " mypy-boto3-builder 7.21.0"
+        "Type annotations for aiobotocore.DataPipeline 2.9.1 service generated with"
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
     keywords="aiobotocore datapipeline type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_datapipeline": ["py.typed", "*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__init__.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 """
 
 from .client import DataPipelineClient
 from .paginator import DescribeObjectsPaginator, ListPipelinesPaginator, QueryObjectsPaginator
 
 Client = DataPipelineClient
 
-
 __all__ = (
     "Client",
     "DataPipelineClient",
     "DescribeObjectsPaginator",
     "ListPipelinesPaginator",
     "QueryObjectsPaginator",
 )
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__init__.pyi` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/__main__.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DataPipeline 2.9.0\nVersion:         2.9.0\nBuilder"
-        " version: 7.21.0\nDocs:           "
+        "Type annotations for aiobotocore.DataPipeline 2.9.1\nVersion:         2.9.1\nBuilder"
+        " version: 7.23.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/client.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 )
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DataPipelineClient",)
 
 
 class BotocoreClientError(Exception):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -91,15 +90,15 @@
         """
 
     async def activate_pipeline(
         self,
         *,
         pipelineId: str,
         parameterValues: Sequence[ParameterValueTypeDef] = ...,
-        startTimestamp: TimestampTypeDef = ...
+        startTimestamp: TimestampTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Validates the specified pipeline and starts processing pipeline tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.activate_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#activate_pipeline)
         """
@@ -158,15 +157,15 @@
 
     async def describe_objects(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        marker: str = ...
+        marker: str = ...,
     ) -> DescribeObjectsOutputTypeDef:
         """
         Gets the object definitions for a set of objects associated with the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#describe_objects)
         """
@@ -228,15 +227,15 @@
         """
 
     async def poll_for_task(
         self,
         *,
         workerGroup: str,
         hostname: str = ...,
-        instanceIdentity: InstanceIdentityTypeDef = ...
+        instanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> PollForTaskOutputTypeDef:
         """
         Task runners call `PollForTask` to receive a task to perform from AWS Data
         Pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#poll_for_task)
@@ -244,15 +243,15 @@
 
     async def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
         pipelineObjects: Sequence[PipelineObjectTypeDef],
         parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
-        parameterValues: Sequence[ParameterValueTypeDef] = ...
+        parameterValues: Sequence[ParameterValueTypeDef] = ...,
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#put_pipeline_definition)
         """
@@ -260,15 +259,15 @@
     async def query_objects(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
         marker: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> QueryObjectsOutputTypeDef:
         """
         Queries the specified pipeline for the names of objects that match the
         specified set of
         conditions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.query_objects)
@@ -322,15 +321,15 @@
     async def set_task_status(
         self,
         *,
         taskId: str,
         taskStatus: TaskStatusType,
         errorId: str = ...,
         errorMessage: str = ...,
-        errorStackTrace: str = ...
+        errorStackTrace: str = ...,
     ) -> Dict[str, Any]:
         """
         Task runners call `SetTaskStatus` to notify AWS Data Pipeline that a task is
         completed and provide information about the final
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
@@ -339,15 +338,15 @@
 
     async def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
         pipelineObjects: Sequence[PipelineObjectTypeDef],
         parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
-        parameterValues: Sequence[ParameterValueTypeDef] = ...
+        parameterValues: Sequence[ParameterValueTypeDef] = ...,
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed
         and can be run without
         error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/client.pyi` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         """
 
     async def activate_pipeline(
         self,
         *,
         pipelineId: str,
         parameterValues: Sequence[ParameterValueTypeDef] = ...,
-        startTimestamp: TimestampTypeDef = ...
+        startTimestamp: TimestampTypeDef = ...,
     ) -> Dict[str, Any]:
         """
         Validates the specified pipeline and starts processing pipeline tasks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.activate_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#activate_pipeline)
         """
@@ -154,15 +154,15 @@
 
     async def describe_objects(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        marker: str = ...
+        marker: str = ...,
     ) -> DescribeObjectsOutputTypeDef:
         """
         Gets the object definitions for a set of objects associated with the pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.describe_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#describe_objects)
         """
@@ -224,15 +224,15 @@
         """
 
     async def poll_for_task(
         self,
         *,
         workerGroup: str,
         hostname: str = ...,
-        instanceIdentity: InstanceIdentityTypeDef = ...
+        instanceIdentity: InstanceIdentityTypeDef = ...,
     ) -> PollForTaskOutputTypeDef:
         """
         Task runners call `PollForTask` to receive a task to perform from AWS Data
         Pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.poll_for_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#poll_for_task)
@@ -240,15 +240,15 @@
 
     async def put_pipeline_definition(
         self,
         *,
         pipelineId: str,
         pipelineObjects: Sequence[PipelineObjectTypeDef],
         parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
-        parameterValues: Sequence[ParameterValueTypeDef] = ...
+        parameterValues: Sequence[ParameterValueTypeDef] = ...,
     ) -> PutPipelineDefinitionOutputTypeDef:
         """
         Adds tasks, schedules, and preconditions to the specified pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.put_pipeline_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/client/#put_pipeline_definition)
         """
@@ -256,15 +256,15 @@
     async def query_objects(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
         marker: str = ...,
-        limit: int = ...
+        limit: int = ...,
     ) -> QueryObjectsOutputTypeDef:
         """
         Queries the specified pipeline for the names of objects that match the
         specified set of
         conditions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.query_objects)
@@ -318,15 +318,15 @@
     async def set_task_status(
         self,
         *,
         taskId: str,
         taskStatus: TaskStatusType,
         errorId: str = ...,
         errorMessage: str = ...,
-        errorStackTrace: str = ...
+        errorStackTrace: str = ...,
     ) -> Dict[str, Any]:
         """
         Task runners call `SetTaskStatus` to notify AWS Data Pipeline that a task is
         completed and provide information about the final
         status.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.set_task_status)
@@ -335,15 +335,15 @@
 
     async def validate_pipeline_definition(
         self,
         *,
         pipelineId: str,
         pipelineObjects: Sequence[PipelineObjectTypeDef],
         parameterObjects: Sequence[ParameterObjectTypeDef] = ...,
-        parameterValues: Sequence[ParameterValueTypeDef] = ...
+        parameterValues: Sequence[ParameterValueTypeDef] = ...,
     ) -> ValidatePipelineDefinitionOutputTypeDef:
         """
         Validates the specified pipeline definition to ensure that it is well formed
         and can be run without
         error.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Client.validate_pipeline_definition)
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/literals.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,27 @@
 import sys
 
 if sys.version_info >= (3, 12):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DescribeObjectsPaginatorName",
     "ListPipelinesPaginatorName",
     "OperatorTypeType",
     "QueryObjectsPaginatorName",
     "TaskStatusType",
     "DataPipelineServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DescribeObjectsPaginatorName = Literal["describe_objects"]
 ListPipelinesPaginatorName = Literal["list_pipelines"]
 OperatorTypeType = Literal["BETWEEN", "EQ", "GE", "LE", "REF_EQ"]
 QueryObjectsPaginatorName = Literal["query_objects"]
 TaskStatusType = Literal["FAILED", "FALSE", "FINISHED"]
 DataPipelineServiceName = Literal["datapipeline"]
 ServiceName = Literal[
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/literals.pyi` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/paginator.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,71 +36,66 @@
     PaginatorConfigTypeDef,
     QueryObjectsOutputTypeDef,
     QueryTypeDef,
 )
 
 __all__ = ("DescribeObjectsPaginator", "ListPipelinesPaginator", "QueryObjectsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeObjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#describeobjectspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#describeobjectspaginator)
         """
 
-
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#listpipelinespaginator)
         """
 
-
 class QueryObjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#queryobjectspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/paginator.pyi` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,64 +38,68 @@
     QueryTypeDef,
 )
 
 __all__ = ("DescribeObjectsPaginator", "ListPipelinesPaginator", "QueryObjectsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeObjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#describeobjectspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#describeobjectspaginator)
         """
 
+
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
         self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#listpipelinespaginator)
         """
 
+
 class QueryObjectsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#queryobjectspaginator)
     """
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> AsyncIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/type_defs.py` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 else:
     from typing_extensions import NotRequired
 if sys.version_info >= (3, 12):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ParameterValueTypeDef",
     "TimestampTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline/type_defs.pyi` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/PKG-INFO` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-datapipeline
-Version: 2.9.0
-Summary: Type annotations for aiobotocore.DataPipeline 2.9.0 service generated with mypy-boto3-builder 7.21.0
+Version: 2.9.1
+Summary: Type annotations for aiobotocore.DataPipeline 2.9.1 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/
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
 
 <a id="types-aiobotocore-datapipeline"></a>
 
 # types-aiobotocore-datapipeline
 
 [![PyPI - types-aiobotocore-datapipeline](https://img.shields.io/pypi/v/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-datapipeline.svg?color=blue)](https://pypi.org/project/types-aiobotocore-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-datapipeline)](https://pepy.tech/project/types-aiobotocore-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore.DataPipeline 2.9.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[aiobotocore.DataPipeline 2.9.1](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [types-aiobotocore-datapipeline docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_datapipeline/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `types-aiobotocore-datapipeline-2.9.0/types_aiobotocore_datapipeline.egg-info/SOURCES.txt` & `types-aiobotocore-datapipeline-2.9.1/types_aiobotocore_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

